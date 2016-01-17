--- 
title: Moving Away From Wordpress
tags: 
- website
- jekyll
- ruby
- static
- wordpress
type: post
layout: post
category: blog
---

Since as long as I have been on the internet I've been playing around with [Wordpress](http://wordpress.org/), they have two versions a completely hosted version and an open source version which can be installed on a web server, PHP and a database of sorts.

This is great and the whole project has a lot of experience and advanced support, but I wondered what alternatives people were using for blogging. I only do the odd post here and there, maybe my setup was a little overkill. A lower maintenance blog generator and described as blogging for hackers called [Jekyll](https://github.com/mojombo/jekyll)  written in ruby and the backbone for [github pages](http://github.com/pages).

A few migration scripts and some reading of their documentation and I had my Wordpress setup converted into static files and published as a Jekyll site.

The idea is you create a simple layout and include your posts as text files in a directory, which the scripts build a website from, you can put your posts into either markdown or html format and just run Jekyll to recompile the site when your ready to publish.

The benefits of having all your site in static files is mainly speed, without php and database calls it doesn't matter as big your site gets.

I've been building a tutorial for beginners to get straight in and create their first Jekyll powered site. But for now I recommend visiting the github page and read some of the [documentation](https://github.com/mojombo/jekyll/wiki/usage).