usb-relay-hid
=============

![](http://vusb.wdfiles.com/local--files/project:driver-less-usb-relays-hid-interface/relay2.jpg)

The goal of this little project is to provide open-source API for low-cost USB HID relays 
(search on eBay for "5V USB Relay Programmable Computer Control For Smart Home").

The big advantage of HID-based interface is that no kernel drivers and no simulated COM-ports are needed. It is easy to detect and address the connected devices.

The main project web page is on the [V-USB wiki](http://vusb.wikidot.com/project:driver-less-usb-relays-hid-interface "driver-less-usb-relays-hid-interface"). This is because the firmware of the device is based on [V-USB](http://www.obdev.at/products/vusb/index.html). V-USB enables amazingly simple and low-cost USB hardware solutions.  
This repository contains only the host side software.

The vendors currently offer only an API library for Windows, and only in binary form.

We are not associated with the manufacturer(s) of these devices or author(s) of the original software offered by eBay sellers.
Our intent is to make these devices work on Linux, 64-bit Windows and other platforms where we need it.


Binary downloads, documentation, bugs, TO-DOs and more
----------------------

All this is in the [Github project](http://git.io/bGcxrQ) - see the wiki pages and Issues. 



Current state
-------------

A simple command-line utility for Linux (x86 or x64), Apple OS X and Windows (XP and newer, 32 and 64-bit).

Source of the Windows DLL (USB_RELAY_DEVICE.DLL) and GUI demo app is now available. This is quite compatible with the binaries from the device vendors.


- Windows version: builds with VC++ and WDK 7.1, or VC++ 2013 "community edition" with its matching SDK (Win8.1).
- Linux version builds with gcc and libusb v. 0.1. Tested on RH and Ubuntu.
- OS-X 10.9+ version builds with Xcode and plain IOKit libraries. 


License
-------

Currently we reuse some code from other V-USB projects, which is dual-licensed: GPL + commercial. Until we remove this code, we cannot set any other license. 

We could not locate any copyright information in the software package offered by the eBay sellers. No source code was reused from that package, besides of the C API header (the .h file).
