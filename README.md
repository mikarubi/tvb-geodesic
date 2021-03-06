# External Library Geodesic

[![Build Status](https://travis-ci.org/maedoc/tvb-geodesic.svg?branch=trunk)](https://travis-ci.org/maedoc/tvb-geodesic)

Original library (published under MIT license):
http://code.google.com/p/geodesic/

We added a python wrapped and made small fixes to the original library, to make it compatible with cython.

To install this, either run `pip install gdist` or download these
sources and run `python setup.py install` in current folder.

Basic test could be:
```
python
import gdist
```

Python 2.7, Cython, and a C++ compiler are required.

## Debian package

In order to produce a Debian package, assuming you have the requisite tools
installed (`apt-get install devscripts python-all-dev python-stdeb`)

```
cd debian
debuild -us -uc
cd ../../
```

and you should find a suitable deb file for your system.
