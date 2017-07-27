---
layout: post
title: "Double Post Stopper"
category: enhancement
date: 2017-03-17
comments: false
short: "Stop users from double posting and bumping/spamming topics"
license: MIT
version: v1.0
allhooks: yes
elkversion: 1.0
support: http://www.elkarte.net/community/index.php?topic=4336.0
bugs: https://github.com/live627/elk-dps/issues
author: live627
thumbnail: https://raw.githubusercontent.com/live627/elk-dps/master/FireShot%20Screen%20Capture%20%23038%20-%20'Add-on%20Settings'%20-%20localhost_Elkarte10_index_php_action%3Dadmin%3Barea%3Daddonsettings%3Bsa%3Dgeneral.png
download: https://github.com/live627/elk-dps/releases/download/v1.0/double_post_stopper.zip
images:
  - ACP: https://raw.githubusercontent.com/live627/elk-dps/master/FireShot%20Screen%20Capture%20%23038%20-%20'Add-on%20Settings'%20-%20localhost_Elkarte10_index_php_action%3Dadmin%3Barea%3Daddonsettings%3Bsa%3Dgeneral.png
  - Error: https://raw.githubusercontent.com/live627/elk-dps/master/FireShot%20Screen%20Capture%20%23037%20-%20'An%20Error%20Has%20Occurred'%20-%20localhost_Elkarte10_index_php_action%3Dpost%3Btopic%3D906_0%3Blast_msg%3D9995.png
---

[![MIT license](http://img.shields.io/badge/license-MIT-009999.svg)](http://opensource.org/licenses/MIT)
[![GitHub issues](https://img.shields.io/github/issues/live627/elk-dps.svg)](https://github.com/live627/elk-dps/issues)
[![Latest Version](https://img.shields.io/github/release/live627/elk-dps.svg)](https://github.com/live627/elk-dps/releases)
[![Total Downloads](https://img.shields.io/github/downloads/live627/elk-dps/total.svg)](https://github.com/live627/elk-dps/releases)
[![Support](https://supporter.60devs.com/api/b/axlsj1o8o0amepfrr5eqlcjza)](https://supporter.60devs.com/give/axlsj1o8o0amepfrr5eqlcjza)

## Introduction:
Stop users from double posting and bumping/spamming the topics. 

- Setup this mod at Administration Center » Add-on Settings » Miscellaneous.
- Removes Quick Reply if a bump is not allowed
  - Does NOT remove the 'Reply' buttons.
  - This is intentional and is set up to facilitate users receiving the error message, rather than asking (repeatedly) "Why can't I reply?"
- The applicable group threshold is the lowest in the user's groups.
  - Global moderators get 1 hour while newbies have 3 days to wait.
  - If a newbie is also a global moderator, then their wait time is 1 hour.

## Installation:
{% include install_std.MD %}

### License:
{% include license.MD param="MIT" %}
