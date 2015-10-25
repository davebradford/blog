--- 
title: Moving to Digital Ocean
tags: 
- vps
- server
- digital ocean
- migration
type: post
layout: post
published: ture
---

Two months ago I moved this website over to the fine folks at Digital Ocean, who offer SSD based VPS servers.

I get the freedom to configure everything myself and experiment with configurations that aren't supported with shared hosting. I came over from [Linode](http://linode.com) another VPS provider who are brilliant, I wanted to test to see how easy it was moving everything over and see what Digital Ocean had to offer.

## Basic Server Setup

[Feross Aboukhadijeh](http://feross.org/about/) helped me with most of the details with his guide [How To Set Up Your Linode For Maximum Awesomeness](http://feross.org/how-to-setup-your-linode/). It's focuses mainly toward setting up a Linode but you could apply most of the tweaks and setup to Ubuntu Server LTS 12.04.

I took a tip from my pal [Danny](http://dannytsang.co.uk/) and created a shell script with most of my install automated. In the future I'd like to look into [Puppet](http://puppetlabs.com) as they seem to be the way to go for this kind of stuff.

## Website Deployment

Sometime ago I [moved this site over to Jekyll](http://davebradford.com/blog/moving-away-from-wordpress/), a static-site generator that compiles your site from plain text files. It powers GitHub pages and I could host this site there for free however I have some Jekyll plugins that GitHub do not support.

I keep the source files on my machine and when I need to make changes or update I simple compile the site and sync the changes to my server using [Capistrano](https://github.com/capistrano/capistrano), which allows you to create workflows for remote multi-server automation. 

Although this isn't necessary for a single server having a workflow to compile and publish changes to a remote location works wonderfully. I simply create the directories on my server, point my Capistrano workflow at the new destination and publish!

Digital Ocean have a [great guide on setting this up](https://www.digitalocean.com/community/articles/how-to-get-started-with-jekyll-on-an-ubuntu-vps).

## Finally

Finally I updated my DNS records to point to the new server and waited. This has been the most painless server migration I've completed. 

I put this down to Jekyll and way I can easily re-deploy my site to a new server without extensive configuration.

Digital Ocean offers a great service, overall I am pretty impressed with their performance. If your interested in trying them out, please consider using my [referral link](https://www.digitalocean.com/?refcode=b35972924bb4).
