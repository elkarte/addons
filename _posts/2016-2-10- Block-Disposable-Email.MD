---
layout: post
title: "Block Disposable Email"
pkid: "spuds:dea"
category: admin
date: 2016-2-10
comments: false
short: "Prevents users from changing to or registering with a disposable email address"
license: MPL
version: 1.0.0
allhooks: yes
elkversion: 1.0
support: https://github.com/Spuds/Elk_Block_Disposable_Email/issues
bugs: https://github.com/Spuds/Elk_Block_Disposable_Email/issues
author: spuds
thumbnail: https://raw.githubusercontent.com/Spuds/Elk_Block_Disposable_Email/master/sample_images/dea.jpg
download: https://github.com/Spuds/Elk_Block_Disposable_Email/archive/master.zip
images:
  - dea: https://raw.githubusercontent.com/Spuds/Elk_Block_Disposable_Email/master/sample_images/dea.jpg
---

## Introduction:
This addon prevents people from registering with disposable email addresses (dea) like the ones provided by mailinator (also known as throw-away email, one-time email). It protects your most important asset, your registered user base, by preventing contamination by fake accounts.

### Features
The addon does not contain a list of domains to block, instead it uses the service of http://www.block-disposable-email.com. This is a very accurate free service for up to 200 queries a month. For larger sites several pay plans are available.  Using the service is more accurate and prevents having to do local maintenance of blacklists etc.

The addon, when activated, prevents both registering with a DEA as well as changing to a DEA (via profile edits)

## Installation:
{% include install_std.MD %}

### License:
{% include license.MD param="bsd" %}
