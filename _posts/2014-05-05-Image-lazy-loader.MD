---
layout: post
title: "Lazy Load Images"
category: feature
date: 2014-05-05
comments: false
short: "Allows your forum images to lazy load"
license: BSD
version: 0.0.2
allhooks: yes
elkversion: 1.0
support: http://www.elkarte.net/community/index.php?topic=1405.0
bugs: https://github.com/emanuele45/ImgLazyLoading/issues
author: emanuele45
thumbnail:
download: https://github.com/emanuele45/ImgLazyLoading/archive/master.zip
images:
---

## Introduction:
This addon makes all the images "lazy load".  It is common that a website presenting images, some of which will be off screen until the users scrolls down the page.  In this case and in order to make the websites load faster, we can use lazy loading where those off screen images are not fetched until such time as they begin to enter the viewport.

In order to do the lazy loading, the Lazy Load Plugin for jQuery is used.

## Installation:
{% include install_std.MD %}

### License:
{% include license.MD param="bsd" %}