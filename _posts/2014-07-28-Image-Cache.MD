---
layout: post
title: "Image Cache"
category: enhancement
date: 2014-07-28
comments: false
short: "Allows browsers to show external images or https connections"
license: BSD
version: 0.1.0
allhooks: yes
elkversion: 1.0
support: http://www.elkarte.net/community/index.php?topic=1791.0
bugs: https://github.com/emanuele45/imgcache/issues
author: emanuele45
thumbnail:
download: https://github.com/emanuele45/imgcache/releases/download/v0.1.0/imgcache_0-1-0.zip
images:
---

## Introduction:
When using HTTPS connections browsers usually do not show external images embedded with the img tag that link to HTTP urls because they breach the security of the page.

This addon, when necessary, fetches a preview of the image, stores it in the cache directory and shows it in place of the original image, along with a message (added through javascript) that instructs the members and visitors to click to see the image at it's original size.

It's a very basic implementation without any setting, more will come.

## Installation:
{% include install_std.MD %}

### License:
{% include license.MD param="bsd" %}