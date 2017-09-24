---
layout: post
title:  "Get set up for development on mac - Tweaking the terminal"
categories: general
---


# Tweaking the terminal colors

update the bash prompt
to display 
UserName@Hostname:cwd

Add the following to the bash profile

export PS1="\[\033[36m\]\u\[\033[m\]@\[\033[32m\]\h:\[\033[33;1m\]\w\[\033[m\]/\n$ "
export CLICOLOR=1
alias ls='ls -als'

Use the solarized theme
https://github.com/tomislav/osx-terminal.app-colors-solarized
Change font to menlo 11

![terminal 1](/images/terminal-1.png)

![terminal 2](/images/terminal-2.png)

![terminal 3](/images/terminal-3.png)


