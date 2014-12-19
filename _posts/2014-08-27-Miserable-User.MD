---
layout: post
title: "Miserable User"
category: feature
date: 2014-09-06
comments: false
short: "Targets problem users and enables various site deterrents to disrupt their visit"
license: MPL 1.1
version: 1.0.0
allhooks: yes
elkversion: 1.0
support: http://www.elkarte.net/community/index.php?topic=1907.0
bugs: https://github.com/Spuds/Elk-Misery/issues
author: spuds
thumbnail:
download: https://github.com/Spuds/Elk-Misery/archive/master.zip
images:
---

## Introduction:
This addon allows you to target specific users and give them the special gift of "misery" until they chill out or leave your community.
It can be used as
-  As an alternative to banning or deleting users from a community.
-  As a means by which to punish members of your community.
-  To delight in the suffering of others.

In your admin panel you will need to enable it, and set the various misery options in percent.  You will find the settings under Security and Moderation -> Misery

## Features:
The aim of misery is to be not traceable by users that are on the list, so misery actions should be sufficiently subtle to avoid suspicion. It provides that selected users may experience various "errors" interrupting their site experience.

The following page load misery can be applied:

-  Delay: Creates a random-length delay, giving the appearance of a slow connection
-  White screen: Presents the user with a white-screen
-  Wrong page: Redirects to a defined URL instead of the page they requested
-  Random HTTP errors: Presents error screens like 403 Access Denied, 404 Not Found, etc
-  JS popup: Shows a user defined message (by default it says to enable cookies) that they must clear to continue
-  Logout: Log the user out

Form misery (posting, PM, email) when applied will randomly result in the following errors

-  They submit but it does not actually post
-  The message subject is removed and they are warned that a subject is needed
-  The message body is removed and they are warned that a message can't be left blank
-  Session timeout error
-  Already submitted error
-  Post to long error

Feature disabled, blamed on server load, includes

-  Search disabled
-  New replies to your posts disabled
-  Show this user's posts disabled
-  Show unread posts since last visit disabled
-  Show recent posts disabled

## Installation:
{% include install_std.MD %}

### License:
{% include license.MD param="MPL 1.1" %}