Syntax Highlighting
===================

* [Tree Sitter and the Complications of Parsing Languages](https://www.masteringemacs.org/article/tree-sitter-complications-of-parsing-languages)
    * most IDEs and text editors work (with regex syntax) ... why?
    * Well, because it’s gosh-darn hard to do it the right way. The proper way is to start with a grammar of the language, usually Extended Backus-Naur Format, and work your way through its terse definitions of the language until you have a reasonable grasp of what you need to do and, ah — yes. Now you have to write the parser. And it mustn’t be slow, either; oh, and you have to make it work with broken code, too. Because that’s the resting state of all code that you are editing: as you type the syntax highlighter beavers away in the background to give you some semblance of what reality would look like, if only you’d hurry up and make it syntactically correct, thank-you-very-much.
    * If a regular expression is the answer that yields two problems (as the old joke goes)
    * Even if you did have the grammar and an able parser, the grammar might be wrong or it might lack sufficient context to parse it with that alone. For Python it’s good enough; for C or C++ then I wish you good luck. And for Perl ...
    * Solution - partial updating cached tree