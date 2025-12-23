Optimizations
=============

* See also [[performance-profileing]]

Web
---

* [Why your website should be under 14kB in size](https://endtimes.dev/why-your-website-should-be-under-14kb-in-size/)
    * 14kb is 10 TCP packets, no need for acks, [[tcp]] slow start. MTU size of 1500bytes (ethernet layer2 limitation)
* [Optimizing Your Web App 100x is Like Adding 99 Servers](https://lukerissacher.com/blog/optimizing_your_web_app)
    * Do we need scalable architecture when you can optimize one box for most cases
* [The mythical “fast” web page](https://calendar.perfplanet.com/2020/the-mythical-fast-web-page/)
    * What is a fast website? #perceived-performance


[[languages]]
-------------

* [High throughput Fizz Buzz](https://codegolf.stackexchange.com/questions/215216/high-throughput-fizz-buzz)
    * GB/per second for fizbuzz generation - drag race
    * `<your_program> | pv > /dev/null`
* [Fast midpoint between two integers without overflow](https://lemire.me/blog/2022/12/06/fast-midpoint-between-two-integers-without-overflow/)


* [Helldivers 2 devs slash install size from 154GB to 23GB, thanks to the help of PC port veterans — ditching HDD optimization, 85% size reduction accomplished by de-duplicating game data](https://www.tomshardware.com/video-games/pc-gaming/helldivers-2-install-size-slashed-from-154gb-to-just-23gb-85-percent-reduction-accomplished-by-de-duplicating-game-data-an-optimization-for-older-mechanical-hard-drives)
    * > bringing the size down from ~154GB to just ~23GB, saving a massive ~131GB of storage space.


[performance-profileing]: performance-profileing.md "Performance Profiling"
[tcp]: tcp.md "TCP"
[languages]: languages.md "Languages"

