---
layout: post
title:  "Ruby"
categories: general
---
# Ruby tutorial series
Install rvm using inbuilt ruby
\curl -sSL https://get.rvm.io | bash -s stable --ruby

Rvm list known
Rvm install ruby-2.4.0

edoras:~ peterikin$ which ruby
/Users/peterikin/.rvm/rubies/ruby-2.4.0/bin/ruby
edoras:~ peterikin$ ruby --version
ruby 2.4.0p0 (2016-12-24 revision 57164) [x86_64-darwin16]
edoras:~ peterikin$ 

## Install ruby version manager (RVM)

see rvm.io for curl line.

## basic usage

rvm requirements --- > installs all the requirements that rvm needs via brew?
### install rubies
rvm install <ruby-version>

e.g. rvm install ruby-2.2.1  
e.g. rvm install ruby-head


### listing
rvm list --> list rmv rubies installed
rvm list gemsets --> list rubies and gemsets
rvm gemset list --> gemsets for current rubies

### using rubies
rvm use <version>
 e.g. rvm use ruby-2.2.1
 e.g. rvm use system --> use the system ruby


### Updating RVM
rvm get stable --> for latest stable version
rvm get head --> for head version (most bugfixes)

### upgrading rubies
rvm upgrade (old version) (new version)
e.g. rvm upgrade 2.2.1 2.3.1

