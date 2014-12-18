---
layout: post
title: "InLine Attachments"
category: feature
date: 2014-11-17 00:00:00
comments: false
short: "Allows you to place attachments inline with your post text"
license: MPL 1.1
version: 1.0.0
allhooks: yes
elkversion: 1.0
author: "spuds"
thumbnail:
download: https://github.com/Spuds/Elk_Inline_Attachments/archive/master.zip
images:
---

## Introduction:
This addon adds the ability to position your attachments in your post, like the IMG tag, using newly created BBC codes. 

This is useful for inserting attachments inline with your text.  Several types of attachments are possible such as : full-size, thumbnail or link. 

For each attachment you can select how and where the attachment appears within the message. You can also use the same image in multiple areas in the same post. You can of course still have the attachment at the bottom of the post as is the ElkArte default.

## Features:
-  Adds new bbcodes to position attachments within the post, note n is the number of the attachment in the post, eg first = 1, second = 2, etc
  -  [attachimg=n] (full size image)
  -  [attach=n] (thumbnail image)
  -  [attachurl=n] (link with view/download count)
  -  [attachmini=n] (simple link)
-  Use simple [attach] tag to insert the added attachments sequentially
-  Adds optional align and width attributes as [attachimg=1 align=left width=80]
-  Align can be left, right or center.  For left and right aligns the text will flow around the image
-  Width works on attachimg, if the specified width is less than the image then a link (or highslide) is added to one to view the full sized image
-  The default placement of attachments at the bottom of the post is unaffected for the attachments that were not used in line.
-  Works in all areas of the board such as new posts since last visit / all posts of user / new, reply, modify messages / Topic/Reply History.

There are some basic admin settings available with this mod, go to admin - configuration - addon settings - ILA. Here you can disable/enable the mod.

## Installation:
{% include install_std.MD %}

### License:
{% include license.MD param="MPL 1.1" %}