---
layout: post
title:  "Get Set up for Development on MacOS - Part 3 - Homebrew"
categories: general
---
# Homebrew for package management

MacOS comes with lots of programming tools pre-installed, for instance python, perl, ruby etc. Though thee system versions of these tools
are perfectly usable, they are only updated when the main OS is updated. Updating these packages out of sequence with the main OS is not 
recommended as it may cause issues with the normal operation of your machine. In addition there are many other tools that are not installed 
as default on the MacOS system. 

# Enter Homebrew
Rather than install and manage these packages manually on a case by case basis there is a class of tool, homebrew being one of them, called
a package manager which allows you to easily install, uninstall and upgrade both windowed and command line applications.  

To install homebrew open a terminal and paste in the following command.
``` bash
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```
This downloads and installs the homewbrew ruby scripts. The installation instructions above are also available from the homebrew website [brew.sh][brew-link].

Once installed everything should be good to go. If you want to verify your installation, at any time, you can type the following command at the terminal.
``` bash
brew doctor
```
This command verifies the installation and also performs a number of checks to make sure your homebrew installation is working correctly.
You can also update homewbrew itself through the command line by typing 
``` bash
brew update
```
If you have just got homebrew installed it should already be the latest version and this command will likely do nothing.

Its now pretty easy to install stuff through homebrew e.g.
``` bash
brew install mysql
``` 
would install the mysql database. When using homebrew everything is built on demand and placed in /usr/local/bin (i.e. part of your user area). This means
no elevated priveliges are required (e.g. sudo) to install or run any applications. The installed applications also don't overwrite any of the sytem packages as
they are installed in a different location. It is just as easy to unistall programs by typing ```brew uninstall mysql``` which would result in the mysql package being unistalled.


[brew-link]: https://brew.sh