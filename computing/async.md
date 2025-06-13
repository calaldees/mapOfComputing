Async
=====

* `async` is a language feature for performing concurrency in single threaded languages

* [Asyncio, twisted, tornado, gevent walk into a bar... they pay, they leave, they drink, they order.](https://www.bitecode.dev/p/asyncio-twisted-tornado-gevent-walk)
    * Great explanation of #concurrency in python with 3 different methods
        * -
            * concurrency is having two lines of customers ordering from a one cashier
            * parallelism is having two lines of customers ordering from two cashiers
        * Example of fetching 10 urls
* [I'm not feeling the async pressure](https://lucumr.pocoo.org/2020/1/1/async-pressure/) - Backpressure (python3 dose not have it)
* [Async Python is not faster](http://calpaterson.com/async-python-is-not-faster.html)


Python
* [asyncstdlib](https://asyncstdlib.readthedocs.io/en/stable/source/api/asynctools.html#async-transforming)
* [Decorator to facilitate sync and async calls to one function](https://discuss.python.org/t/decorator-to-facilitate-sync-and-async-calls-to-one-function/78986)
```python
import asyncio
import functools
from collections.abc import Coroutine
from typing import Callable, TypeVar, Union, Awaitable

T = TypeVar("T")


def async_or_sync(func: Callable[..., Coroutine[None, None, T]]) -> Callable[..., Union[T, Awaitable[T]]]:
    """Decorator to enable calling the same function synchronously or asynchronously.

    It determines the context in which the function is called (sync or async) and runs it appropriately.
    In an async context, the wrapped function is awaited, whereas in a sync context, it is executed using
    `asyncio.run`.

    :param func: The function to be wrapped. Must be async (`async def myfunction(...)`).
    :return: The return value of the wrapped function, modified to handle either synchronous or asynchronous execution.
    """

    @functools.wraps(func)
    def wrapper(*args, **kwargs):
        if asyncio.iscoroutinefunction(func):
            try:
                # Run asynchronously if there is an active event loop
                asyncio.get_running_loop()
                return func(*args, **kwargs)
            except RuntimeError:
                # Run synchronously
                return asyncio.run(func(*args, **kwargs))
        else:
            raise TypeError("The decorated function must be asynchronous.")

    return wrapper


if __name__ == '__main__':
    # Simple test case to show the intended use

    @async_or_sync
    async def my_test_function(name: str):
        await asyncio.sleep(1)
        print(f"Hello, {name}")
        return name


    async def async_test_caller():
        x = await my_test_function("Alice")


    def sync_test_caller():
        x = my_test_function("Bob")


    asyncio.run(async_test_caller())
    sync_test_caller()
```

```
$ python3 -m timeit -s "def f(): pass" "f()"
5000000 loops, best of 5: 41 nsec per loop
$ python3 -m timeit -s "from asyncio import run" -s "async def cr(): pass" "run(cr())"
5000 loops, best of 5: 69.4 usec per loop

$ python3 -m timeit -s "from asyncio import run, to_thread" -s "def f(): pass" "run(to_thread(f))"
500 loops, best of 5: 650 usec per loop
```
> Note the difference in units: nanoseconds for a regular synchronous function call, microseconds to start an event loop, run a coroutine, and then shut the event loop down again.
> In the other direction, the overhead of using asyncio.to_thread to run synchronous APIs in an async context is lower than that of using asyncio.run in a synchronous context (since the event loop sets up and manages a thread executor that lives as long as the event loop does), but it’s still not negligible (one order of magnitude for a do-nothing function rather than the 3 orders of magnitude we saw with asyncio.run):
