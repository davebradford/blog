---
title: Supercharging my Photo Workflow
tags: 
- photo
- workflow
- iphoto
- lightroom
type: post
layout: post
published: false
--- 

Photo Workflow

There has been a lot of talk about photo management on the internet recently and a few months ago I got thinking about my photo workflow and setup. My pictures break down into two categories.

- photos from my phone
- photos from my digital camera

Previously I've used iPhoto part of the iLife suite of apps, this came with first Mac over 6 years ago. It was a welcome addition to my setup at the time I had a few date stamped folders from my previous setup. iPhoto actually made me take photo organisation seriously but now I'm ready for something more. 

iPhoto is a great start and does a decent job of organisating photos but it comes with a few problems:

- iPhoto uses it's own propiately library format your library is contained into a package where all the original files life and iPhoto keeps all the metadata in it's own database, from time-to-time I'd get database corruption, possible due to the age of my hardware.

Most of my other files I oranigse using a good old trusty files and folder scheme. That's exactly how I'm going to structure my photos.

## Getting photos out of iPhoto

One of my favourite writers [Federio Vittici][http://twitter.com/vittici] has talked about [getting photos out of iPhoto extensively][http://www.macstories.net/tutorials/moving-from-iphoto-to-dropbox/], he used a great little utility called [Phoshare][https://code.google.com/p/phoshare/] to export his photos out but as of October 2012 this is no longer being developed due to limitations in iPhoto 9.4 and has some strange behavior with version iPhoto 9.5. I looked at a few other methods including writing my own automator workflow but after a bit of testing I found the export feature in iPhoto to be more than enough!

I simply selected my whole library from photos File > Export, where I got this dialogue box. 

<< screenshot >>

Under file export I used Kind: Original (I didn't really do too many edits in iPhoto and wasn't worried about loosing any corrections I'd done) with this method I get the original files which I'd imported from my devices by not choosing subfolder format I got a get a big directory of images. Export took a bit of time, I made a cup of tea and came back in later.

## Building a new structure 

### Folders

I'd already decided in my head how I wanted the new structure to look, I wanted a folder for each year, then a month folder for example:

2012 \ 06 - June \ photo.jpg

I tried this at first by using just the month number on it's own, but adding the month in words really helped with the readability when scanning year folders quickly.

I dabbled with the idea of using days as well in the folder structure, but I came to the conclusion that this created unnessary folder levels which where not required. 

The odd photo here and there and small collections can live in the root level for the momth as these will be harder to find it makes scanning the top level a lot easier If i know rougly was month the photo was taken. Larger groups of photos, we can call these events of albums I'll get to it a bit.

### Filenames

Another reason to move to this setup was to create a standard for naming my photos, I decided on the following naming convention:

2012-06-17 13.02.51.jpg

Having the full date and the time helps give the file a unnique name, adding the seconds keep it simple when dealing with burst images or photos taken very close together.

### Events

I would miss having events in iPhoto for large groups of photos, I decided to way I wanted to organise these was to create a folder inside a month with a specicial charater (I've used the @ symbol), the full date again and a breif description of the collection of photos.

2012 \ 06 - June \ @ 2012-06-17 Trip to the Mountains \ photo.jpg

I'm going to breakdown my thinking here:

I've choosen the @ symbol here because it's a valid operating system charater on Windows \ Mac \ Linux filesystems and creating a simple search for just '@' on top level folder will give me a list of all my events/collections/albums whatever you want to call them. Having the full date and the description enables me to see the full date of the event from the search without seeing or knowing the containing directory structure.

<< add information about group events which contain more an than day spanning over one month >>

## Organising the files

Right now I have my file/folder stucture all worked out it's time to get all the photos which I exported earlier into this, the only way this is going to be painless is to automate. 

<< add information about dr drangs photo management scripts >>

I decided in the end to use an app I already had called [Hazel][http://www.noodlesoft.com/hazel.php] which can do some pretty nifty automation tasks to files.

I setup Hazel to look at my directory of files and created a new rule.

<< insert rule information and screenshots >>

Creating the groups of events I choose not to automate, I have a list of a few key events which I wanted to keep together doing this manually was ok as I didn't have many to work though. However I have explored the idea of creating a Hazel rule to look my photos and automatically create groups based on large amount of photos in a specific date. 

reference links
http://lifehacker.com/why-i-ditched-photo-management-apps-and-use-dropbox-ins-1063233673
http://www.macstories.net/tutorials/my-photo-management-workflow-early-2014/














