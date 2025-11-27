javascript (ECMAScript)
==========

* [ECMAScript Language Specification](https://tc39.es/ecma262/)
* [The Modern JavaScript Tutorial](https://javascript.info/)
* [Modern Javascript: Everything you missed over the last 10 years](https://turriate.com/articles/modern-javascript-everything-you-missed-over-10-years)
* [Deep JavaScript](https://exploringjs.com/deep-js/toc.html)
* [JavaScript for Data Science](http://js4ds.org/) - complete book of how to code, but focusing on techniques for data science
    * Great examples and diagrams
* [A Guide to Console Commands](https://css-tricks.com/a-guide-to-console-commands/)
    * console.log
    * .assert
    * .count
    * .group .groupEnd
    * .table([])
    * .time .timeLog .timeEnd
    * .trace()
* [CSS-Tricks - Web Javascript Snippets](https://css-tricks.com/snippets/javascript/)
* [Why I’m skeptical of rewriting JavaScript tools in “faster” languages](https://nolanlawson.com/2024/10/20/why-im-skeptical-of-rewriting-javascript-tools-in-faster-languages/)

http://vanilla-js.com/
* https://plainvanillaweb.com/
    * No dependencies, no frameworks, no build chain
    * An explainer for doing web development using only vanilla techniques. No tools, no frameworks — just HTML, CSS, and JavaScript.
* [Vanilla JavaScript support for Tailwind Plus](https://tailwindcss.com/blog/vanilla-js-support-for-tailwind-plus)
https://htmldom.dev/

https://developer.mozilla.org/en-US/docs/Web/JavaScript

https://github.com/morris/vanilla-todo

http://youmightnotneedjquery.com/
* [replace-jquery](https://github.com/sachinchoolur/replace-jquery)
  * Automatically finds jQuery methods from existing projects and generates vanilla js alternatives.
* [cash](https://github.com/fabiospampinato/cash) -  An absurdly small jQuery alternative for modern browsers.

* [Using ES Modules (ESM) in Node.js: A Practical Guide (Part 1)](https://gils-blog.tayar.org/posts/using-jsm-esm-in-nodejs-a-practical-guide-part-1/)
    * How to use ES2015+ modules

* [khalidx/node-typescript-esm.md](https://gist.github.com/khalidx/1c670478427cc0691bda00a80208c8cc)
    * The experience of using Node.JS with TypeScript, ts-node, and ESM is horrible.
    * There are countless guides of how to integrate them, but none of them seem to work.
    * Here's what worked for me.
    * Just add the following files and run `npm run dev`. You'll be good to go!
    * `package.json`

* [ES2015+ cheatsheet](https://devhints.io/es6)
* [10 New JavaScript Features in ES2020 That You Should Know](https://www.freecodecamp.org/news/javascript-new-features-es2020/)

* [es6-cheatsheet](https://github.com/DrkSephy/es6-cheatsheet)
* [JavaScript destructuring like Python kwargs with defaults](https://www.peterbe.com/plog/javascript-destructuring-like-python-kwargs-with-defaults)
    * ```javascript
        function processFolder({source,destination = "/tmp",quiet = false,verbose = false} = {}) {
            // all args as kwargs (no positional)
        }
        console.log(processFolder({ source: "/user", quiet: true }))
        ```

https://til.hashrocket.com/posts/yq02bobyth-swap-javascript-array-items-inline
```javascript
[array[0], array[1]] = [array[1], array[0]]
```
* [Sparse vs Dense Arrays in JavaScript](https://dmitripavlutin.com/javascript-sparse-dense-arrays/)

* [GPU.js](https://gpu.rocks/)
    * Wrapper for using javaacript on GPU's
* [sheetJS](https://sheetjs.com/)
    * Import/export, live edit and sql spreadsheets
