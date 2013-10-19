libbcm2835
==========

Python bindings to the C library for Broadcom BCM 2835 as used in Raspberry Pi. (http://www.airspayce.com/mikem/bcm2835/)

These bindings require the library be built as a shared library object. To do this manually simply gcc -shared -o libbcm2835.so -fPIC bcm2835.c and copy library to /usr/local/lib.
