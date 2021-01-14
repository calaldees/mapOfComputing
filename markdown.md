MarkDown
========


What is MarkDown
----------------

* [markdownguide.org](https://www.markdownguide.org/)
* [Markdown CheatSheet](https://devhints.io/markdown)
* [Basic Github Syntax](https://help.github.com/en/github/writing-on-github/basic-writing-and-formatting-syntax)


Why use MarkDown
----------------

Presentation software has been refereed to as _slideware jail_.

> Traditional slideware is hard to proofread, and tweaking text size and alignment on large decks feels like a waste of time.

> ... taking the contents of a single text file (markdown) and turning it into a completely acceptable and usable slide deck.

Quote from [DeckDown](http://deckdown.org/)

Online Document editing tools are also insufficient. We would not have an approval process. This would be damaging once a critical size of collaborators is reached.

We want to create a set of teaching resources that
* Version control
    * Changelog (with rollback)
* Facilitates collaboration
    * Comments
    * Approval process (2 people need to approve)
* Use open industry tooling

We can use Git and Markdown.

If we use MarkDown to describe our content, there are system for exporting to:
* Slideshows
    * HTML
    * Powerpoint
* PDF's
* Books
* A4 Handouts
* Websites
    * [MdMe](https://github.com/susam/mdme)

There are plugins for Markdown to render
* Mathematical symbols
* UML
* Musical notation
* MindMaps (to svg and live web)
    * https://markmap.js.org/
* Video ??
    * [VideoPuppet](https://www.videopuppet.com/docs/script/)


Technologies
------------

* Presentations
    * [MarP: Markdown Presentation Ecosystem](https://marp.app/)
        * [vscode marp](https://marketplace.visualstudio.com/items?itemName=marp-team.marp-vscode)
    * [DeckDown](http://deckdown.org/)
    * [johnloy/markdown-for-slide-decks.md](https://gist.github.com/johnloy/27dd124ad40e210e91c70dd1c24ac8c8)
* Books
    * [bookdown.org](https://bookdown.org/)
        * [bookdown: Authoring Books and Technical Documents with R Markdown](https://bookdown.org/yihui/bookdown/)
        * [blogdown: Creating Websites with R Markdown](https://bookdown.org/yihui/blogdown/)



Specs
-----

* [CommonMark](https://commonmark.org/) - A strongly defined, highly compatible specification of Markdown

Implementations
---------------

[markdown-it](https://markdown-it.github.io/) - javascript renderer with plugins (used by vscode)


### Upcomming?
* [ChartSS.css](https://rbitr.github.io/ChartS.css/) - accessible html/css charts with markdown support


Zettelkasten
------------

* Zettelkasten
    * [Stop Taking Regular Notes; Use a Zettelkasten Instead](https://eugeneyan.com/2020/04/05/note-taking-zettelkasten/)
    * [Zettelkasten note-taking in 10 minutes](https://blog.viktomas.com/posts/slip-box/)
* Knowlege base software (see desktop below)

Editors
-------

* Desktop App
    * [RMarkdown](https://rmarkdown.rstudio.com/) - [Introduction Video](https://player.vimeo.com/video/178485416) 1min
    * [typora](https://typora.io/) - A truly minimal markdown editor
        * [Draw Diagrams With Markdown](https://support.typora.io/Draw-Diagrams-With-Markdown/) - Mermaid and FlowchartJS
    * [qownnotes](https://www.qownnotes.org/) Plain-text file markdown note taking with Nextcloud integration
    * [Obsidian](https://obsidian.md/) is a powerful knowledge base that works on top of a local folder of plain text Markdown files
    * [zettlr](https://www.zettlr.com/) A Markdown editor for the 21st century 
    * [Trilium Notes](https://github.com/zadam/trilium) is a hierarchical note taking application with focus on building large personal knowledge bases
* Browser
    * [Github Markdown Support](https://docs.github.com/en/free-pro-team@latest/github/writing-on-github/basic-writing-and-formatting-syntax)
        * Basic (no diagram plugins)
        * [GitHub Mermaid Support ticket](https://github.community/t/feature-request-support-mermaid-markdown-graph-diagrams-in-md-files/1922/42) 5 years old?
        * [GitHub Chrome Extension for Markdown](https://github.com/BackMarket/github-mermaid-extension)
    * [GitLab Markdown Support](https://docs.gitlab.com/ee/user/markdown.html#diagrams-and-flowcharts)
        * Mermaid
        * PlantUML
        * Maths
    * [HackMD](https://hackmd.io/)
        * [Diagram examples](https://hackmd.io/MathJax-and-UML?both)
        * MathJax
        * Mermaid
        * Flowchart.js
        * ABC
        * Graphviz
        * Missing
            * PlantUML support?
    * [stackedit.io](https://stackedit.io/) - Online editor to sync with GoogleDrive and GitHub
        * Mermaid
        * ABC
* IDE Plugin/Extension
    * vscode
        * [Foam](https://foambubble.github.io/foam/)
            * [Markdown-all-in-one](https://marketplace.visualstudio.com/items?itemName=yzhang.markdown-all-in-one)
                * Keyboard shortcuts
                * Table of content
            * [Markdown Notes](https://marketplace.visualstudio.com/items?itemName=kortina.vscode-markdown-notes)
                * `[[wiki-links]]`
                * Backlinks
                * `#tag` linking
        * [HackMD Extension](https://marketplace.visualstudio.com/items?itemName=HackMD.vscode-hackmd)
            * replaces the builtin preview
            * (See HackMD browser above for list of supported extras)
        * [Markdown Preview Enhanced](https://shd101wyy.github.io/markdown-preview-enhanced/)
            * [extension](https://marketplace.visualstudio.com/items?itemName=shd101wyy.markdown-preview-enhanced)
                * added new preview mode
                * sometimes unstable on large documents?
            * Mermaid
            * flowchart.js
            * Missing
                * GraphViz
                * abc
            * PlantUML
            * Presentation Writer
            * Pandoc (output pdf, word)
            * Code Chunk - render code output into documents
        


Diagram Extensions Examples
---------------------------

* [Mermaid](https://mermaid-js.github.io/mermaid/) - Generation of diagrams and flowcharts from text in a similar manner as markdown
    * [mermaid-live-editor](https://mermaid-js.github.io/mermaid-live-editor/)
    * [vscode markdown support](https://marketplace.visualstudio.com/items?itemName=bierner.markdown-mermaid)

    * ```mermaid
        graph TB

        SubGraph1 --> SubGraph1Flow
        subgraph "SubGraph 1 Flow"
        SubGraph1Flow(SubNode 1)
        SubGraph1Flow -- Choice1 --> DoChoice1
        SubGraph1Flow -- Choice2 --> DoChoice2
        end

        subgraph "Main Graph"
        Node1[Node 1] --> Node2[Node 2]
        Node2 --> SubGraph1[Jump to SubGraph1]
        SubGraph1 --> FinalThing[Final Thing]
        end
      ```
    * ```mermaid
        gantt
            title A Gantt Diagram

            section Section
            A task           :a1, 2014-01-01, 30d
            Another task     :after a1  , 20d
            section Another
            Task in sec      :2014-01-12  , 12d
            anther task      : 24d
      ```
* [PlantUML](https://plantuml.com/)
    * ```plantuml
        Bob -> Alice : hello
        Alice -> Bob : hi
      ```
    * ```plantuml
        start

        if (Graphviz installed?) then (yes)
        :process all diagrams;
        else (no)
        :process only
        __sequence__ and __activity__ diagrams;
        endif

        stop
      ```
* [flowchart.js](http://flowchart.js.org/)
    * ```sequence
        Alice->Bob: Hello Bob, how are you?
        Note right of Bob: Bob thinks
        Bob-->Alice: I am good thanks!
        Note left of Alice: Alice responds
        Alice->Bob: Where have you been?
      ```
    * ```flow
        st=>start: Start
        e=>end: End
        op=>operation: My Operation
        op2=>operation: lalala
        cond=>condition: Yes or No?

        st->op->op2->cond
        cond(yes)->e
        cond(no)->op2
      ```
* [graphviz](https://graphviz.org/)
    * [gallery](https://graphviz.org/gallery/)
    * [Drawing Graphs using Dot and Graphviz](https://www.tonyballantyne.com/graphs.html)
    * [WebGraphViz](http://www.webgraphviz.com/)
    * [create diagrams with code using graphviz](https://ncona.com/2020/06/create-diagrams-with-code-using-graphviz/)
    * ```graphviz
        digraph G {
            main -> parse -> execute;
            main -> init;
            main -> cleanup;
            execute -> make_string;
            execute -> printf
            init -> make_string;
            main -> printf;
            execute -> compare;
        }
      ```
    * ```graphviz
        digraph G {
            node [shape = record,height=.1];
            node0[label = "<f0> |<f1> G|<f2> "];
            node1[label = "<f0> |<f1> E|<f2> "];
            node2[label = "<f0> |<f1> B|<f2> "];
            node3[label = "<f0> |<f1> F|<f2> "];
            node4[label = "<f0> |<f1> R|<f2> "];
            node5[label = "<f0> |<f1> H|<f2> "];
            node6[label = "<f0> |<f1> Y|<f2> "];
            node7[label = "<f0> |<f1> A|<f2> "];
            node8[label = "<f0> |<f1> C|<f2> "];
            "node0":f2 -> "node4":f1;
            "node0":f0 -> "node1":f1;
            "node1":f0 -> "node2":f1;
            "node1":f2 -> "node3":f1;
            "node2":f2 -> "node8":f1;
            "node2":f0 -> "node7":f1;
            "node4":f2 -> "node6":f1;
            "node4":f0 -> "node5":f1;
        }
      ```
    * ```graphviz
        digraph hierarchy {

                nodesep=1.0 // increases the separation between nodes

                node [color=Red,fontname=Courier,shape=box] //All nodes will this shape and colour
                edge [color=Blue, style=dashed] //All the lines look like this

                Headteacher->{Deputy1 Deputy2 BusinessManager}
                Deputy1->{Teacher1 Teacher2}
                BusinessManager->ITManager
                {rank=same;ITManager Teacher1 Teacher2}  // Put them on the same level
        }
      ```
* [abc](http://abcnotation.com/examples) - Musical notation
    * [Abc music notation tutorial](http://www.lesession.co.uk/abc/abc_notation.htm)
    * [abc:standard](http://abcnotation.com/wiki/abc:standard)
*   ```abc
    M:6/8
    L:1/8
    K:G
    V:1 name="Whistle" snm="wh"  
    B3 A3 | G6 | B3 A3 | G6 ||  
    V:2 name="violin" snm="v"  
    BdB AcA | GAG D3 | BdB AcA | GAG D6 ||  
    V:3 name="Bass" snm="b" clef=bass  
    D3 D3 | D6 | D3 D3 | D6 ||
    ```

Other text systems
------------------

* [extension integrates Draw.io into VS Code](https://github.com/hediet/vscode-drawio)
* [Diagram as Code](https://diagrams.mingrammer.com/) Diagrams lets you draw the cloud system architecture in Python code.
* [Create beautiful diagrams just by typing mathematical notation in plain text](https://github.com/penrose/penrose)
* [elk](https://rtsys.informatik.uni-kiel.de/elklive/)


Unsorted
--------

https://github.com/Jam3/math-as-code
https://www.getoutline.com/

[Ask HN: What do you use to keep track of bookmarks/notes/snippets?](https://news.ycombinator.com/item?id=22778123)

[histre](https://histre.com/) Notes on web history

[This page is a truly naked, brutalist html quine](https://secretgeek.github.io/html_wysiwyg/html.html)
[markdown-css](https://mrcoles.com/demo/markdown-css/) - make HTML look like plain text markdown source
[GitHub css in markdown](https://github.com/sindresorhus/css-in-readme-like-wat)
