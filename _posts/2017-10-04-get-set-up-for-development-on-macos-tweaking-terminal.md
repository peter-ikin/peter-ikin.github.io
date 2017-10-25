---
layout: post
title:  "Get Set up for Development on MacOS - Part 2 - Tweaking the terminal"
categories: general
---
# Tweaking the terminal
Out of the box the terminal app is not exactly pretty, it is simple black text on a white background as shown below

![terminal 1](/images/terminal-1.png)

It is possible to customize the terminal to make it more pleasant to work with as well as being easier to read.

# The Prompt and Colors
The first thing I like to customize is the prompt i.e. change the prompt to display UserName@Hostname:cwd, where cwd is 
the current working directory. In order to do this the ``` .bash_profile``` file needs to be edited to add the following.

``` bash
export PS1="\[\033[36m\]\u\[\033[m\]@\[\033[32m\]\h:\[\033[33;1m\]\w\[\033[m\]/\n$ "
export CLICOLOR=1
```

This looks pretty archaic, indeed it is not the most readable thing in the world. You can use the snippet above as is, however if 
you would like more detail there is a comprehensive guide, available [here][prompt-link] that details all the ins and outs 
of bash prompt customization.

# Terminal Themes and font choice
There are many different theme choices available for the terminal app. With the terminal app open, go to the main menu and select 
preferences. From the profiles tab there are a selection of color themes available that can be chosen from. It is also possible to 
use external themes. One theme that I like to use is the solarized dark theme available from [here][theme-link]. Simply download the file
from the url and save it somewhere on your disk. To install the theme click on the cog icon at the bottom of the profiles tab of the terminal
preferences dialog and select import. In addition to the theme I also like to change the font to menlo 11. Once all of the changes above
have been made the terminal app should now look something like the following.

![terminal 2](/images/terminal-2.png)



[prompt-link]: http://www.tldp.org/HOWTO/Bash-Prompt-HOWTO/index.html
[theme-link]: https://github.com/tomislav/osx-terminal.app-colors-solarized
