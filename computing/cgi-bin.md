CGI-BIN
=======

The old way of running scripts on web request

* [Serving 200 million requests per day with a cgi-bin](https://simonwillison.net/2025/Jul/5/cgi-bin-performance/) 2400 requests per second
    * Modern golang and rust that have almost zero startup make this approach really feasible
    * > CGI programs, because they run as separate processes, are excellent at taking advantage of many CPUs!
