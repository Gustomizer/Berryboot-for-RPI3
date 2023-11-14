First of all,

I want to give a special thanks to Floris Bos (maxnet),

who inspired me to start a continuation of his abandoned Berryboot project!


Berryboot
=========

```
Berryboot -- Boot menu / OS installer for ARM devices

Author: Floris Bos <bos AT je-eigen-domein DOT nl> 
License: Simplified BSD - see LICENSE.berryboot for details
Programming language: C++

Source code available at: https://github.com/maxnet/berryboot
```

Website: http://www.berryterminal.com/doku.php/berryboot 


Folders
===

BerrybootGUI2.0 - source of the graphical boot menu and installer interface (uses Qt)
buildroot - build system to create a minimal Linux operating system to run the boot menu under
buildroot/package/berrybootgui2/init - script that gets executed on boot, starts BerrybootGUI


Build requirements
===

Berryboot uses Buildroot to build a minimal Linux operating system to run under.
Buildroot requires that the following packages are installed: http://www.buildroot.org/downloads/manual/manual.html#requirement


To build for the Raspberry Pi 3
===

```
./build-berryboot.sh device_pi3
```

The files in the output folder must be copied to an empty FAT formatted SD card. 
