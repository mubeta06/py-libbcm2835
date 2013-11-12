libbcm2835
==========
Fork of mubeta06/py-libbcm2835 to address Python 3 issues

Python bindings to the C library for Broadcom BCM 2835 as used in Raspberry Pi. (http://www.airspayce.com/mikem/bcm2835/)

These bindings require the library be built as a shared library object. To do this manually simply gcc -shared -o libbcm2835.so -fPIC bcm2835.c and copy library to /usr/local/lib.

Installation
------------
1. Clone from git or download zip file and extract

2. In root of download directory type

  sudo python3 setup.py install

NB, you can also use Python 2, simply type

  sudo python setup.py install

3. You can now use the library in your code like so:

import libbcm2835._bcm2835 as soc

print(soc.BCM2835_I2C_REASON_OK)
