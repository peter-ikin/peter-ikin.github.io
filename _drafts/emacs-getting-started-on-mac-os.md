---
layout: post
title:  "Emacs - getting started on MacOs"
categories: general
---
# Intro

Your in luck emacs is already installed on MacOS.
Open up a terminal app and type emacs , you are greeted with the following screen

![default emacs install](/images/emacs-default.png)

All is good , at least after a fashion. If you look at the version number it is 22.1.1 which is pretty old (we are currently on 25.2.1)


# The app way 

-- head to https://emacsformacosx.com 

Download the dmg file and double click it

Then drag the app into the applications folder in the dialog.

The emacs app will now show up in all the usual places that an app would (launcher , applications folder etc.)

![emacs install screen](/images/emacs-install-screen.png)

/Applications/Emacs.app/Contents/MacOS/Emacs -nw 

Need to alias into .bash_profile
Alias emacs='/Applications/Emacs.app/Contents/MacOS/Emacs -nw'

# Using homebrew

If you don't have it already install homebrew with

/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

Then using homebrew install emacs with

brew install emacs - -with-cocoa

this installs the latest version of emacs (25.2) in the 
/usr/local/Cellar/emacs/25.2 directory

in here there is a MacOS app (Emacs.app) also in the bin directory is an emacs executable that can be invoked from the command line

ie. /usr/local/Cellar/emacs/25.2/bin/emacs
As with the previous installation method executing this will start the Mac app, if you want emacs to launch in the current terminal window use the -nw option.

As  before it is useful to setup an alias in your .bash_profile

alias emacs=‘/usr/local/Cellar/emacs/25.2/bin/emacs -nw’
also if you want to have the app show up in the launchpad, create an alias through UI by opening up a finder window and select go to folder and go to the folder above. then right click on the emacs.app and select make alias. Rename the alias if you wish, then move it to the applications folder.