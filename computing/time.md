Time
====

Time on computers is hard and #complex
* Leap Years?
* Leap seconds?
* Locale?

* [The Problem with Time & Timezones - Computerphile](https://www.youtube.com/watch?v=-5wpm-gesOY) Tom Scott 10min
* [03:14:07 on Tuesday, 19 January 2038](https://cookieplmonster.github.io/2022/02/17/year-2038-problem/) 32bit unsigned overflow epoc
* [The leap second’s time is up: world votes to stop pausing clocks](https://www.nature.com/articles/d41586-022-03783-5)

* [How a leap second caused havoc with the Internet](https://www.talesfromtheopsside.com/blog/how-a-leap-second-caused-havoc-with-the-internet/)
    * In 2012 the internet broken all over the world at the same time
    * > human-made structures have the ability to affect time. ... “NASA has calculated that the water stored in the Three Gorges Dam in China has increased the length of the day by 0.06 microseconds,”
    * > “The problem with leap seconds is everyone has a different way of implementing it. For Linux systems, which is what we use, as well as a large portion of the Internet, the day can only ever have 86,400 seconds.”
    * > five years prior, someone in the Linux community flagged a potential issue with its leap second implementation. A deadlock, or a computer freeze, could occur. To fix this, a single line of code was changed. A comment was left behind with this change to note one seemingly small caveat: “The only possible side effect of this removal might be that the timer fires one second too late after a leap second.’ Scarily, this side effect is what took down large portions of the Internet in 2012.
