---
layout: post
title: "Image Proxy"
category: enhancement
date: 2022-11-21
comments: false
short: "Allows browsers to show http images on https connections"
license: MPL 1.1
version: 1.0.6
pkid: "spuds:imagecache"
allhooks: yes
elkversion: 1.1
support: https://www.elkarte.net/community/index.php?topic=3432.0
bugs: https://github.com/Spuds/Elk_Image_Cache/issues
author: spuds
thumbnail:
download: https://github.com/Spuds/Elk_Image_Cache/releases/download/1.0.6/elk_image_proxy_1-1-6.zip
images:
---

## Introduction:
When using HTTPS connections browsers will not show external images embedded with the img tag that link to HTTP sites as they breach the security of the page.

This addon will serve images embedded with [IMG] tags from your domain through a proxy mechanism. The remote image is saved to your cache directory and served from there. You can choose to do this for all [IMG] tags or just those that would cause "insecure content" warnings when your site is running HTTPS

## Features

 - Added as a core feature
 - Scheduled task to remove images which have not been access in a given period of time
 - Option to cache all [img][/img] files or just those required for proper https validation
 - Automatically will retry fetching failed images up to 10 times.
 - No source edits.

## Installation:
{% include install_std.MD %}

### License:
{% include license.MD param="bsd" %}