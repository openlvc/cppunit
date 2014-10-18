CppUnit Git Mirror for OpenLVC
===============================

I love C++. No really, I do (not really).

Various OpenLVC projects make use of CppUnit to test their C++ interfaces.
The source for CppUnit live in an SVN repo on SourceForge (link below), but
we live in the new world, so we love Git. This repository is the canonical
source of CppUnit for all OpenLVC projects, it is periodically built to
static libraries that can then be included as third-party deps.

Original Source Location:
https://svn.code.sf.net/p/cppunit/code/trunk


Building CppUnit on Mac OS X
-----------------------------
These instructions were used to build CppUnit on Mac OS X 10.9 (Mavericks).

```
sudo port install autoconf // if not already installed
sudo port install automake // if not already installed
sudo port install libtool  // if not already installed - will give you glibtoolize
cd cppunit
./autogen.sh
./configure --disable-shared
make
```

The library can then be located in `src/cppunit/.libs/libcppunit.a`


