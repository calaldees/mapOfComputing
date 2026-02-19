Cache
-----


* [Cache Oblivious Algorithms](https://jiahai-feng.github.io/posts/cache-oblivious-algorithms/) Caching stratergies are hard.

* [Myths Programmers Believe about CPU Caches](https://software.rajivprab.com/2018/04/29/myths-programmers-believe-about-cpu-caches/)
    * [[cpu]]
    * MESI
        Modified (M)
            This data has been modified, and differs from main memory
            This data is the source-of-truth, and all other data elsewhere is stale
        Exclusive (E)
            This data has not been modified, and is in sync with the data in main memory
            No other sibling cache has this data
        Shared (S)
            This data has not been modified, and is in sync with the data elsewhere
            There are other sibling caches that (may) also have this same data
        Invalid (I)
            This data is stale, and should never ever be used


* [HTTP caching, a refresher](https://danburzo.ro/http-caching-refresher/)
    * [[http]]
    * The Cache-Control header accepts a set of comma-separated directives, some of which are meant to be added to HTTP requests, and others to HTTP responses. A typical response header:
    * ```
        HTTP/2 200
        Cache-Control: max-age=0, must-revalidate
      ```
    * Some of these directives specifically target shared caches, that is intermediary caches that serve the same cached responses to many users, while others also apply to private caches such as the browser cache.
    * `Cache-Control`, `Expires`, `Date`, `Last-Modified`, `ETag`
    * Cache-Control
        * must-revalidate
        * no-cache
        * no-store
        * must-understand
        * private
        * public
        * s-maxage
        * proxy-revalidate
        * no-transform
        * stale-while-revalidate=`number`
        * stale-if-error=`number`
    * ETag [[etag]]
        * Last-Modified: `date` becomes If-Modified-Since: `date`;
        * ETag: "`value`" becomes If-None-Match: "`value`".
        * When both preconditions are present, only If-None-Match is evaluated.



[cpu]: cpu.md "CPU"


[http]: http.md "HTTP"

[etag]: etag.md "etag"