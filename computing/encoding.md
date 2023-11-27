Data Encoding
=============

* [The Base16, Base32, and Base64 Data Encodings](https://tools.ietf.org/html/rfc3548.html)
    * [Base58](https://tools.ietf.org/id/draft-msporny-base58-01.html)
    * [Base45](https://datatracker.ietf.org/doc/draft-faltstrom-base45/)
    * [Why did base64 win against uuencode?](https://retrocomputing.stackexchange.com/questions/3019/why-did-base64-win-against-uuencode)
* [Encoding and Decoding Base64 Strings in Python](https://stackabuse.com/encoding-and-decoding-base64-strings-in-python/)


* [On Endianness](https://technicalsourcery.net/posts/on-endianness/) #endiann
    * Big Endian Advantages
        * Detecting sign
        * Convention
        * “Naturalness”
        * Sorting unknown uint-struct blobs
    * Little Endian Advantages
        * Detecting odd/even
        * Recasting a pointer
        * Arbitrary precision numbers and arithmetic
        * Arbitrary length encodings
        * Variable length encoding with a prepended length field
    * > The biggest advantages go to little endian because little endian works best with “upward-growing” data (meaning data whose bits cluster to the low bits and grow into the upper empty bits). An example would be integers, which use higher and higher order bits as more digits are needed. And since integers are the most common data type in use, they offer the most opportunities.
    * > Big endian ordering works best with “downward-growing” data. An example would be floating point, which in some little endian architectures is actually stored in big endian byte order (although this practice is not very common due to portability issues).

Data Space
[What 3 Words](https://what3words.com/) - Entire planet in 3m squares
See hashing too
