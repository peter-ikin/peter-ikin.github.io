---
layout: post
title:  "Jekyll"
categories: general
---
## Jekyll 
A static site generator

### Installation

### Basic usage

$ jekyll build --> current folder will be generated into ./_site
  	       --> --destination <dest> where jekyll builds to
	       --> --source <src> which folder to generate from
$ jekyll build --watch -->current folder will be generated into ./_site, watched for changes and regenerated automatically.


$ jekyll serve --> run a dev server at http://localhost:4000, auto regeneration is enabled use '--no-watch' to disable.
$ jekyll serve --detach as above but will run in background

These config options can be specified on command line as above. OR specified in the _config.yml file. placed at the root of the source directory.

e.g. _config.yml
source: _source
destination: _deploy

will result in both of the commands being the same.
$ jekyll build
$ jekyll build --source _source --destination _deploy

### drafts 
create _drafts folder and add drafts to it e.g. draft-post.md
to preview site with drafts do 
$ jekyll serve --drafts