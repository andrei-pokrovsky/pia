pia
===

Calculate the area of intersection of a pair of polygons each
specifed as an array of pairs of floats representing the polygon
vertices.

The return value is a float and is accurate to float precision.
Degenerate cases are avoided by working in exact arithmetic and
"fudging" the exact coordinates to an extent smaller than float
precision.

This code is a derived from Norman Hardy's `aip.c` which can be
downoaded [here](http://www.cap-lore.com/MathPhys/IP/), the
modification being to convert the original GCC-specific code to
C89, and later to C99.  This code compiles with gcc and clang on
x86 and amd64 architectures with `-O3 -std=c99`.

[![Build Status](https://travis-ci.org/jjgreen/pia.png)](https://travis-ci.org/jjgreen/pia)
[![Coverage Status](https://coveralls.io/repos/jjgreen/pia/badge.svg?branch=master)](https://coveralls.io/r/jjgreen/pia?branch=master)
[![Coverity](https://scan.coverity.com/projects/8808/badge.svg)](https://scan.coverity.com/projects/jjgreen-pia)
