Web Assembly
============

WebASMmbly

C applications can be compiled to webassembly target.
The future!

* [CheerpX](https://leaningtech.com/pages/cheerpx.html)
    * [CheerpX -> repl](https://repl.leaningtech.com/)
    * is a x86 to WebAssembly virtualization technology
    * can virtualize native executables or full operating systems
    * can run any x86 application, fully client side

* [The State of WebAssembly 2022](https://blog.scottlogic.com/2022/06/20/state-of-wasm-2022.html)
    * Rust is the most popular compiled labguage
    * Strangely Compiling a javascript runtime in WASM and executing JS code is reasonably feasable

Python (in browser)
------
* [brython](https://brython.info/) - Python3 in the browser instead of javascript
* [Introducing PyScript](https://lwn.net/SubscriberLink/898452/357b195db1ecce28/)
    * ```html
        <py-script>
            print("Hello PyCon 2022!")
        </py-script>
        ```