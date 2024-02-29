---
layout: post
title: "Turnstile"
category: security
date: 2024-02-29
comments: false
pkid: "spuds:turnstile"
short: "Adds Cloudflare Turnstile CAPTCHA to your site"
license: BSD
version: 1.0.0
allhooks: yes
elkversion: 1.1
support:
bugs: https://github.com/Spuds/Elk_Turnstile/issues
author: ant59
thumbnail: https://raw.githubusercontent.com/Spuds/Elk_Turnstile/master/sample-images/verification.png
download: https://github.com/Spuds/Elk_Turnstile/releases/download/v1.0.0/Tunstile_1-0-0.zip
images:
  - Settings: https://raw.githubusercontent.com/Spuds/Elk_Turnstile/master/sample-images/settings.png
  - Screen : https://raw.githubusercontent.com/Spuds/Elk_Turnstile/master/sample-images/verification.png
---

## Introduction:
Turnstile is a free service from Cloudflare that protects your site from spam and abuse.

## Description
Turnstile delivers frustration-free, CAPTCHA-free web experiences to website visitors. Turnstile stops abuse and confirms visitors are real without the data privacy concerns or awful user experience of CAPTCHAs.

To use Turnstile, you need to sign up for an API key pair for your site https://www.cloudflare.com/products/turnstile/ . The key pair consists of a site key and secret. The site key is used to display the widget on your site. The secret authorizes communication between your application backend and the Turnstile server to verify the user's response. The secret needs to be kept safe for security purposes.

## Options:
You can enable / disable this verifcation control.
Area to enter the site and secret keys.

## Installation:
{% include install_std.MD %}

### License:
{% include license.MD param="bsd" %}