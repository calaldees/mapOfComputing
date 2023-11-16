tracking
========

* [How Bear does analytics with CSS](https://herman.bearblog.dev/how-bear-does-analytics-with-css/)
    * GENIUS!
    *   ```css
        body:hover {
            border-image: url("/hit/{{ post.id }}/?ref={{ request.META.HTTP_REFERER }}");
        }
        ```
        * Bots don't do the `:hover`
    * `/hit` endpoint (server side - called from the css above)
        * not store any identifying information about the reader (either in browser cookies, or on the server)
        * use the IP address of the request to determine the country, then hash the IP address along with the date. 
        * All subsequent requests to the page are checked for matching IP address + date hashes and duplicates are discarded.
