MarkDown
========

What is MarkDown
----------------

* [markdownguide.org](https://www.markdownguide.org/)
    * [basic-syntax](https://www.markdownguide.org/basic-syntax/)
* Markdown [CheatSheet](https://devhints.io/markdown) [CheatSheet2](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
* [Basic Github Syntax](https://help.github.com/en/github/writing-on-github/basic-writing-and-formatting-syntax)

Alternate Tech
--------------

* [[latex]]

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

We can use [[Git]] and Markdown.

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


* [Semantic Line Breaks](https://sembr.org/)


Technologies
------------

TODO: investigate mkdocs
```bash
pip3 install mkdocs
mkdocs serve
```

* Presentations
    * [Slidev](https://sli.dev/guide/why)
        * Markdown replacement for PPT. Recordings, web export, live preview, modular css
    * [MarP: Markdown Presentation Ecosystem](https://marp.app/)
        * [vscode marp](https://marketplace.visualstudio.com/items?itemName=marp-team.marp-vscode)
    * [DeckDown](http://deckdown.org/)
    * [fusuma](https://hiroppy.github.io/fusuma/) - [github/fusuma](https://github.com/hiroppy/fusuma)
    * [johnloy/markdown-for-slide-decks.md](https://gist.github.com/johnloy/27dd124ad40e210e91c70dd1c24ac8c8)
    * [remarkjs](https://remarkjs.com)
        * [github.com/gnab/remark](https://github.com/gnab/remark)
        * Just pop a JS cdn in html and instant presentation!
        * P == presenter mode
        * `---` for a new slide
    * [presenterm](https://github.com/mfontanini/presenterm)
        *  A markdown terminal slideshow tool 
* Books
    * [bookdown.org](https://bookdown.org/)
        * [bookdown: Authoring Books and Technical Documents with R Markdown](https://bookdown.org/yihui/bookdown/)
        * [blogdown: Creating Websites with R Markdown](https://bookdown.org/yihui/blogdown/)
* Web (blog)
    * Article
        * [Blog with Markdown + Git, and degrade gracefully through time](https://brandur.org/fragments/graceful-degradation-time)
* Science
    * [MyST Markdown Tools](https://mystmd.org/guide)
        * an ecosystem of open-source, community-driven tools designed to revolutionize scientific communication. Our powerful authoring framework supports blogs, online books, scientific papers, reports and journals articles.
* Feeds
    * [MdRss](https://github.com/TimoKats/mdrss)
        * Convert markdown files to RSS feed using GO. 

* [Styling Markdown](https://webdev.bryanhogan.com/miscellaneous/styling-markdown/)

Input
-----
* [Nanonets-OCR](https://huggingface.co/nanonets/Nanonets-OCR-s)
    * OCR Document to Markdown (via LLM). Great for more LLM usage

Specs
-----

* [CommonMark](https://commonmark.org/) - A strongly defined, highly compatible specification of Markdown

Implementations
---------------

* [markdown-it](https://markdown-it.github.io/) - javascript renderer with plugins (used by vscode)


### Upcomming?
* [ChartSS.css](https://rbitr.github.io/ChartS.css/) - accessible html/css charts with markdown support


Knowledge base
--------------

* #Zettelkasten
    * [Stop Taking Regular Notes; Use a Zettelkasten Instead](https://eugeneyan.com/2020/04/05/note-taking-zettelkasten/)
    * [Zettelkasten note-taking in 10 minutes](https://blog.viktomas.com/posts/slip-box/)
    * [Zettelkasten, Linking Your Thinking, and Nick Milo's Search for Ground](https://writing.bobdoto.computer/zettelkasten-linking-your-thinking-and-nick-milos-search-for-ground/)
        *  Linking Your Thinking (LYT) and zettelkasten remain two different ways to achieve similar, but ultimately different goals
        *  Luhmann felt that writing, not his zettelkasten, was the only way to think with any sense of complexity
        *  LYT is a Life Operating System
* software (see desktop below)
* [Using sqlite3 as a notekeeping document graph with automatic reference indexing](https://epilys.github.io/bibliothecula/notekeeping.html)
    * Amazing use of binary data, insert triggers, virtual tables, search indexing, json meta data extraction in queries
* [SuperNotes.app](https://supernotes.app/)
    * > Free Your Thoughts - Supernotes is your new home for ideas, records, tasks, and lists. Enjoy efficient note-taking without the hassle.
    * Online service for Zettelkasten/Markdown stuff
* [How I use Obsidian](https://stephango.com/vault)
    * No folders
    * Internal links
    * Keep dates consistent `YYYY-MM-DD`
* [MDWiki](http://dynalon.github.io/mdwiki/)

Editors
-------

* Desktop App
    * [Marker](https://marker.pages.dev/)
        * > A Secure Visual Markdown Editor That is Fully Yours. Marker is an open-source, user-friendly UI for writing & editing markdown files. Everything you create lives in your filesystem.
    * [RMarkdown](https://rmarkdown.rstudio.com/) - [Introduction Video](https://player.vimeo.com/video/178485416) 1min
    * [typora](https://typora.io/) - A truly minimal markdown editor
        * [Draw Diagrams With Markdown](https://support.typora.io/Draw-Diagrams-With-Markdown/) - Mermaid and FlowchartJS
    * [qownnotes](https://www.qownnotes.org/) Plain-text file markdown note taking with Nextcloud integration
    * [Obsidian](https://obsidian.md/) is a powerful knowledge base that works on top of a local folder of plain text Markdown files
    * [zettlr](https://www.zettlr.com/) A Markdown editor for the 21st century 
    * [Trilium Notes](https://github.com/zadam/trilium) is a hierarchical note taking application with focus on building large personal knowledge bases
    * [MindForger](https://www.mindforger.com/)
* Browser
    * [Github Markdown Support](https://docs.github.com/en/free-pro-team@latest/github/writing-on-github/basic-writing-and-formatting-syntax)
        * Basic (no diagram plugins)
        * Mermaid
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
            * [syntax](https://github.com/shd101wyy/markdown-preview-enhanced/blob/master/docs/markdown-basics.md)
                * Superscript, line number, CriticMarks Admonition
                * `enableExtendedTableSyntax` in extension settings
            * Mermaid
            * flowchart.js
            * Missing
                * GraphViz
                * abc
            * PlantUML
            * Presentation Writer
            * Pandoc (output pdf, word)
            * [wavedrom](https://shd101wyy.github.io/markdown-preview-enhanced/#/diagrams?id=wavedrom) timing diagrams
            * [ditaa](https://shd101wyy.github.io/markdown-preview-enhanced/#/diagrams?id=ditaa) - ascii art flow diagrams
            * Code Chunk - render code output into documents
            * [@import](https://github.com/shd101wyy/markdown-preview-enhanced/blob/master/docs/file-imports.md)
                * ```
                    @import "your_file"
                    @import "test.puml" {code_block=true class="line-numbers"}
                    @import "test.md" {line_begin=2 line_end=10}
                    ```
                * partial line numbers from file
                * can execute commands and include the output
* Custom
    * [Ditching Obsidian and building my own](https://amberwilliams.io/blogs/building-my-own-pkms)
* [mkdocs](https://squidfunk.github.io/mkdocs-material/)
    * > Write your documentation in Markdown and create a professional static site in minutes – searchable, customizable, in 60+ languages, for all devices.
    * This looks so beautiful!

### Admonition
* admonition
    * note, abstract, info, tip, success, question, warning, failure, danger, bug, example, quote
(can add custom ones! see documentation)

https://github.com/shd101wyy/markdown-preview-enhanced/blob/master/docs/markdown-basics.md#admonition
https://squidfunk.github.io/mkdocs-material/reference/admonitions/

!!! warning    This is the admonition title
    This is the admonition body

Github has own flavor of admonition - called 'alerts' (thanks github)
https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#alerts

> [!NOTE]
> Useful information that users should know, even when skimming content.

> [!TIP]
> Helpful advice for doing things better or more easily.

> [!IMPORTANT]
> Key information users need to know to achieve their goal.

> [!WARNING]
> Urgent info that needs immediate user attention to avoid problems.

> [!CAUTION]
> Advises about risks or negative outcomes of certain actions.

Some after space


Flavors
-------

Markdown is reasonably fragmented. There are a range of standards

* GitHub Flavoured Markdown
* GitLab Flavoured Markdown
* CommonMark
    * An attempt to formally describe MarkDown behaviour
* [MDx](https://mdxjs.com/)
    * > MDX allows you to use JSX in your markdown content. You can import components, such as interactive charts or alerts, and embed them within your content. This makes writing long-form content with components


Diagram Extensions Examples
---------------------------

* [Mermaid](https://mermaid-js.github.io/mermaid/) - Generation of diagrams and flowcharts from text in a similar manner as markdown
    * [mermaid-live-editor](https://mermaid-js.github.io/mermaid-live-editor/)
    * [vscode markdown support](https://marketplace.visualstudio.com/items?itemName=bierner.markdown-mermaid)
    * [Mermaid to ASCII](https://github.com/lukilabs/beautiful-mermaid)
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
    * [planter](https://github.com/achiku/planter) - Generate PlantUML ER diagram textual description from PostgreSQL tables 
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
* geo
    * ```geo
        The British Museum
        ```
* [markmap](https://markmap.js.org/)
    * Mind map
* fretboard
    * ```fretboard {title="horizontal, 5 frets", type"h6 noNut"}
        -oO-*-
        --o-o-
        -o-oo-
        -o-oO-
        -oo-o-
        -*O-o-
        ```
* [Markdown Preview Enhanced: Diagrams - examples](https://gist.github.com/blackcater/1701e845a963216541591106c1bb9d3b)
* [vega](https://vega.github.io/vega/examples/) and [vega-lite](https://vega.github.io/vega-lite/examples/)
    * ```vega
            {
                "$schema": "https://vega.github.io/schema/vega-lite/v5.json",
                "description": "A simple bar chart with embedded data.",
                "data": {
                    "values": [
                    {"a": "A", "b": 28}, {"a": "B", "b": 55}, {"a": "C", "b": 43},
                    {"a": "D", "b": 91}, {"a": "E", "b": 81}, {"a": "F", "b": 53},
                    {"a": "G", "b": 19}, {"a": "H", "b": 87}, {"a": "I", "b": 52}
                    ]
                },
                "mark": "bar",
                "encoding": {
                    "x": {"field": "a", "type": "nominal", "axis": {"labelAngle": 0}},
                    "y": {"field": "b", "type": "quantitative"}
                }
            }
        ```
    * ```
        @import "your_vega_source.json" {as="vega"}
        ```
* More
    * [CommonMark Extensions](https://irosyadi.gitbook.io/irosyadi/markdown/library-extended-commonmarks)
        * Vega and [Vega-lite](https://vega.github.io/vega-lite/examples/)
            * Graphs (bar graphs)
        * Railroad
            * Sequence
* [CodiMD Documentation](https://hackmd.io/c/codimd-documentation/%2F%40codimd%2Fextra-supported-syntax#Extra-Supported-Syntax)
* Other features
    * Collapsing content
        * ```
            <details>
                <summary>(expand tutorial css)</summary>
                your collapsed content here
            </details>
          ```
    * Heavy References at bottom to make viewing raw text more readable
        * ```
            [My Link Text][1-refernce]

            [1-reference]: https://example.com/
          ```
    * Comments 
        * https://stackoverflow.com/a/32190021/3356840
        * ```
            (empty line)
            [comment]: # (This actually is the most platform independent comment)
            ```
    * [MUME](https://github.com/shd101wyy/mume) renderer features (used in MarkdownPreviewEnhanced)
        * rendering of code blocks with line numbers and 'partial file' inclusion
            * https://shd101wyy.github.io/markdown-preview-enhanced/#/markdown-basics?id=line-numbers
            * https://shd101wyy.github.io/markdown-preview-enhanced/#/file-imports?id=import-certain-lines
            * These use an underlying Markdown Library called MUME for rendering
            * I need to do more research into how this could be done on the commandline and CI
* [Tenno](https://tenno.app/)
    * 'cell like' spreadsheet cells support in markdown to make graphs.
    * Looks really cool!


Guides
------

* [Web Publications — LaTeX Style](https://goessner.github.io/mdmath/publication.html) - Markdown + Maths

Other text systems
------------------

* [Dumbdown](https://github.com/treenotation/dumbdown) - no brackets or syntax, just words
* [extension integrates Draw.io into VS Code](https://github.com/hediet/vscode-drawio)
* [Diagram as Code](https://diagrams.mingrammer.com/) Diagrams lets you draw the cloud system architecture in Python code.
* [Create beautiful diagrams just by typing mathematical notation in plain text](https://github.com/penrose/penrose)
* [elk](https://rtsys.informatik.uni-kiel.de/elklive/)
* [Beautiful PDFs from HTML](https://pdf.math.dev/)
* OfficeDocs to Markdown (in browser) [Run Python in Your Browser Effortlessly](https://kai.bi/post/run-python-programs-easily-in-the-browser)
    * Also an example of Python+[[web-assembly]]
* [texme](https://github.com/susam/texme) - Self-rendering Markdown + LaTeX documents in browser (from textarea with js)
* [Svgbob Editor](https://ivanceras.github.io/svgbob-editor/)
    * Convert your ascii diagram scribbles into happy little [[svg]]

Unsorted
--------

* [Podlite](https://podlite.org/)
    * Something similar to Markdown?
    * [live](https://pod6.in/)
* [Plain text. With lines.](http://akkartik.name/lines.html) #plaintext
    * markdown with drawing lines in a code block
* [Typograms](https://code.sgo.to/typograms/) (typographic diagrams) 
    * a lightweight image format (text/typograms) useful for defining simple diagrams in technical documentation.
* [MonoDraw](https://monodraw.helftone.com/)
    * Powerful ASCII art editor designed for the Mac. 
https://github.com/Jam3/math-as-code
https://www.getoutline.com/
* [treesheets](http://strlen.com/treesheets/)
    * more structured than a text file - hierarchical
* [Ask HN: What do you use to keep track of bookmarks/notes/snippets?](https://news.ycombinator.com/item?id=22778123)

* [This page is a truly naked, brutalist html quine](https://secretgeek.github.io/html_wysiwyg/html.html)
* [markdown-css](https://mrcoles.com/demo/markdown-css/) - make HTML look like plain text markdown source
* [How to Style Images With Markdown](https://dzone.com/articles/how-to-style-images-with-markdown)



[GitHub css in markdown](https://github.com/sindresorhus/css-in-readme-like-wat)


Alternatives?
--------------

* [excalidraw.com](https://excalidraw.com)
    * Diagrams that look sketched by pencil
* [kroki.io](https://kroki.io/) - Creates diagrams from textual descriptions!
    * Live site for rendering LOADS of text to diagram notation, Vega, Graphviz, PlantUML
* [jendeley](https://akawashiro.github.io/jendeley/) is a JSON-based document organizing software.
    * jendeley is JSON-based. You can see and edit your database quickly.
    * jendeley works locally. Your important database is owned only by you. No cloud.
    * jendeley is browser-based. You can run it anywhere node.js runs.


HTML to Markdown
----------------

* [Reader-LM: Small Language Models for Cleaning and Converting HTML to Markdown](https://jina.ai/news/reader-lm-small-language-models-for-cleaning-and-converting-html-to-markdown/)


[latex]: latex.md "latex"
[Git]: git.md "GIT"
[web-assembly]: web-assembly.md "Web Assembly"
[svg]: svg.md "SVG"

