---
layout: post
title: "Check for Disposable Email"
pkid: "spuds:checkmail"
category: admin
date: 2024-02-28
comments: false
short: "Prevents users from changing to, or registering with, a disposable email address"
license: MPL
version: 1.0.0
allhooks: yes
elkversion: 1.1
support: https://github.com/Spuds/Elk_Check_Mail/issues
bugs: https://github.com/Spuds/Elk_Check_Mail/issues
author: spuds
thumbnail: https://raw.githubusercontent.com/Spuds/Elk_Check_Mail/master/sample_images/checkmail.jpg
download: https://github.com/Spuds/Elk_Check_Mail/releases/download/v1.0.0/checkmail_1-0-0.zip
images:
  - checkmail: https://raw.githubusercontent.com/Spuds/Elk_Check_Mail/master/sample_images/checkmail.jpg
  - failure: https://raw.githubusercontent.com/Spuds/Elk_Check_Mail/master/sample_images/failure.png

---

### Introduction
This addon prevents people from registering with disposable email addresses (dea) like the ones provided by mailinator (also known as throw-away email, one-time email). It protects your most important asset, your registered user base, by preventing contamination by fake accounts.

### Features
The addon does not contain a list of domains to block, instead it uses the service of https://check-mail.org/. 
This is a very accurate free service for up to 1000 queries a month. For larger sites pay for plans are available.  Using the service is more accurate and prevents local maintenance of blacklists etc.  You must sign up for an API key and then choose/subscribe to a plan to use the service.

The addon, when activated, 
  - Prevents both registering with a DEA and changing to a DEA (via profile edits)
  - Checks if the email domain is valid, and lets the user check for input errors

## Installation:
{% include install_std.MD %}

### License:
{% include license.MD param="bsd" %}
