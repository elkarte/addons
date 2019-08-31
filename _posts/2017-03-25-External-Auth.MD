---
layout: post
pkid: "Spuds:ExternalAuth"
title: "External Authenitcation with Social Media Sites"
category: feature
date: 2019-08-31
comments: false
short: "Allows your users to connect with one click to your ElkArte Forum using their social network accounts."
license: closed
version: 1.0.4
allhooks: yes
elkversion: 1.0-1.1
support: http://www.elkarte.net/community/index.php?topic=4370
bugs: https://github.com/Spuds/Elk_Social_Login/issues
author: spuds
thumbnail: https://raw.githubusercontent.com/Spuds/Elk_Social_Login/master/sample_images/sample3.png
download: https://github.com/Spuds/Elk_Social_Login/releases/download/1.0.4/elk_external_auth_104.zip
images:
  - Admin: https://raw.githubusercontent.com/Spuds/Elk_Social_Login/master/sample_images/sample1.png
  - Profile: https://raw.githubusercontent.com/Spuds/Elk_Social_Login/master/sample_images/sample2.png
  - Login: https://raw.githubusercontent.com/Spuds/Elk_Social_Login/master/sample_images/sample3.png
  - Register: https://raw.githubusercontent.com/Spuds/Elk_Social_Login/master/sample_images/sample4.png
---

## Summary
Allows your users to connect with one click to your ElkArte Forum using their social network accounts.

Supports social networks: Facebook, Twitter, LinkedIn, Google, Yahoo, GitHub

## Description
The settings for the addon are under Admin -> Members -> Registration -> OAuth Providers

Each social network will **require that you** create an external application linking your Web site to their api. These external OAuth applications ensure that users are logging into the correct Web site and allows it to send the user back to the correct Web site after successfully authenticating.

The link to setup your OAuth accounts for these sites is provided in the Admin Panel along with general steps of what to do for each API.  Most important will be the Redirect URIs which is provided in the help for each.

## Features

* Allows a single ElkArte user profile to be connected to multiple social provider accounts
* Follows Elkarte's registration workflow but streamlined with provider authorization.
* Attempt to fetch some profile information from the social site during registartion (avatar, gender, website, etc) access depends on each social site.
* Allows users to authorize / deauthorize providers in their account settings (Modify Profile -> Connected Accounts)
* Allows admin to selectively enable / disable providers
* Allows for one button login to connected accounts

## Installation:
{% include install_std.MD %}

### License:
Currently Closed
