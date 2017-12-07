# NewPipe Blog Generator

Repo for the [NewPipe Blog](https://newpipe.schabi.org/blog/).

The blog is based on [Bootstrap](https://getbootstrap.com) 3.3.7 and [Jekyll](https://jekyllrb.com/) 3.6.2.


# Development

#### Installation
Install Jekyll and Bundler gems through RubyGems:
```
~ $ gem install jekyll bundler
```

Navigate to this directory and build the site on the preview server:
```
~ $ jekyll serve
```

Run http://localhost:4000.

# Documentation

#### Categories / Tags
 
We do not make a difference between categories and tags, but only use categories.
Categories are used to tag posts, so they can be found easier.
Every tag has an overview page where you can find all posts with this tag.
Tags are also recognized as keywords by the search and posts get with these tags get an extra boost and are listed higher.
 
You can add a category / tag in the YAML header of each page:
 
 
`categories: category1`
 
`categories: [category1, category2, category3]`
 
Post with tags get the following permalink: `/category1/category2/title`
 
These categories are implemented right now:
 
- release
- article
 
New categories can be implemented via an extra HTML page named `categoryName.html` and placed in the root folder of this repository.
It should look like this:
 
```
---
layout: category
title: categoryName
category: categoryName
---
```