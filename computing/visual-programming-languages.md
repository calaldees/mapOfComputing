Visual Programming Languages
============================

* ["structural editor" rather than a "text editor"](https://crowdhailer.me/2025-01-02/the-evolution-of-a-structural-code-editor/)
    * No syntax errors. Zero time is spent on missing quotes, semi-colons or other details.
    * Better type information. Because the program is always in a valid state the type checker can always run and give meaningful feedback.
    * No keywords Variables can be called var and functions called fn. Either can also be called 🧪 or !_// though maybe they shouldn’t be.
    * Rich visualisations A program can be shown as box and wires, or boolean logic operators. On a smaller scale a record of latitude and longitude can be shown on a map.
    * Reduced complexity

* [Principles of Educational Programming Language Design](https://infedu.vu.lt/journal/INFEDU/article/797/info)  Michael Kölling   2024
    * > why is this still an area of fundamental disagreement among educators?
    * > discuss the relative benefits of pedagogical languages vs. industry languages and articulate why every generation of learners needs their own language.
    * [hacker news comments](https://news.ycombinator.com/item?id=42427428)
        * > a lot of pushback about the article - we simply dont know how to teach programming
        * > I find the core position of the author unconvincing - that is, the author advocates for non-professional languages for beginners, instead using languages designed specifically for teaching. The main argument put forward in favor of professional languages is crossover: if a student learns a language in class, they may be able to use that language professionally. The author then argues against that main point.
        * > I think students should be taught in "professional" languages, but crossover is not my main reason. Rather, it's that professional languages have an enormous corpus of examples that students can look up. If a student is learning on a teaching language without much adoption, there's just not much else a student can do but use the materials that part of the course. Teaching languages don't let students expand their universe of examples.
        * > I agree with the author's point about real insight coming on learning the second (and third, etc.) language and systems. But I don't find it as a compelling point in favor of teaching languages - quite the opposite. To me it means there's no need to obsess over first languages.

* [PyFlow](https://wonderworks-software.github.io/PyFlow/)
    * Like blueprints, but for python

* [Learnable Programming](http://worrydream.com/#!/LearnableProgramming) - Designing a programming system for understanding programs
    * http://worrydream.com/LearnableProgramming/

* [Rethinking Visual Programming with Go](https://divan.dev/posts/visual_programming_go/) #golang [[golang]]
    * Great description of conventional code editing is "caveman in a dark cave with a tourch" analogy
    * great eye tracking gif of reading code (not linear)
    * > But there is no truly mainstream general purpose Visual Programming Language at the moment. By every single metric, modern programming languages landscape is 100% dominated by textual programming languages with zero exceptions.
    * [Programming_language_theory](https://en.wikipedia.org/wiki/Programming_language_theory)
    * > Vision, for example, mostly deals with spatial information - you have to get all input “at once” – you can’t see the image looking it one pixel at a time
    * > Hearing, on the other hand, works predominantly with temporal patterns - you can’t listen to a melody by listening all notes together at the same time.
    * > And that is exactly where both visual and textual representations of code are often missing the point. They attempt to express both, spatial and temporal, components in a similar fashion, and it just adds a cognitive load and doesn’t help at all.
    * > Encoding spatial component visually makes absolutely perfect sense – it’s the most natural way to encode it, 
      > but the temporal component is still better expressed with text - not perfect, but a still unbeatable

* [Developers spend most of their time figuring the system out](https://lepiter.io/feenk/developers-spend-most-of-their-time-figuri-9q25taswlbzjc5rsufndeu0py/)
    * [[software-engineering-skills]]
    * [Glamorous Toolkit](https://gtoolkit.com/)
        * is a multi-language notebook. A fancy code editor. A software analysis platform. A visualization engine. A knowledge management system. All programmable. Free and open-source. 


* [VPL: Visual Programming Language](https://en.wikipedia.org/wiki/Visual_programming_language)

* [Hacker News folk wisdom on visual programming](https://drossbucket.com/2021/06/30/hacker-news-folk-wisdom-on-visual-programming/)
    * Comments and commentary

* [Learnable Programming](http://worrydream.com/#!/LearnableProgramming) Bret Victor / September 2012
    * Designing a programming system for understanding programs

* [Why Programming is Hard to Fundamentally Improve](https://aidancunniffe.com/why-programming-is-hard-to-fundamentally-improve-4101612d4ad9)
    * > I think most of the stalled innovations in programming focused disproportionally on learnability. 
      > The problem is, within a few weeks of using any paradigm developers usually have built a repository of habits that keep them from making mistakes. For instance, if a new visual logic builder prides itself on preventing all syntax errors, that’s really cool, but most developers have learned to do that automatically.


* [Fabrik](https://web.archive.org/web/20070927190552/http://users.ipa.net/~dwighth/smalltalk/Fabrik/Fabrik.html) - A Visual Programming Environment 1988

* [Joy.js](https://ncase.me/joy/)
    * visually see the steps take place
        * Music
        * Turtle
        * Graph/equations


* [viscuit](https://www.viscuit.com/) JP
    * [How Can Children Express Their Intentions Through Coding?: Analysis of Viscuit Programs in Kindergarten](https://dl.acm.org/doi/10.1145/3304221.3325558)
        * > you can move and change multiple pictures on the screen using eyeglasses, which make a sequence from left to right, following from-to (picture rewriting) rules. Its distinguishing feature is that the program is expressed solely with pictures and their layouts. No letters are necessary at all. Therefore, Viscuit is perfectly suitable for pre-school children. 

* [PyFlow](https://github.com/Bycelium/PyFlow) #python 
    * An open-source tool for visual and modular block programing in python 

* [λ-2D](https://www.media.mit.edu/projects/2d-an-exploration-of-drawing-as-programming-language-featuring-ideas-from-lambda-calculus/overview/)
    * An Exploration of Drawing as Programming Language, Featuring Ideas from Lambda Calculus
    * Experimental visual gates for param and arguments - can also see the program run



copied from teacherEducation
----------------

Visual Programming
==================

See more at https://github.com/calaldees/mapOfComputing/blob/main/computing/visual-programming-languages.md
* [Strype](https://strype.org/): a frame-based approach to Python
    * Help transition from blocks to text
    * >  A free Python editor that combines the strengths of blocks and text programming into frame-based editing: write Python code in your browser with structured support.

* [](https://www.cambridge.org/core/books/cambridge-handbook-of-computing-education-research/pedagogic-approaches/6B64002A4E73841A01F32EB1C17E7DE6)
    * > Another recent development is Guo’s (Reference Guo2013) web-based Python simulation and visualization environment that allows learners to move backward and forward through an execution, visualizing stack frames and variables, heap object contents, and memory. While earlier work has long provided similar technical support for this degree of program simulation and visualization (Findler et al, Reference Findler, Clements, Flanagan, Flatt, Krishnamurthi, Steckler and Felleisen2002), an interesting aspect of this tool is the ability to generate a URL for a specific point in the execution visualization, which can be shared among learners to aid collaboration and discussion.

* [VPL: Visual Programming Language](https://en.wikipedia.org/wiki/Visual_programming_language)
* [Hacker News folk wisdom on visual programming](https://drossbucket.com/2021/06/30/hacker-news-folk-wisdom-on-visual-programming/) 2021
    * Superb and in depth review of all the visual programming constructs
* [Learnable Programming](http://worrydream.com/#!/LearnableProgramming) - Designing a programming system for understanding programs

* [Exploring programming misconceptions: an analysis of student mistakes in visual program simulation exercises](https://dl.acm.org/doi/10.1145/2401796.2401799)
    * [uuhistle](http://www.uuhistle.org/) No longer developed
    * [kelmu](https://github.com/Aalto-LeTech/kelmu)
        * [Jsvee & Kelmu: Creating and Tailoring Program Animations for Computing Education ](https://www.youtube.com/watch?v=Q3T_QLRWb78) 5min
            * Python average function animation - really cool!

* [Joy.js](https://ncase.me/joy/)
    * a pedagogic tool?
    * cross curricular? could you approach a science, maths or music teachers? would they be interested?

* [xod.io](https://xod.io/) (Arduino)
    * A visual programming language for microcontrollers



[//begin]: # "Autogenerated link references for markdown compatibility"
[golang]: golang.md "Golang"
[software-engineering-skills]: software-engineering-skills.md "Software Engineer Skills"
[//end]: # "Autogenerated link references"