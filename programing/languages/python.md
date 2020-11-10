python3
=======

[Learn Python for Data Science](https://github.com/blobcity/python-for-data-science) - Basics of python in juyter notebooks

The confusing brackets
* []
    * create lists pre-populated
    * list comprehensions (loops)
    * selecting (slicing)
    * selecting from dicts!
* ()
    * create tuples pre-populated
        * ('',) single element!
        * or (''), !
    * generators!
    * Logical grouping
        * multiline
* {}
    * create dicts
    * dict comprehensions
    * sets !
        * not interoperable with dicts?
    * set comprehensions !
* <>
    * no used?


https://book.pythontips.com/en/latest/index.html


[black](https://black.readthedocs.io/)
[Google StyleGuide](https://google.github.io/styleguide/pyguide.html)
[pep8](https://www.python.org/dev/peps/pep-0008/)

[Google DocString Guide](https://sphinxcontrib-napoleon.readthedocs.io/en/latest/example_google.html)
[sphinx docstring format](https://thomas-cokelaer.info/tutorials/sphinx/docstring_python.html#template.MainClass1.function1)


See lanaguageEdgeCases
https://github.com/satwikkansal/wtfpython


Professional Interview Screening

what is PEP8 -> style guide
what is a decorator -> function wrapper
what is the difference between list & tuple -> mutability

```python
    >>> aa=(x+1 for x in range(3)) ; print(tuple(aa), tuple(aa))
    ((1, 2, 3), ())
    # Q: Why? - A: The generator is exhausted

    >>> aa=[1,2,3] ; bb=aa ; aa[:]=[4,5,6] ; print(aa, bb)
    ([4, 5, 6], [4, 5, 6])
    # Q: Why? - A: aa an bb reference the same list

    >>> dd = {i for i in (1,2,2,3)} ; dd &= {2,3,4} ; print(dd)
    set([2, 3])
    # Q: Why? - A: sets have no duplicates `&=` is union_in-place modification
```
    #aa=[1,2,3];bb=aa;aa=[4,5,6];print(aa,bb)

    t = 10 + 1, 20 + 2 ; assert t == 11, 22
    # https://twitter.com/raymondh/status/1318242020461367296

[see interviewquetions.md]
https://imranontech.com/2007/01/24/using-fizzbuzz-to-find-developers-who-grok-coding/
https://www.youtube.com/watch?v=QPZ0pIK_wsc
FizzBuzz

```python
for i in range(100):
    r = ''
    if i % 3 == 0:
        r += 'fizz'
    if i % 5 == 0:
        r += 'buzz'
    if not r:
        r = i
    print(r)
```


```python
dd={'a':1, 'b':2}
for k in dd.keys():
    dd[k]=2
print(dd)


for i in (1,2,3):
    if i == 4:
        break
else:
    

```

```python
from itertools import chain, cycle, permutations
from functools partial, lru_cache, reduce, wraps
from collections import defaultdict, namedtuple, ChainMap, deque
```

* [Hypermodern Python](https://cjolowicz.github.io/posts/hypermodern-python-01-setup/)
    * pyenv
    * poetry
    * click

[Overview of python dependency management tools](https://modelpredict.com/python-dependency-management-tools)

* [Practical Python Course](https://github.com/dabeaz-course/practical-python) Creative commons course

https://github.com/SigmaQuan/Better-Python-59-Ways

Advanced Modules
----------------

* [Trailtlets](https://github.com/ipython/traitlets) for config



* [brython](https://brython.info/) - Python3 in the browser instead of javascript

Reference Implementation
------------------------

* [Python behind the scenes #4: how Python bytecode is executed](https://tenthousandmeters.com/blog/python-behind-the-scenes-4-how-python-bytecode-is-executed/)
