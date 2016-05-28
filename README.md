# Description #

This is a fork of Sigrok's libserialport (https://sigrok.org/wiki/Libserialport) that I created to be compatible with cmake. I wanted to be able to compile it using MinGW alone, without the need for MSYS2 or Cygwin. It compiles fine and creates both shared and static libraries.

# Building #

Make sure you have installed one of the Windows SDKs (I have tested 8 and 10) so that you have the dependencies required for windows (cfgmgr32.lib and SetupAPI.Lib). Once you have that installed, all you need to run in the MinGW terminal is:

* mkdir build
* cd build
* cmake -G "MinGW Makefiles" ..
* make

And obviously you need CMake installed as well.

I have also included precompiled libraries for x64 versions of Windows if you'd like to use those. Just make sure to copy libserialport.h into your "include" directory.

## Contributors ##

Scott Mudge - mail@scottmudge.com (cmake compatibility)

Sigrok Community - everything else (https://sigrok.org/wiki/Libserialport)