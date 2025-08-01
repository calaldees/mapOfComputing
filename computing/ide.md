Integrated Development Environment (IDE)
========================================

* Visual Studio Code
    * [vscodium](https://vscodium.com/) MIT open without telemetry
* Atom
* IntelliJ
* Eclipse
* Visual Studio 2019
* Notpad++
* emacs
* vim
    * Macros are records of operations/keypress's. Every interaction can be scripted
        * Some madlad created 'Bad Apple' in just vim queries [v](https://eieio.games/blog/bad-apple-with-regex-in-vim/)
* PyCharm

* [[history-of-ide]]

* [Ask HN: How do you sync your computer’s development configurations/environment?](https://news.ycombinator.com/item?id=31517668)
    * Stick/learn the defaults where possible

vscode
https://code.visualstudio.com/docs/getstarted/tips-and-tricks


* [VS Code inserting '.' when adding two spaces after a word #9](https://github.com/AdamMaras/vscode-overtype/issues/9)
    * Settings -> Keyboard -> TextInput(InputSources) Edit -> Hidden menu of shit
    * Turn off keyboard "Smart Quotes" and "Add period with double space"



Show whitespace

Hotkeys
-------

Stick/learn the defaults where possible

tab
shift + tab

ctrl + click (goto)  (TODO: key?)
history
crtl + -
crtl + shift + -

alt + up/down (move lines)

ctrl + l (select line)

MultiCursor Editing
vscode multicursor rename
    (ctrl/cmd) + shift + L   or  (crtl/cmd) + f2
alt + click (add cursor)
Add cursor vertical up/down: ctrl/cmd + alt + up/down

esc (back to single)

cmd + p - quick open

search
crtl + f
crtl + shift + f


crtl + alt + f - formatter

shift + alt + drag - block drag




shift + alt + F12  (find all references - current file)



### characters

Show whitespace - tabs and spaces
Three types of quotes: backtick, single quote, double quote
```
`'" 
```
(watch out for unicode fudgeery of single and double quotes)

Four types of brackets
```
<{[( )]}>
```
Unicode

Live Share
----------

[The best parts of Visual Studio Code are proprietary](https://underjord.io/the-best-parts-of-visual-studio-code-are-proprietary.html) - LiveShare


Browser Based
-------------

* [[ide-in-browser]]
* Hotkeys are masked by browser defaults
    *  TODO: investigate vscode in browser hotkeys

Terminal-IDE
------------

* [an atonement of nano](https://www.noa-s.org/nano.html)
    * for years nano has been nothing but a mockery for those who use emacs or vim. 
    * nano is a friendly and pragmatic editor, but it's no notepad. nano has depth
* [Build Your Own Text Editor](https://viewsourcecode.org/snaptoken/kilo/)
    * [antirez kilo](http://antirez.com/news/108)
    * Pure C - no dependencies
    * 184 steps of adding/remove (like my programming projects)
    * [Text Editor Data Structures](https://cdacamar.github.io/data%20structures/algorithms/benchmarking/text%20editors/c++/editor-data-structures/)

Custom
------

* [Embrace the Chaos](https://edita.vercel.app/blog/approach/) - How to Write a Code Editor from Scratch in 4 Months
    * Building an IDE from scratch is pretty complicated
        * > I’ve written a code editor from the ground up, including: a fast (~120fps) canvas-based editor component; multi-language syntax highlighting with Tree-sitter; snippets; a file browser; find-and-replace with regex and JavaScript expression support; and two completely new features: AST mode and CodePatterns.
    * This [[software-engineering]] approach is - 'Move really really fast and break stuff'

Dark Mode
---------

* [Is Dark Mode Good For Your Eyes?](https://kevquirk.com/is-dark-mode-such-a-good-idea/)
    * > I’ve decided to stop using dark mode across all of my devices, because research suggests that going to the dark side ain’t all that.

[//begin]: # "Autogenerated link references for markdown compatibility"
[history-of-ide]: history-of-ide.md "History of IDE"
[ide-in-browser]: ide-in-browser.md "IDE in browser"
[software-engineering]: software-engineering.md "Software Engineering"
[//end]: # "Autogenerated link references"