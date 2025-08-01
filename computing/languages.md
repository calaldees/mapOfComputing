Languages
=========

* [[language-design]]
* [[language-features]]
* [[language-cheatsheets]]
* [[dsl]]
* [[dynamic-programming]]

* [[static-languages]]
* [[dynamic-languages]]

* [[no-code]]


* [Writing that changed how I think about PL](https://bernsteinbear.com/blog/pl-writing/)
    * > Every so often I come across a paper, blog post, or (occasionally) video that completely changes how I think about a topic in programming languages and compilers. For some of these posts, I can’t even remember how I thought about the idea before reading it—it was that impactful.

* [To Learn a New Language, Read Its Standard Library](http://patshaughnessy.net/2021/10/23/to-learn-a-new-language-read-its-standard-library)

* [Wikipedia: List of programming languages by type (Categorical)](https://en.wikipedia.org/wiki/List_of_programming_languages_by_type)
    * [[visual-programming-languages]]
* [Evaluating Programming Languages](https://cs.lmu.edu/~ray/notes/evaluatingprogramminglanguages/)
    * > So, if you ever get into an argument about programming languages, what should you say?
    * Criteria for Evaluation • Popularity • Understanding Evaluation Tradeoffs
* [Energy Usage per language](https://www.researchgate.net/figure/Normalized-global-results-for-Energy-Time-and-Memory_tbl2_320436353)
* [rosettacode.org](http://rosettacode.org)
    * Rosetta Code is a programming chrestomathy site. The idea is to present solutions to the same task in as many different languages as possible, to demonstrate how languages are similar and different, and to aid a person with a grounding in one approach to a problem in learning another.

* [Little Languages](https://chreke.com/little-languages.html)
    * (well referenced)
    * we just keep building bigger tools that rely on bigger tools (like building the pyramids)
    * We should consider simpler DSL mini languages for sub-problems (Regex, SQL). But how do we link these together?

* [Honeypot](https://www.youtube.com/channel/UCsUalyRg43M8D60mtHe6YcA) YouTube Channel
    * YouTube documentaries for languages and frameworks

* [4 Programming Paradigms In 40 Minutes](https://www.youtube.com/watch?v=cgVVZMfLjEI) Coding Tech 40min RubyConf 2017 Aja Hammerly
    * Object oriented (example in Ruby)
    * Functional (example in Racket)
    * Logical (example in [[prolog]])
        * Describe _what_ not _how_
        * Variables/Constants, Facts, Rules (specify relationships between facts)
        * _ancestors_ example
        * programs can run backwards and forwards finding missing value
    * Procedural (example in Assembler)
        * two register A and D
        * no multiplication, devision
        * constants go to A
        * Jump if eq, lt, gt

* [Seven Languages in Seven Weeks - A Pragmatic Guide to Learning Programming Languages](https://pragprog.com/titles/btlang/seven-languages-in-seven-weeks/) 2010 by Bruce A. Tate
    * ISBN 9781934356593
    * Ruby, IO, Prolog, Scala, Clojure, Haskell
* [Exercises in Programming Style](https://www.routledge.com/Exercises-in-Programming-Style/Lopes/p/book/9780367350208) 2020 Cristina (Crista) Lopes
    * ISBN 9780367350208
    * Part 1 Historical
    * Part 2 Basic Styles
    * Part 3 Function Composition
    * Part 4 Objects and Object Interaction
    * Part 5 Reflection and Metaprogramming
    * Part 6 Adversity
    * Part 7 Data-Centric
    * Part 8 Concurrency
    * Part 9 Interactivity
    * Part 10 Neural Networks

* [[assembly]]
* [[c]]
* [[c++]]
* [[nim]]
* [[rust]]
* [[fstar]]
* [[golang]]
* [[javascript]] ECMAScript
* [[logo]]
* [[python]]
* [[prolog]]
* [[ruby]]
* [[qbasic]]
* [[shaders]]
* [[web-assembly]]
* [[lisp]]
* [[erlang]]
* [[elm]]
* #ClojureScript
* Ember
    * [Ember Documentary](https://www.youtube.com/watch?v=Cvz-9ccflKQ) 27min
* [Squeak/Smalltalk](https://squeak.org/)
    * [6.0](https://raw.githubusercontent.com/squeak-smalltalk/squeak-app/squeak-trunk/release-notes/6.0) 2022
* [blocky](https://blockly-demo.appspot.com/static/demos/index.html)
* [BluePrints UE4](https://docs.unrealengine.com/4.26/en-US/ProgrammingAndScripting/Blueprints/)
    * [blueprintue.com](https://blueprintue.com/)
    * [Blueprints as a programming language](https://boxbase.org/entries/2019/jan/20/blueprints/)
* [Verse](https://dev.epicgames.com/documentation/en-us/uefn/verse-language-reference)
    * Super interesting! Tim Sweeny! Large distributed, functional
* Self
    * [Programming as an Experience: The Inspiration for Self](https://link.springer.com/chapter/10.1007/3-540-49538-X_15)
    * Smalltalk extreeem
* scala
    * [hands on scala](https://www.handsonscala.com/)
* [[logo]]
* C# #csharp
    * [C# 10 new feature CallerArgumentExpression, argument check and more](https://weblogs.asp.net/dixin/csharp-10-new-feature-callerargumentexpression-argument-check-and-more)
        * New feature .. read .. 
* pascal
    * [Castel Game Engine](https://castle-engine.io/why_pascal) Written in Pascal!? [[game-engines]]
* https://www.hylo-lang.org/
    * Hylo (formely Val) is a programming language that leverages mutable value semantics and generic programming for high-level systems programming.
* [html-lang](https://html-lang.org/)
    * Some crazy person used html to make a language with a js executor
    * Could be interesting as a learning exercise as the dom is the abstract syntax tree?

* [[language-cheatsheets]]
* [[formal-specification]]




* [alice](https://www.alice.org/)


* [Here’s what people in tech had to say about JavaScript when it debuted in 1995](https://medium.com/dailyjs/heres-what-people-in-tech-had-to-say-about-javascript-when-it-debuted-in-1995-a4b81dc05b71)
* [PYPL PopularitY of Programming Language](http://pypl.github.io/PYPL.html)
* [The Top Programming Languages 2023: Python and SQL are on top, but old languages shouldn’t be forgotten](https://spectrum.ieee.org/the-top-programming-languages-2023) 29 Aug 2023 Stephen Cass

Static languages
----------------

* [Typing is Hard](https://3fx.ch/typing-is-hard.html)
    * Static typing description in a variety of languages


Systems level languages
-----------------------

* [The case for a modern language (part 1)](https://jeang3nie.codeberg.page/case-for-modern-language-pt1/)
    * C is less than perfect
    * > as with many things #BSD even when thay do something that is obviously better than Linux it just never really gets adopted there
    * > the fact that `libc` looks and feels very much like it was hacked together by a bunch of random dudes over the course of a few decades rather than being designed. Which is, of course, exactly what happened. 
    * > I have some other complaints about C that revolve around the lack of any kind of official error handling strategy, the issue of null in general, etc 
    * > but what it really comes down to is that if we keep the language we should at the very least modernize `libc` and standardize the other tooling around the language somewhat.

* C
* Rust
* Nim
* Zig



Learn Online
------------

* [Codewars](https://www.codewars.com/) - Browser based challenges
* [freecodecamp](https://www.freecodecamp.org/)
    * JavaScript challenges in browser
    * (other langauges with multiple choice and videos)
* [Khan Academy](https://www.khanacademy.org/)
    * Whole computing course
    * JS in browser



Other Languages
===============

* [On repl-driven programming](http://mikelevins.github.io/posts/2020-12-18-repl-driven/)
    * Common Lisp and Smalltalk are repl languages
        * Other languages have something similar
    * repl: read-eval-print loop


* [Microsoft power-fx](https://github.com/microsoft/power-fx)

Other Language Domains
----------------------

* [Catala: A Programming Language for the Law](https://arxiv.org/abs/2103.03198)
* 

smalltalk
---------
Live coding in browser (?)
* [caffeine.js.org](https://caffeine.js.org/)
    * > Caffeine is a livecoding environment for web browsers, Node.js, and WebAssembly. After adding it to a webpage, you can use it to make live persistent changes to that page and other pages running Caffeine, without reloading.



Esoteric
--------

* [A Brief Introduction to Esoteric Languages](https://www.hillelwayne.com/talks/esolangs/)
    * Brainfuck (turing complete - obtuse)
    * Piet (executable image)
* [orca](http://100r.co/site/orca.html)
    * designed to create procedural sequencers in which each letter of the alphabet is an operation, where lowercase letters operate on bang, uppercase letters operate each frame.
    * The application is not a synthesiser, but a flexible livecoding environment capable of sending MIDI, OSC & UDP to your audio interface, like Ableton, Renoise, VCV Rack or SuperCollider.
* [J](https://www.jsoftware.com/help/jforc/loopless_code_i_verbs_have_r.htm)
    * Loopless code
* [Ballerina](https://www.infoq.com/articles/ballerina-data-oriented-language/): a Data-Oriented Programming Language

Number systems
--------------

Python has "abstract" number system

Java, Golang, C are all based on x86
Overflow
Modulo operator does not support negative

Javascript (which should be abstract, but was heavily designed in an era of systems performance requirements) uses x86 modulo operator (which does not work with negative numbers)


Performance
------------

* [Modern Python performance considerations](https://lwn.net/SubscriberLink/893686/8978976335696804/) [[performance-profileing]] [[dynamic-programming]] [[python]]
    * Why is python slow?
* [[optimisations]] look at fizzbuzz drag racing


[//begin]: # "Autogenerated link references for markdown compatibility"
[language-design]: language-design.md "Language Design"
[language-features]: language-features.md "Language Features"
[language-cheatsheets]: language-cheatsheets.md "Language Cheatsheets"
[dsl]: dsl.md "Domain Specific Languages (DSL)"
[dynamic-programming]: dynamic-programming.md "Dynamic Programming"
[static-languages]: static-languages.md "Static Languages"
[dynamic-languages]: dynamic-languages.md "Dynamic Languages"
[no-code]: no-code.md "NoCode"
[visual-programming-languages]: visual-programming-languages.md "Visual Programming Languages"
[prolog]: prolog.md "Prolog"
[assembly]: assembly.md "Assembly Code"
[c]: c.md "C"
[c++]: c%2B%2B.md "c++"
[nim]: nim.md "NIM"
[rust]: rust.md "Rust"
[fstar]: fstar.md "F*"
[golang]: golang.md "Golang"
[javascript]: javascript.md "javascript (ECMAScript)"
[logo]: logo.md "Logo"
[python]: python.md "python3"
[ruby]: ruby.md "Ruby"
[qbasic]: qbasic.md "qbasic"
[shaders]: shaders.md "Shaders"
[web-assembly]: web-assembly.md "Web Assembly"
[lisp]: lisp.md "LISP"
[erlang]: erlang.md "Erlang"
[elm]: elm.md "Elm"
[game-engines]: game-engines.md "game-engines"
[formal-specification]: formal-specification.md "Formal Specification"
[performance-profileing]: performance-profileing.md "Performance Profiling"
[optimisations]: optimisations.md "Optimisations"
[//end]: # "Autogenerated link references"