---
layout: post
title: "Footer Menu"
category: enhancement
date: 2016-08-07
comments: false
short: "Appends a menu to the bottom of every page"
license: MIT
version: v1.0
allhooks: yes
elkversion: 1.0.7
support: http://www.elkarte.net/community/index.php?topic=3938.0
bugs: https://github.com/live627/elk-footer-menu/issues
author: live627
thumbnail: https://raw.githubusercontent.com/live627/elk-footer-menu/master/FireShot%20Screen%20Capture%20%23015%20-%20'Footer%20Menu%20-%20Add'%20-%20localhost_Elkarte10_index_php_action%3Dadmin%3Barea%3Dfootermenu%3Bsa%3Deditcategory%3Bc10a4ac%3D5914932a804e96.png
download: https://github.com/live627/elk-footer-menu/releases/download/v1.0/footermenu.zip
images:
  - ACP: https://raw.githubusercontent.com/live627/elk-footer-menu/master/FireShot%20Screen%20Capture%20%23007%20-%20''%20-%20localhost_Elkarte10_index_php_action%3Dadmin%3Barea%3Dfootermenu%3Bsa%3Dindex%3Bc10a4ac%3D5914932a804e964621cac644660be788.png
  - ACP: https://raw.githubusercontent.com/live627/elk-footer-menu/master/FireShot%20Screen%20Capture%20%23008%20-%20'Footer%20Menu%20-%20Add'%20-%20localhost_Elkarte10_index_php_action%3Dadmin%3Barea%3Dfootermenu%3Bsa%3Dedit%3Bc10a4ac%3D5914932a804e964621cac6.png
  - ACP: https://raw.githubusercontent.com/live627/elk-footer-menu/master/FireShot%20Screen%20Capture%20%23010%20-%20''%20-%20localhost_Elkarte10_index_php_action%3Dadmin%3Barea%3Dfootermenu%3Bsa%3Dcategories%3Bc10a4ac%3D5914932a804e964621cac644660be788.png
  - ACP: https://raw.githubusercontent.com/live627/elk-footer-menu/master/FireShot%20Screen%20Capture%20%23011%20-%20'Footer%20Menu%20-%20Add'%20-%20localhost_Elkarte10_index_php_action%3Dadmin%3Barea%3Dfootermenu%3Bsa%3Deditcategory%3Bc10a4ac%3D5914932a804e96.png
  - Foot: https://raw.githubusercontent.com/live627/elk-footer-menu/master/FireShot%20Screen%20Capture%20%23012%20-%20'Footer%20Menu%20-%20Add'%20-%20localhost_Elkarte10_index_php_action%3Dadmin%3Barea%3Dfootermenu%3Bsa%3Deditcategory%3Bc10a4ac%3D5914932a804e96.png
  - Foot: https://raw.githubusercontent.com/live627/elk-footer-menu/master/FireShot%20Screen%20Capture%20%23014%20-%20'Footer%20Menu%20-%20Add'%20-%20localhost_Elkarte10_index_php_action%3Dadmin%3Barea%3Dfootermenu%3Bsa%3Deditcategory%3Bc10a4ac%3D5914932a804e96.png
  - Foot: https://raw.githubusercontent.com/live627/elk-footer-menu/master/FireShot%20Screen%20Capture%20%23015%20-%20'Footer%20Menu%20-%20Add'%20-%20localhost_Elkarte10_index_php_action%3Dadmin%3Barea%3Dfootermenu%3Bsa%3Deditcategory%3Bc10a4ac%3D5914932a804e96.png
---

[![MIT license](http://img.shields.io/badge/license-MIT-009999.svg)](http://opensource.org/licenses/MIT)
[![GitHub issues](https://img.shields.io/github/issues/live627/elk-footer-menu.svg)](https://github.com/live627/elk-footer-menu/issues)
[![Latest Version](https://img.shields.io/github/release/live627/elk-footer-menu.svg)](https://github.com/live627/elk-footer-menu/releases)
[![Total Downloads](https://img.shields.io/github/downloads/live627/elk-footer-menu/total.svg)](https://github.com/live627/elk-footer-menu/releases)
[![Support](https://supporter.60devs.com/api/b/axlsj1o8o0amepfrr5eqlcjza)](https://supporter.60devs.com/give/axlsj1o8o0amepfrr5eqlcjza)
## Introduction:
This is a direct port of my SMF mod to Elkarte.

Appends a menu to the bottom of every page

- Admin settings are under the Forum sub-menu in the admin panel.
- Unlimited categories and links
- Is cached in the settings table so no extra query per page load is needed
- Follows default database order (usually chronologically but is based on ID)
- If the cache get corrupt, simply edit an item, make no changes, click save
- Categories will not show unless it contains at least one link

## Installation:
{% include install_std.MD %}

### License:
{% include license.MD param="MIT" %}
