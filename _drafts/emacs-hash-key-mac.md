---
layout: post
title:  "Emacs - hash key woes"
categories: general
---
Where is my hash key.
Alt-3

Fine in most apps , not great in terminal

Create a file in ~/Library/KeyBindings/DefaultKeyBinding.dict with the following contents & restart.
{
  /* Map # to § key*/
  "§" = ("insertText:", "#");
}
 (PICTURE OF KEY ON KEYBOARD)
 
 works most places, but not all i.e. webstorm.
