---
layout: post
title:  "Get Set up for Development on MacOS - Part 1 - XCode & Command line tools"
categories: general
---
# Getting Set up for Development on MacOS
This post is the start of a series of tutorials on getting set up as a developer on the MacOS system. The first thing any developer should do
to get there system primed is to download the xcode app and the xcode command line tools. These tools are used by many other applications that we 
may be using even if we never actually touch xcode itself.

# Installing XCode
XCode can be installed from the mac app store just like any other application. The download itself is quite large so it may take a while
to get it downloaded and installed.

# Installing cmd line tools
In addition to the main application there are a selection of command line tools (compilers, linkers etc.) that should be installed as well.
These can be installed by typing the following command from the terminal app.

``` bash 
xcode-select --install
```

Follow the prompt to download the tools ( you don't need to download xcode again ), any further updates to the tools are managed through 
the normal software update process in the mac app store. 

To verify that the installation occured correctly type ```gcc --version``` from the terminal app and you should then get
 some output similar to the following.
``` bash
$ gcc --version
Configured with: --prefix=/Applications/Xcode.app/Contents/Developer/usr --with-gxx-include-dir=/usr/include/c++/4.2.1
Apple LLVM version 9.0.0 (clang-900.0.37)
Target: x86_64-apple-darwin16.7.0
Thread model: posix
InstalledDir: /Applications/Xcode.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/bin
```
 Getting the command line tools installed is an important first step, from here you are ready to proceed with the further setup guides. 