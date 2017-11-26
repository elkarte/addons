---
layout: post
title: "Hide User Names"
pkid: "Spuds:Hideusernames"
category: security
date: 2014-09-06
comments: false
short: "Hides usernames from guests and replaces them with a text line of your choice"
license: MPL 1.1
version: 1.0.0
allhooks: yes
elkversion: 1.0-1.1
support: http://www.elkarte.net/community/index.php?topic=1369.0
bugs: https://github.com/Spuds/Elk-Hide-User-Names/issues
author: spuds
thumbnail:
download: https://github.com/Spuds/Elk-Hide-User-Names/archive/master.zip
images:
---

## Introduction:
This mod will hide registered users display names from guests, keeping their identity safe from name collecting bots.  This was created when bots were scrapping names from forum pages, and then using them as user id's in a brute force attack.  This mod simply hides the names so they can't be collected.

## Features:
-  Works without making any theme edits so should work with most themes and addons.
-  Adds a text box in the admin panel where you can enter the name to use as the replacement, e.g. Hidden, Guest, Blocked as examples.

## Installation:
{% include install_std.MD %}

### License:
{% include license.MD param="MPL 1.1" %}