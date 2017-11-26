---
layout: post
title: "Descriptive Links"
pkid: "Spuds:DescriptiveLinks"
category: enhancement
date: 2017-04-25
comments: fa11e
short: "This will give URLs posted in your topics an automatic title"
license: MPL 1.1
version: 1.0.2
allhooks: no
elkversion: 1.0-1.1
support: http://www.elkarte.net/community/index.php?topic=1370.0
bugs: https://github.com/Spuds/Elk-Descriptive-Links/issues
author: spuds
thumbnail: https://raw.githubusercontent.com/Spuds/Elk-Descriptive-Links/master/sample_images/dlinks_xmp.jpg
download: https://github.com/Spuds/Elk-Descriptive-Links/releases/download/v1.0.2/elk_descriptive.links.zip
images:
  - ACP: https://raw.githubusercontent.com/Spuds/Elk-Descriptive-Links/master/sample_images/dlinks_acp.jpg
  - Example: https://raw.githubusercontent.com/Spuds/Elk-Descriptive-Links/master/sample_images/dlinks_xmp.jpg
---

## Introduction:
Using this addon will give URLs posted in your topics an descriptive title.  If a user posts a link outside of bbcode tags and optionally within them, this addon will find them, look up the webpage, get the title, and replace the link with a bbcoded url with the webpages title.

```http://www.somesite.com will convert to [url=http://www.somesite.com]Website Title[/url] and display as Website Title```

## Features:
 -  Adds capability to automatically update links in posts to display the links website/page title instead of the url.
 -  Converts internal links to show the topic subject or board name as appropriate, external links to website title
 -  Optional length and generic name protection to avoid changing links to things like Login, Welcome, etc
 -  Optionally convert links contained inside of BBC URL codes
 -  Permissions to allow users to disable link conversion on a per post basis (under post additional options)
 -  Only converts links when the post is saved or modified, ensuring no performance impact during normal message viewing.

## Installation:
This addon make 2 template edits in order to add a checkbox to the post template advanced option section.  This option allows a user to disable the function for a particular post as some links are better left as URL's.

{% include install_std.MD %}

### License:
{% include license.MD param="MPL 1.1" %}