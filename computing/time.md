Time
====

Time on computers is hard and #complex
* Leap Years?
* Leap seconds?
* Locale?

* [The Problem with Time & Timezones - Computerphile](https://www.youtube.com/watch?v=-5wpm-gesOY) Tom Scott 10min
* [03:14:07 on Tuesday, 19 January 2038](https://cookieplmonster.github.io/2022/02/17/year-2038-problem/) 32bit unsigned overflow epoc
* [The leap second’s time is up: world votes to stop pausing clocks](https://www.nature.com/articles/d41586-022-03783-5)
* [Falsehoods programmers believe about time](https://gist.github.com/timvisee/fcda9bbdff88d45cc9061606b4b923ca)
* [How a leap second caused havoc with the Internet](https://www.talesfromtheopsside.com/blog/how-a-leap-second-caused-havoc-with-the-internet/)
    * In 2012 the internet broken all over the world at the same time
    * > human-made structures have the ability to affect time. ... “NASA has calculated that the water stored in the Three Gorges Dam in China has increased the length of the day by 0.06 microseconds,”
    * > “The problem with leap seconds is everyone has a different way of implementing it. For Linux systems, which is what we use, as well as a large portion of the Internet, the day can only ever have 86,400 seconds.”
    * > five years prior, someone in the Linux community flagged a potential issue with its leap second implementation. A deadlock, or a computer freeze, could occur. To fix this, a single line of code was changed. A comment was left behind with this change to note one seemingly small caveat: “The only possible side effect of this removal might be that the timer fires one second too late after a leap second.’ Scarily, this side effect is what took down large portions of the Internet in 2012.

You've got 
* the trip round the sun time - this is separate from the duration of a day - it's not an exact (integer division) number of days. - so we need leap years with an extra day.
* The 24h in a day, is not quite exact and you need a leap second to correct this occasionally - you also over the period of thousands of years, the planet spins slower/faster? so we need to correct for that too .. (I think the spin thing is real - need to check)


* [A Very Fast 64–Bit Date Algorithm: 30–40% faster](https://www.benjoffe.com/fast-date-64)
    * Counting years backwards unlocks faster speed.
    * The first date algorithm to use only 4 multiplications, instead of 7+.
* [HN Comments](https://news.ycombinator.com/item?id=46020193)
    * > I wrote my own date calculation functions a while ago. And during that, I had an aha moment to treat March 1 as the beginning of the year during internal calculations. I thought it was a stroke of genius. It turns out this article says that’s the traditional way.
    * > it simplifies the leap year date calculation. If February is the last month of the year, then the possibly-existing leap day is the last day of the year. If you do it the normal way your calculations for March through December need to know whether February is a leap year. Now none of that is needed. You don’t even need explicit code to calculate whether a given year is a leap year: it’s implicit in the constants 146097, 36524, and 1461.
    * > The magic numbers at the end of this explanation are the number of days of each part of the leap year cycle:
      > 146097 days = 400 year portion of the leap year cycles (including leap years during that)
      > 36524 days = same for the 100 year portion of the leap year cycles
      > 1461 days = 4 year cycle + 1 leap day
