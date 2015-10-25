--- 
title: Twitter Profile Bookmarklet for Tweetbot
tags: 
- twitter
- bookmarklet
- tweetbot
- automation
type: post
layout: post
published: true
category: blog
---

Every so often I follow a link from a website for a twitter profile and have to copy the username into Tweetbot manually to then follow the user. I'm never logged onto the Twitter mobile site via my phone.

So I created a bookmarklet to take the Twitter profile URL from their mobile site and format using the Tweetbot x-callback-url scheme for opening directly into a users profile. You have to be on the users profile page via the mobile twitter site (eg. https://mobile.twitter.com/username).

    javascript:var%url=document.URL;var%tweetbotProfile=url.replace("https://mobile.twitter.com/","tweetbot:///user_profile/");window.location=tweetbotProfile;

I've [posted a gist](https://gist.github.com/davebradford/9697962) to GitHub, it breaks down each line of JavaScript and explains how to adapt this to work for Twitterific for iPhone.

If you find this useful or can make this bookmarklet more efficient, feel free to [contact me](http://twitter.com/davebradford).

I'm going to try and adapt this in the future to check for non mobile addresses, so I can use this on my iPad as well.

**UPDATE: Sunday 11th May 2014**

I received some great feedback on this bookmarklet. It turns out that Tweetbot doesn't care if the full URL exists in the string which is passed via x-callback-url, very handy to know. Therefore this bookmarklet can be cut down considerably, a new script is listed below. 

Instead it just opens the x-callback-url in Tweetbot for the user profile parameter and adds whatever the previous URL from the address bar.

    javascript:window.location='tweetbot:///user_profile'+location.pathname

Thanks to [lepht](https://github.com/lepht) on GitHub for discovering this and commenting on the original gist.

