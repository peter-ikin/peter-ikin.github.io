---
layout: post
title:  "Get set up for development on mac - Homebrew"
categories: general
---
# homebrew for package management

OSX comes with lots of tools preinstalled e.g.
python , perl , ruby etc. though these are perfectly usable, they are only updated when the main OS is updated. Updating these packages out of sequence with the main OS is not recommended as it may cause issues.

It is better to manage different versions of these applications yourself.

Install homebrew - see website
ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
Everything is built on demand and placed in /usr/local/bin (i.e. part of your user area) so nothing requires a sudo to install

type
brew doctor
to check the environment is setup correctly
brew update
will update homebrew itself. If you just got homebrew installed it should already be the latest version.

Its now pretty easy to install stuff through homebrew e.g.
brew install mysql 
will install the mysql database
to see a list of all the packages in homebrew (called formulae) type
brew search
as you can see there is quite a lot available.