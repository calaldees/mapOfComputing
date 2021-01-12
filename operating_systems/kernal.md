Kernal
======

* [Linux Kernel Map](https://makelinux.github.io/kernel/map/)

* [Why mmap is faster than system calls](https://sasha-f.medium.com/why-mmap-is-faster-than-system-calls-24718e75ab37)
    * Great explanation of what syscalls are
* [Discovering and exploring mmap using Go](https://brunocalza.me/2021/01/10/discovering-and-exploring-mmap-using-go/)
    * [[golang]]

WindowsNT
---------

* [Windows Subsystem for Linux: The lost potential](https://jmmv.dev/2020/11/wsl-lost-potential.html)
    * WSL1 translated linux calls to windows calls and had a single kernal
        * You could see linux process's in the windows process tree
    * WSL2 is just a co-resident kernel (a separate vm)
    * BSD did the translation layer years ago in reverse
