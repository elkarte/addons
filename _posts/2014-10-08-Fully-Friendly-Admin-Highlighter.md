---
layout: post
title: "FFAHM: Fully Friendly Admin Highlighter"
category: enhancement
date: 2014-10-08
comments: false
short: "Highlight most parts of admin area with light cyan when that area is on hover or mouse over"
license: BSD
version: 1.1.1
allhooks: yes
elkversion: 1.0
support: http://www.elkarte.net/community/index.php?topic=2105.0
bugs:
author: ahrasis
thumbnail: http://www.elkarte.net/community/index.php?action=dlattach;topic=2105.0;attach=1718;image
download: http://www.elkarte.net/community/index.php?topic=2105.0
images:
  - Image 1: http://www.elkarte.net/community/index.php?action=dlattach;topic=2105.0;attach=1718;image
  - Image 2: http://www.elkarte.net/community/index.php?action=dlattach;topic=2105.0;attach=1720;image
---

## Introduction:
This addon will highlight most part of admin area with light cyan when that area is on hover or mouse over.

There are two versions of this mod i.e. fixed version and changeable version. You can change light cyan color via addons page for the latter. However for the former, you need to change the light cyan color by editing its css file i.e. FFAHM.styles.css.

While changeable version is easier in terms of color changing, it is using addons database instead of text css file like the one in the fixed version.

![Valid xhtml10](http://validator.w3.org/images/valid_icons/valid-xhtml10)
![Valid css](http://jigsaw.w3.org/css-validator/images/vcss)

## Features:
1. Please do your own backup though every installation is backed up automatically.
2. This mod highlight most admin areas on hover, so you can be certain where you are pointing at.
3. Upon successful installation, in the addons page, you can turn this mod on/off.
4. You can change the default highlight color lightcyan to other preferred color.
5. The line covered is anything thing that fall under the following css:
```#admin_content p.description:hover, #admin_content dl.settings:hover, #admin_content li:hover,
#admin_content .infobox:hover, #admin_content .information:hover,
#admin_content div.windowbg:hover, #admin_content div.windowbg2:hover, #admin_content div.content:hover,
#admin_content tr.windowbg:hover, #admin_content tr.windowbg2:hover, #admin_content tr.standard_row:hover, #admin_content tr:hover td```
6. You can also test it in lower version too as IMO it should work just fine. ;)

## Installation:
{% include install_std.MD %}

### License:
{% include license.MD param="bsd" %}