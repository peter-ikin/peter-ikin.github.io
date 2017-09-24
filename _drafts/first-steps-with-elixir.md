---
layout: post
title:  "Emacs - getting started on MacOs"
categories: general
---
## First steps with elixir

Installing on OSX is simply a matter of using homebrew package manager.

brew update

to make sure homebrew is up to date

brew install elixir

which will install elixir and all its pre-requisites which is chiefly erlang.
once homebrew has finished you can check that everything is installed by doing the following

elixir -v

which will print out the version of elixir just installed 

you can also check that erlang has installed correctly by typing
erl
which will bring you into the erlang shell
to exit type
halt().
note the period '.' at the end of the command

Elixir has an interactive shell called iex

bring up Iex by typing 

iex
<image>

for now we can see that we can perform basic calcualtions
e.g. 
1 + 2
3
etc..

In the next post we will hopefully go into more detail of the basic syntax of elixir