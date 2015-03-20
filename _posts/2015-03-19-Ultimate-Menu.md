---
layout: post
title: "Ultimate Menu"
category: enhancement
date: 2015-03-19
comments: false
short: "Add custom buttons to the main menu"
license: MIT
version: v1.0-beta
allhooks: yes
elkversion: 1.0
support: http://www.elkarte.net/community/index.php?topic=2497.0
bugs: https://github.com/live627/elk-um/issues
author: live627
thumbnail: https://raw.githubusercontent.com/live627/elk-um/master/FireShot%20Screen%20Capture%20%23171%20-%20%27Add%20Button%27%20-%20localhost_Elkarte_index_php_action%3Dadmin%3Barea%3Dumen%3Bsa%3Daddbutton.png
download: https://github.com/live627/elk-um/releases/download/v1.0-beta/ultimate_menu.zip
images:
  - ACP: https://raw.githubusercontent.com/live627/elk-um/master/FireShot%20Screen%20Capture%20%23171%20-%20%27Add%20Button%27%20-%20localhost_Elkarte_index_php_action%3Dadmin%3Barea%3Dumen%3Bsa%3Daddbutton.png
---

## Introduction:
This is a direct port of my SMF mod to Elkarte.

This is a tool for configuring the main menu within Elkarte, allowing custom buttons to be added at will, complete with children and grandchildren menus (so, a main menu item, a dropdown and a follow-on dropdown)

## Known issues:
-  The select lists are lmimited to only 2em (quite bizarre,  but whatever)
-  Grandchild butons cannot be added using 'before'  or 'after'; not sure how to fix this

###Missing for first release:
-  Fixing select list height

###Future plans:
-  Complete rewrite using objects
-  Follow PSR-2 and PSR-4
-  Use generators (PHP 5.5+)
-  Use closures (PHP 5.3+)
-  Use late statiic bindigs (PHP 5.3+)
-  any suggestion that would come up in the topic

## Installation:
{% include install_std.MD %}

### License:
{% include license.MD param="MIT" %}
