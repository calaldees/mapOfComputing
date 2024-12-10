etag
====

https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/ETag

Server
```
ETag: W/"<etag_value>"
ETag: "<etag_value>"

ETag: "33a64df551425fcc55e4d42a148795d9f25f89d4"
ETag: W/"0815"
```
Weak etags are same content - but not byte for byte the same
(caution string etags are byte for byte the same - including headers!!!)

Client Request
```
If-None-Match: "33a64df551425fcc55e4d42a148795d9f25f89d4"
```
Server Response
```
304 Not Modified
```



https://github.com/sanic-org/sanic/issues/51#issue-183498689
```python
from zlib import adler32
import os.path
    if add_etags:
        headers['ETag'] = '{}-{}-{}'.format(
            int(os.path.getmtime(location)),
            hex(os.path.getsize(location)),
            adler32(location.encode('utf-8')) & 0xffffffff)
```
