# Encoding

Previous versions of Fluxion used to support more encoding standards.

Those standards are UTF-16 and UTF-32.

However, these standards are not important since Fluxion supports
UTF-8. 

The way UTF-8 works as it uses Variable-Integer encoding just like
how Fluxion uses to increase the size of one "char" (glyph) from
1 byte (ASCII) to 2 bytes (UTF-16) to 4 bytes (UTF-32).

Since UTF-8 supports the same range and implementing UTF-16 and
UTF-32 in other languages (such as C++ 11) is hard.

In the case of C++ 11, we have to use additional libraries to
use UTF-16 and UTF-32 encoding which inflates the library
size, we decided to cut off the support of UTF-16 and 
UTF-32 in C++ 11 library.

In short, Fluxion v3 only supports UTF-8.
