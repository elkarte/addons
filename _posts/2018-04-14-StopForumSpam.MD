---
layout: post
title: "Stop Forum Spam"
pkid: "tinoest:StopForumSpam"
category: security
date: 2018-04-14
comments: false
short: "Query the Stop Forum Spam database on user registration and refuse access if above threshold"
license: BSD 3
version: 1.0.0
allhooks: yes
elkversion: 1.1
support: https://github.com/tinoest/ElkStopForumSpam
bugs: https://github.com/tinoest/ElkStopForumSpam/issues
author: tinoest
thumbnail:
download: https://tinoest.co.uk/releases/ElkStopForumSpam.zip
images:
---

## Introduction:
Checks a user against the Stop Forum Spam database when they register, rejects the user if above a threshold

## Features:
Choose wether to block the user based upon their IP, Username and Email Address. Can set a custom threshold level of your choosing. 

## Installation:
Install then set up via the modification settings section within ElkArte.

{% include install_std.MD %}

### License:
{% include license.MD param="BSD 3" %}
