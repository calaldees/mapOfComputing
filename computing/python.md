python3
=======

* [Legally Free Python Books List](https://www.pythonkitchen.com/legally-free-python-books-list/) - Jan 2020
    * Loads of topics - begginer, algorithums, web, bioinformatis, visulisations
* [A Python Book: Beginning Python, AdvancedPython, and Python Exercises](http://www.davekuhlman.org/python_book_01.pdf) Dave Kuhlman 2013
    * [online course version](http://www.davekuhlman.org/python_course_03.html)
* [Beej's Guide to Python Programming For Beginners](https://beej.us/guide/bgpython/)
* [Learn Python for Data Science](https://github.com/blobcity/python-for-data-science) - Basics of python in juyter notebooks

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

* `and`, `or`, `not`, `^` wtf python!
* `0x11`==17 `0b11`==3 `0o11`==9
* `hex()` `bin()` `oct()` to string `f'0b{number:08b}'`

python arrays/lists are janky - it would be nice to use chainable functions
* [funct](https://github.com/Lauriat/funct) enhanced functions for lists

https://book.pythontips.com/en/latest/index.html

* [[styleguide]]
    * [black](https://black.readthedocs.io/)
    * [Google StyleGuide](https://google.github.io/styleguide/pyguide.html)
    * [pep8](https://www.python.org/dev/peps/pep-0008/)

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
    # aa=[1,2,3];bb=aa;aa=[4,5,6];print(aa,bb)

    t = 10 + 1, 20 + 2 ; assert t == 11, 22
    # https://twitter.com/raymondh/status/1318242020461367296

See [[interview]]

```python
def fizzbuzz(i):
    """
    * [FizzBuzz](https://en.wikipedia.org/wiki/Fizz_buzz#Programming_interviews) [_](https://imranontech.com/2007/01/24/using-fizzbuzz-to-find-developers-who-grok-coding/)
        * > Write a program that prints the numbers from 1 to 100. But for multiples of three print “Fizz” instead of the number and for the multiples of five print “Buzz”. For numbers which are multiples of both three and five print “FizzBuzz”.
        * In under 5min (Pro) - in under 10min (A Grade)
        * [Tom Scott commentary and solution](https://www.youtube.com/watch?v=QPZ0pIK_wsc)

    >>> tuple(map(fizzbuzz, range(100)))
    ('fizzbuzz', 1, 2, 'fizz', 4, 'buzz', 'fizz', 7, 8, 'fizz', 'buzz', 11, 'fizz', 13, 14, 'fizzbuzz', 16, 17, 'fizz', 19, 'buzz', 'fizz', 22, 23, 'fizz', 'buzz', 26, 'fizz', 28, 29, 'fizzbuzz', 31, 32, 'fizz', 34, 'buzz', 'fizz', 37, 38, 'fizz', 'buzz', 41, 'fizz', 43, 44, 'fizzbuzz', 46, 47, 'fizz', 49, 'buzz', 'fizz', 52, 53, 'fizz', 'buzz', 56, 'fizz', 58, 59, 'fizzbuzz', 61, 62, 'fizz', 64, 'buzz', 'fizz', 67, 68, 'fizz', 'buzz', 71, 'fizz', 73, 74, 'fizzbuzz', 76, 77, 'fizz', 79, 'buzz', 'fizz', 82, 83, 'fizz', 'buzz', 86, 'fizz', 88, 89, 'fizzbuzz', 91, 92, 'fizz', 94, 'buzz', 'fizz', 97, 98, 'fizz')
    """
    r = ''
    if i % 3 == 0:
        r += 'fizz'
    if i % 5 == 0:
        r += 'buzz'
    if not r:
        r = i
    return r
```


What happens if

```python
dd={'a':1, 'b':2}
for k in dd.keys():
    dd[k]=2
print(dd)


for i in (1,2,3):
    if i == 4:
        break
else:
    


ff = [1,2,3]
gg = [3,4,5]
hh = [5,6,7]
ii = ff
jj = ii
kk = hh

# What is ff, gg, hh, ii, jj, kk?
jj.append(10)

gg.append(11)

kk = gg + gg
kk.append(12)

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
* [__strict__=True](https://instagram-engineering.com/python-at-scale-strict-modules-c0bb9245c834)
    * Experimental flag to prevent mutable state at import time
    * Prevent loads of startup code time

[Overview of python dependency management tools](https://modelpredict.com/python-dependency-management-tools)

* [Practical Python Course](https://github.com/dabeaz-course/practical-python) Creative commons course

https://github.com/SigmaQuan/Better-Python-59-Ways

### Type checking in python

Useful? Or unneeded complexity?
Surely this defeats the purpose of a dynamic language?

* [Python's type checking renaissance](https://dafoster.net/articles/2021/01/26/python%27s-type-checking-renaissance/)


Advanced Modules
----------------

* [Trailtlets](https://github.com/ipython/traitlets) for config

* [toolz](https://toolz.readthedocs.io/en/latest/index.html)
    * Functional, Composable, Lazy tools for python
    * (kind of annoying that these are not part of the standard language)

* [brython](https://brython.info/) - Python3 in the browser instead of javascript
* [Pyodide](https://lwn.net/SubscriberLink/855875/25b1611bb7e4c9a4/) - compile python to [[web-assembly]]

* [Interfaces and Protocols](https://glyph.twistedmatrix.com/2021/03/interfaces-and-protocols.html) in python

Reference Implementation
------------------------

* [Python behind the scenes #4: how Python bytecode is executed](https://tenthousandmeters.com/blog/python-behind-the-scenes-4-how-python-bytecode-is-executed/)


Performance logging - google chrome devtools viewer format? - automatically attach/analyse program

* [python generator "send" function purpose?](https://stackoverflow.com/questions/19302530/python-generator-send-function-purpose)


[//begin]: # "Autogenerated link references for markdown compatibility"
[styleguide]: styleguide.md "StyleGuide"
[interview]: interview.md "Interview Questions"
[web-assembly]: web-assembly.md "WebAssembly"
[//end]: # "Autogenerated link references"