---
layout: post
title: "Topic Prefixes"
category: security
date: 2014-11-11
comments: false
short: "Introduces the ability to add topic prefixes"
license: BSD
version: 0.0.2
allhooks: yes
elkversion: 1.0
support: http://www.elkarte.net/community/index.php?topic=1424.0
bugs: https://github.com/emanuele45/TopicPrefix/issues
author: emanuele45
thumbnail:
download: https://github.com/emanuele45/TopicPrefix/releases/download/v0.0.2/TopicsPrefix_0-0-2.zip
images:
---

## Introduction:
This addons introduces (guess what?) the topic prefixes feature.
Each topic can be "tagged" with a prefix that will be displayed next to the subject of the topic in several places around the forum.
The admin can create new prefixes and can apply custom styles to them (there is a simple web-interface for that, but it works only for the default theme of the board, and only if the "custom.css" file is present in the root of the theme).

The current version (v0.0.2) is still a beta, some things are not yet implemented (permissions) and others may be broken.

## Features:
-  adding/modifying prefixes to a topic
-  showing prefixes in some places (MessageIndex and Display)
-  list of topics with a certain prefix
-  list of prefixes present in a certain board (above the list of messages)
-  filter topics in a board by prefix (based on the list of prefixes in the board)
-  admin interface to actually create and edit prefixes

###Missing for first release:
-  list of all prefixes (I'm working on that)
-  permissions
-  show prefixes "everywhere"

###Future plans:
-  multiple prefixes per topic
-  merge with tags addon with a switch to decide if a tag is a prefix or a tag or something like that?
-  any suggestion that would come up in the topic

## Installation:
{% include install_std.MD %}

### License:
{% include license.MD param="bsd" %}