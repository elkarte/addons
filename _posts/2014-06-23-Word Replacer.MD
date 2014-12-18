---
layout: post
title: "Word Replace"
category: feature
date: 2014-05-23 00:00:00
comments: false
short: "BBC only word censor"
license: BSD
version: 0.1.1
allhooks: yes
elkversion: 1.0
author: "emanuele45"
thumbnail:
download: https://github.com/emanuele45/WordReplacer/archive/master.zip
images:
---

## Introduction:
This is a simple addon, it's task is simply to mimic the word censoring, with a couple of differences:

-  members cannot disable it
-  replacement applies only to text that passes through parse_bbc.  That means for example message bodies, but not subjects.

These differences make the addon useful to replace words with ads or add definition to abbreviations, etc. All the things that once upon a time were done abusing the censoring feature.

## Installation:
{% include install_std.MD %}

### License:
{% include license.MD param="bsd" %}