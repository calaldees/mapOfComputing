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

If we use MarkDown/SVG to describe our content, there are system for exporting to:
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
* Musical notation [abc](http://www.lesession.co.uk/abc/abc_notation.htm)
* MindMaps (to svg and live web)
    * https://markmap.js.org/
* Video ??
    * [VideoPuppet](https://www.videopuppet.com/docs/script/)


Technologies
------------

Below are some examples of possible tech

* [johnloy/markdown-for-slide-decks.md](https://gist.github.com/johnloy/27dd124ad40e210e91c70dd1c24ac8c8)
* [DeckDown](http://deckdown.org/)
* [RMarkdown](https://rmarkdown.rstudio.com/) - [Introduction Video](https://player.vimeo.com/video/178485416) 1min

* [MarP: Markdown Presentation Ecosystem](https://marp.app/)
    * [vscode marp](https://marketplace.visualstudio.com/items?itemName=marp-team.marp-vscode)

* [stackedit.io](https://stackedit.io/) - Online editor to sync with GoogleDrive and GitHub

* [typora](https://typora.io/) A truly minimal markdown editor
    * [Draw Diagrams With Markdown](https://support.typora.io/Draw-Diagrams-With-Markdown/)
* [HackMD](https://hackmd.io/)
    * [vscode extension](https://marketplace.visualstudio.com/items?itemName=HackMD.vscode-hackmd)
    * online, github integration, slides, abc, mermaid
* vscode/atom [Markdown Preview Enhanced](https://shd101wyy.github.io/markdown-preview-enhanced/)
    * Mermaid + other charts
    * TOC
    * Presentations

* [qownnotes](https://www.qownnotes.org/) Plain-text file markdown note taking with Nextcloud integration
* [ChartSS.css](https://rbitr.github.io/ChartS.css/) - accessible html/css charts with markdown support

https://markdown-it.github.io/ renderer with plugins (used by vscode)
https://commonmark.org/ (defined standard)

### Zettelkasten & Knowledge bases

* [Stop Taking Regular Notes; Use a Zettelkasten Instead](https://eugeneyan.com/2020/04/05/note-taking-zettelkasten/)
* [Zettelkasten note-taking in 10 minutes](https://blog.viktomas.com/posts/slip-box/)
* [Obsidian](https://obsidian.md/) is a powerful knowledge base that works on top of a local folder of plain text Markdown files
* [zettlr](https://www.zettlr.com/) A Markdown editor for the 21st century 
* [Trilium Notes](https://github.com/zadam/trilium) is a hierarchical note taking application with focus on building large personal knowledge bases


Diagrams from plain text notation
---------------------------------

* [Mermaid](https://mermaid-js.github.io/mermaid/) - Generation of diagrams and flowcharts from text in a similar manner as markdown.
    * [mermaid-live-editor](https://mermaid-js.github.io/mermaid-live-editor/)
    * [vscode markdown support](https://marketplace.visualstudio.com/items?itemName=bierner.markdown-mermaid)
    * [GitHub Mermaid Support ticket](https://github.community/t/feature-request-support-mermaid-markdown-graph-diagrams-in-md-files/1922/42) 5 years old?
        * GitLab supports this natively
        * [GitHub Chrome Extension](https://github.com/BackMarket/github-mermaid-extension)
    
* [flowchart.js](http://flowchart.js.org/)
* [extension integrates Draw.io into VS Code](https://github.com/hediet/vscode-drawio)
* [Diagram as Code](https://diagrams.mingrammer.com/) Diagrams lets you draw the cloud system architecture in Python code.
* [WebGraphViz](http://www.webgraphviz.com/)
    * [create diagrams with code using graphviz](https://ncona.com/2020/06/create-diagrams-with-code-using-graphviz/)
* [Create beautiful diagrams just by typing mathematical notation in plain text](https://github.com/penrose/penrose)
* [elk](https://rtsys.informatik.uni-kiel.de/elklive/)

* Typora Editor (see above) [Draw Diagrams With Markdown](https://support.typora.io/Draw-Diagrams-With-Markdown/) - Mermaid and FlowchartJS


Unsorted
--------

https://github.com/Jam3/math-as-code
https://www.getoutline.com/

[Ask HN: What do you use to keep track of bookmarks/notes/snippets?](https://news.ycombinator.com/item?id=22778123)

[histre](https://histre.com/) Notes on web history

[This page is a truly naked, brutalist html quine](https://secretgeek.github.io/html_wysiwyg/html.html)
[markdown-css](https://mrcoles.com/demo/markdown-css/) - make HTML look like plain text markdown source
