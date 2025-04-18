Compression
===========

* [[compression-image]]
* [[compression-audio]]

* [Taking a Look at Compression Algorithms](https://cefboud.github.io/posts/compression/) 2025
    * Techniques
        Run-Length Encoding (RLE), Lempel-Ziv (LZ), Huffman Coding
    * Formats
        * Gzip, Snappy, LZ4, ZSTD

RLE
---

Huffman
-------
#huffman
* [Building a data compression utility in Haskell using Huffman codes](https://lazamar.github.io/haskell-data-compression-with-huffman-codes/)
    * [[haskell]]
* [What is Huffman Coding?](https://www.baseclass.io/huffman-coding/) 
* [How Computers Compress Text: Huffman Coding and Huffman Trees](https://www.youtube.com/watch?v=JsTptu56GM8&list=PL96C35uN7xGLLeET0dOWaKHkAlPsrkcha&index=3) Tom Scott 6min


* Visible huffman heatmap
    * [MONOSPACE](http://www.p01.org/MONOSPACE/): Flip dots with feelings, a JavaScript demo in 1021 bytes, winner of the 1024 bytes demo competition at Assembly 2020
        * [PNGStore](https://www.iamcal.com/png-store/)

* [Modern LZ Compression](https://glinscott.github.io/lz/index.html) - Gary Linscott 2021
    * walks through the components of a modern LZ compressor
    * create a compressor that can beat gzip while decompressing at almost the same speed — in less than 1000 lines
    * (beautiful single page layout with code)
* [lizard LZ5](https://github.com/inikep/lizard)
    * > Lizard (formerly LZ5) is an efficient compressor with very fast decompression. It achieves compression ratio that is comparable to zip/zlib and zstd/brotli (at low and medium compression levels) at decompression speed of 1000 MB/s and faster. 
* [lzbench Compression Benchmark](https://morotti.github.io/lzbench-web/)
    * > If you ever try to "7-zip ultra" (LZMA) a 4 GB DVD content, or "gzip --strong" a 100 GB database dump, you might realize that it takes 20 hours to run. 20 hours of wasted CPU and electricty and heat, notwistanding 20 hours too long to run it daily, as the daily backup it was supposed to be. That's when zstd and lz4 come in handy and save the day.
    * > zstd (medium) blows deflate (gzip) out of the water, achieving a better compression ratio than gzip while being multiple times faster to compress.
    * > lz4 (fast) blows lzo and google snappy by all metrics, by a fair margin.


* [Dissecting the GZIP format](https://www.infinitepartitions.com/art001.html)
    * The DEFLATE algorithm uses a combination of LZ77, Huffman codes and run-length-encoding; 

New techniques
--------------
* [vectorly](https://vectorly.io/) Vector video on the web (startup beta) - this is a HARD problem - I don't know how far they will get

Algorithms
-----------

https://en.wikipedia.org/wiki/Discrete_cosine_transform

* [Lossless Text Compression](https://bilalonureskili.com/files/LTC_en.pdf)

Licencing
---------

* [An Invisible Tax on the Web: Video Codecs](https://blog.mozilla.org/blog/2018/07/11/royalty-free-web-video-codecs/)
    * H264 and H265 are patented codecs - playing video is not free
    * AV1 is open source


* [Qpus](https://wiki.xiph.org/OpusFAQ) - lossy audio codec





Video
-----

* [Digital Video File Formats - Understanding QuickTime and Video for Windows](http://archive.retro.co.za/CDROMs/DrDobbs/CD%20Release%2012/articles/1994/9413/9413b/9413b.htm) 1994
* [H.264 is Magic](https://sidbala.com/h-264-is-magic/)
    * High level overview of the components of video compression with simple metrics
* [[av1]]

Audio
-----

* [[audio]]
* metadata and payload data
    * [embedded-lyrics](https://cweiske.de/tagebuch/embedded-lyrics.htm) in ogg

Cloud
-----

* [How Facebook encodes your videos](https://engineering.fb.com/2021/04/05/video-engineering/how-facebook-encodes-your-videos/)
    * Using AI to target encoding

[//begin]: # "Autogenerated link references for markdown compatibility"
[compression-image]: compression-image.md "Compression Image"
[compression-audio]: compression-audio.md "Compression Audio"
[haskell]: haskell.md "Haskell"
[av1]: av1.md "AV1"
[audio]: audio.md "Audio"
[//end]: # "Autogenerated link references"