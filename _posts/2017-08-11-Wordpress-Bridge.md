---
layout: post
title: "Wordpress Bridge"
category: enhancement
date: 2017-08-11
comments: false
short: "Bridge logins between WordPress and ElkArte"
license: MIT
version: v1.0
allhooks: yes
elkversion: 1.0
support: http://www.elkarte.net/community/index.php?topic=4618.0
bugs: https://github.com/live627/Wordpress-Elk/issues
author: live627
thumbnail: https://raw.githubusercontent.com/live627/Wordpress-Elk/master/FireShot%20Screen%20Capture%20%23054%20-%20'Wordpress%20Bridge'%20-%20localhost_Elkarte10_index_php_action%3Dadmin%3Barea%3Dwordpress%3Bb1a0948fc%3Ddb47745ca5eb22c9af69eb83a6e99a.png
download: https://github.com/live627/Wordpress-Elk/releases
images:
  - ACP: https://raw.githubusercontent.com/live627/Wordpress-Elk/master/FireShot%20Screen%20Capture%20%23054%20-%20'Wordpress%20Bridge'%20-%20localhost_Elkarte10_index_php_action%3Dadmin%3Barea%3Dwordpress%3Bb1a0948fc%3Ddb47745ca5eb22c9af69eb83a6e99a.png
  - ACP-2: https://raw.githubusercontent.com/live627/Wordpress-Elk/master/FireShot%20Screen%20Capture%20%23055%20-%20'Wordpress%20Bridge'%20-%20localhost_Elkarte10_index_php_action%3Dadmin%3Barea%3Dwordpress%3Bsa%3Droles%3Bb1a0948fc%3Ddb47745ca5eb22c9af69e.png
  - WP-ACP: https://raw.githubusercontent.com/live627/Wordpress-Elk/master/FireShot%20Screen%20Capture%20%23058%20-%20'Plugins%20%E2%80%B9%20wordpress%20%E2%80%94%20WordPress'%20-%20localhost_wordpress_wp-admin_plugins_php.png
---

[![MIT license](http://img.shields.io/badge/license-MIT-009999.svg)](http://opensource.org/licenses/MIT)
[![GitHub issues](https://img.shields.io/github/issues/live627/Wordpress-Elk.svg)](https://github.com/live627/Wordpress-Elk/issues)
[![Latest Version](https://img.shields.io/github/release/live627/Wordpress-Elk.svg)](https://github.com/live627/Wordpress-Elk/releases)
[![Total Downloads](https://img.shields.io/github/downloads/live627/Wordpress-Elk/total.svg)](https://github.com/live627/Wordpress-Elk/releases)
[![Support](https://supporter.60devs.com/api/b/axlsj1o8o0amepfrr5eqlcjza)](https://supporter.60devs.com/give/axlsj1o8o0amepfrr5eqlcjza)

## Introduction:
Bridge logins between WordPress and ElkArte.

- Setup this mod at Administration Center » Wordpress Bridge.
- Logins are synchronized with your WordPrress site once users log into the forum.
  - The included WP plugin will redirect users to the forum if they try to register or login to the blog site.
    - The single file `elk-wp-auth.php` goes into WP's plugins directory
    - It should be activated within the ElkArte site.
 - The bridge will automatically create new users to try to keep everything in sync.

Note that there is a conflict because both ElkArte and WordPress try to load the same password library into the same namespace. This can easily be remedied by adding a small code snippet.

In ./wp-includes/class-phpass.php, find

```
class PasswordHash {
```

and replace it with the following


```
if (class_exists('PasswordHash')) return;
class PasswordHash {
```

I recommend doing this before installing the bridge, to avoid said conflict if you forget this later. It simply checks if the class is already loaded, and skips loading if it's already in memory.

Requires PHP 5.4 or newer to run

Ask about any questions and please donate if you can.

## Installation:
{% include install_std.MD %}

### License:
{% include license.MD param="MIT" %}
