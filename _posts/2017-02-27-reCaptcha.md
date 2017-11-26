---
layout: post
title: "reCAPTCHA"
category: security
date: 2017-08-27
comments: false
short: "Adds a Google reCAPTCHA to your site"
license: BSD
version: 1.0.1
allhooks: yes
elkversion: 1.0-1.1
support:
bugs: https://github.com/Spuds/Elk_reCAPTCHA/issues
author: ant59
thumbnail: https://raw.githubusercontent.com/Spuds/Elk_reCAPTCHA/master/sample-images/verification.png
download: https://github.com/Spuds/Elk_reCAPTCHA/releases/download/v1.0.1/elk-recaptcha.zip
images:
  - Settings: https://raw.githubusercontent.com/Spuds/Elk_reCAPTCHA/master/sample-images/settings.png
  - Screen : https://raw.githubusercontent.com/Spuds/Elk_reCAPTCHA/master/sample-images/verification.png
---

## Introduction:
reCAPTCHA is a free service from Google that protects your site from spam and abuse.

## Description
It uses advanced risk analysis techniques to tell humans and bots apart. With the new API, a significant number of your valid human users will pass the reCAPTCHA challenge without having to solve a CAPTCHA. reCAPTCHA comes in the form of a widget that you can easily add to your blog, forum, registration form, etc.

To use reCAPTCHA, you need to sign up for an API key pair for your site [http://www.google.com/recaptcha/admin](http://www.google.com/recaptcha/admin)
The key pair consists of a site key and secret. The site key is used to display the widget on your site. The secret authorizes communication between your application backend and the reCAPTCHA server to verify the user's response. The secret needs to be kept safe for security purposes.

## Options:
You can enable / disable this verifcation control.
Area to enter the site and secret keys.
Ability to define the langauge to use for the captcha form.

## Installation:
{% include install_std.MD %}

### License:
{% include license.MD param="bsd" %}