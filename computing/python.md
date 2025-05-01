python3
=======

* Side quest [[python-typing]]

* [python-cheatsheet](https://gto76.github.io/python-cheatsheet/) - best one I've seen
* [Legally Free Python Books List](https://www.pythonkitchen.com/legally-free-python-books-list/) - Jan 2020
    * Loads of topics - begginer, algorithums, web, bioinformatis, visulisations
* [A Python Book: Beginning Python, AdvancedPython, and Python Exercises](http://www.davekuhlman.org/python_book_01.pdf) Dave Kuhlman 2013
    * [online course version](http://www.davekuhlman.org/python_course_03.html)
* [Beej's Guide to Python Programming For Beginners](https://beej.us/guide/bgpython/)
* [Learn Python for Data Science](https://github.com/blobcity/python-for-data-science) - Basics of python in juyter notebooks
* [What’s in which Python](https://nedbatchelder.com/text/which-py.html)
    * Features of python by version

* [This is valid Python syntax](https://www.bitecode.dev/p/this-is-valid-python-syntax)
    * obfuscated python nonsense

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


See [[dynamic-languages]] for a great breakdown of compiler for `dict()` and `{}`

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

I asked ChatGPT on 24/04/2023 these interview screening questions

I have a set of questions I use to screen professional python programmers before inviting them to a job interview.
I have listed three mini programs and their output. I ask candidates to describe why each program creates these outputs.
Can you explain why these python snippets produce the outputs they do?

    >>> aa=(x+1 for x in range(3)) ; print(tuple(aa), tuple(aa))
    ((1, 2, 3), ())

    >>> aa=[1,2,3] ; bb=aa ; aa[:]=[4,5,6] ; print(aa, bb)
    ([4, 5, 6], [4, 5, 6])

    >>> dd = {i for i in (1,2,2,3)} ; dd &= {2,3,4} ; print(dd)
    set([2, 3])

Sure, I'd be happy to explain these snippets!

1. `aa=(x+1 for x in range(3)) ; print(tuple(aa), tuple(aa))`

In this code, a generator expression is created with `(x+1 for x in range(3))` and assigned to the variable `aa`. A generator is a special type of iterable that allows you to iterate over its elements one at a time. 

Then, `tuple(aa)` is called twice: the first time, it creates a tuple with the first three values of the generator (1, 2, 3) and prints it. The second time, `tuple(aa)` creates an empty tuple because all the values in the generator have already been exhausted by the previous `tuple(aa)` call. 

So the output of this program is `((1, 2, 3), ())`.

2. `aa=[1,2,3] ; bb=aa ; aa[:]=[4,5,6] ; print(aa, bb)`

This code creates a list `aa` containing the values 1, 2, and 3, and then assigns `aa` to the variable `bb`. The third line is where the interesting stuff happens: `aa[:]=[4,5,6]`. This is a slice assignment, which means it replaces the entire contents of `aa` with the new list `[4,5,6]`. Since `bb` is just a reference to the same list object as `aa`, it also gets updated with the new values.

So the output of this program is `([4, 5, 6], [4, 5, 6])`.

3. `dd = {i for i in (1,2,2,3)} ; dd &= {2,3,4} ; print(dd)`

In this code, a set comprehension is used to create a new set `dd` containing the unique values from the tuple `(1,2,2,3)`. Since sets can only contain unique values, this set contains the values 1, 2, and 3. 

Then, `dd &= {2,3,4}` performs an in-place intersection of `dd` with the set `{2,3,4}`. This means that any elements in `dd` that are not also in `{2,3,4}` are removed, leaving only the values 2 and 3.

So the output of this program is `set([2, 3])`.

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

* [Understanding all of Python, through its builtins](https://sadh.life/post/builtins/)
    * using a terminal to dynamically investigate python

* [Hypermodern Python](https://cjolowicz.github.io/posts/hypermodern-python-01-setup/)
    * pyenv
    * poetry
    * click
* [__strict__=True](https://instagram-engineering.com/python-at-scale-strict-modules-c0bb9245c834)
    * Experimental flag to prevent mutable state at import time
    * Prevent loads of startup code time

* [Overview of python dependency management tools](https://modelpredict.com/python-dependency-management-tools)
* IBM [import-tracker](https://github.com/IBM/import-tracker)
    * Python utility for tracking third party dependencies within a library 
    * Dependencies of dependencies

* [Practical Python Course](https://github.com/dabeaz-course/practical-python) Creative commons course

https://github.com/SigmaQuan/Better-Python-59-Ways

### Type checking in python

Useful? Or unneeded complexity?
Surely this defeats the purpose of a dynamic language?

* [Python's type checking renaissance](https://dafoster.net/articles/2021/01/26/python%27s-type-checking-renaissance/)
* [Python’s “Type Hints” are a bit of a disappointment to me](https://www.uninformativ.de/blog/postings/2022-04-21/0/POSTING-en.html)
* [json2pyi](https://json2pyi.pages.dev/)
    * web service to take json and suggest python typeddicts
* pydantic
    * has some wholes - mypy and pydantic don't quite see eye to eye
* [msgspec](https://jcristharif.com/msgspec/)
    * msgspec is a fast serialization and validation library, with builtin support for JSON, MessagePack, YAML, and TOML. It features:
    * 🚀 High performance encoders/decoders for common protocols. The JSON and MessagePack implementations regularly benchmark as the fastest options for Python.
    * 🎉 Support for a wide variety of Python types. Additional types may be supported through extensions.
    * 🔍 Zero-cost schema validation using familiar Python type annotations. In benchmarks msgspec decodes and validates JSON faster than orjson can decode it alone.
    * ✨ A speedy Struct type for representing structured data. If you already use dataclasses or attrs, Structs should feel familiar. However, they’re 5-60x faster for common operations.


Advanced Modules
----------------

* [Trailtlets](https://github.com/ipython/traitlets) for config

* [toolz](https://toolz.readthedocs.io/en/latest/index.html)
    * Functional, Composable, Lazy tools for python
    * (kind of annoying that these are not part of the standard language)

* [Pyodide](https://lwn.net/SubscriberLink/855875/25b1611bb7e4c9a4/) - compile python to [[web-assembly]]

* [Interfaces and Protocols](https://glyph.twistedmatrix.com/2021/03/interfaces-and-protocols.html) in python

* [dis](https://docs.python.org/3/library/dis.html) - Disassembler for Python bytecode
    * Look under the hood of a python function

* python nativly in browser with [[web-assembly]]
    * brython
    * pyscript

Techniques
----------

* [Functools - The Power of Higher-Order Functions in Python](https://martinheinz.dev/blog/52)
    * Really nice description of functools
* [Python Program to Merge Dictionaries (with Examples)](https://favtutor.com/blogs/merge-dictionaries-python)
* [json.AttrDict](https://docs.python.org/3.12/library/json.html#json.AttrDict)
    * orbital_period['earth']
    * orbital_period.earth

Reference Implementation
------------------------

* [Python behind the scenes #4: how Python bytecode is executed](https://tenthousandmeters.com/blog/python-behind-the-scenes-4-how-python-bytecode-is-executed/)


Performance logging - google chrome devtools viewer format? - automatically attach/analyse program

* [python generator "send" function purpose?](https://stackoverflow.com/questions/19302530/python-generator-send-function-purpose)

Elegant Example
---------------

* [Raymond Hettinger](https://twitter.com/raymondh/status/1511489127279206404) @raymondh
```python
def predict(unlabeled_point, points, labels, *, k=5):
  "K nearest neighbors classifier"
  knn = set(nsmallest(k, points, key=partial(dist, unlabeled_point)))
  lnn = [label for label, point in zip(labels, points) if point in knn]
  return mode(lnn)
```
> I like it because the powerful lego building blocks (set, nsmallest, partial, dist, zip, and mode) fit together so nicely to express a machine learning algorithm economically and (to my eyes) clearly.

Features
--------

* [python-syntax-errors](https://github.com/jwilk/python-syntax-errors) - This is a collection of no-op statements that are syntactically valid only since Python X.Y, for most X.Y ≥ 2.4.
    * `0_0  # Python >= 3.6 is required`

### Structural Pattern Matching

* [Structural pattern matching in Python 3.10](https://benhoyt.com/writings/python-pattern-matching/)
    * Example of
        * Text Adventure Game input
        * Binary and Unary operators for calculator
        * JSON HTTP match

Compiled Python?
----------------

Compile LLVM Python
https://github.com/exaloop/codon
Includes GPU processing!

Concurrency
-----------

* Global Interpreter Lock (GIL)
* https://www.infoworld.com/article/3704248/python-moves-to-remove-the-gil-and-boost-concurrency.html


GUI
---

Python has built in TK.
* [pywebview](https://pywebview.flowrl.com/blog/pywebview5.html)
    * python #electron bundler - can even bundle for android
    * > jQuery like DOM manipulation, traversal and event handling straight from Python.

Embedded in other software
--------------------------

* [[python-excel]]


Package Manager
===============

* [[package-manager]]

`pip` is showing it's problems. `poetry` came in to save th day but seems to have limited take-up. We still have problems where two dependencies want different versions of a library.

* [Multiversion Python Thoughts](https://lucumr.pocoo.org/2024/9/9/multiversion-python/)

* [The Fiefdom of Files: PyPi](https://fi-le.net/pypi/)
    * Visualization of python packages and grouped by relatedness

Tools
-----

* [tach](https://github.com/gauge-sh/tach)
    * > A Python tool to visualize + enforce dependencies, using modular architecture 🌎 Open source 🐍 Installable via pip 🔧 Able to be adopted incrementally - ⚡ Implemented with no runtime impact ♾️ Interoperable with your existing systems 🦀 Written in rust

[//begin]: # "Autogenerated link references for markdown compatibility"
[python-typing]: python-typing.md "Python Typing"
[styleguide]: styleguide.md "StyleGuide"
[dynamic-languages]: dynamic-languages.md "Dynamic Languages"
[interview]: interview.md "Interview Questions"
[web-assembly]: web-assembly.md "Web Assembly"
[python-excel]: python-excel.md "Python in Excel"
[package-manager]: package-manager.md "Package Manager"
[//end]: # "Autogenerated link references"