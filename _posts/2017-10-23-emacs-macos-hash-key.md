---
layout: post
title:  "Emacs on MacOS - Part 1a - Hash Key Woes"
categories: general
---
# Intro
Welcome to Part 1a of the Emacs on MacOS tutorial series. This is a shorter article targeted at a problem that crops up for certain 
developers with non US keyboard layouts and can be especially irritating for heavy terminal and Emacs users.

# Where is my hash key?
If you have a Mac with a UK keyboard you will have noticed that the hash symbol # also known as the pound symbol is nowhere
to be found. The usual place for this symbol is above the numeral 3 on the keyboard, however in the UK that key has an actual pound symbol £ not 
a faux pound symbol #.

To insert the hash symbol you should use the Alt-3 shortcut which under most circumstances will insert a # into wherever you are typing.

This workaround works fine in most apps, however it does not work great (read - at all) in the terminal or Emacs apps.

# A Solution.
One way around this is to re-purpose one of the under used keys on the keyboard to insert the hash symbol rather than what it usually does.
A prime candidate for this is the rarely used &sect; key.

![key](/images/key-photo.jpg){:width="250px"}

In order to perform this key swap create an empty text file called DefaultKeyBinding.dict in the ~/Library/KeyBindings/ directory.
 Give the file the following contents & restart your machine.
 
```
{
  /* Map # to § key*/
  "§" = ("insertText:", "#");
}
``` 
Now whenever you press the &sect; key it will insert a # symbol instead. This works in the majority of apps however there is the occasional app
where this workaround doesn't work ( e.g. In IntelliJ applications such as WebStorm ). In all of these instances the original Alt-3 shortcut key does work though,

