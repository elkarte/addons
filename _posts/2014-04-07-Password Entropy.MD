---
layout: post
title: "Password Entropy"
pkid: "Spuds:PWEntropy"
category: security
date: 2014-11-10
comments: false
short: "Checks the real strength of an entered password"
license: MPL 1.1
version: 1.0.0
allhooks: yes
elkversion: 1.0-1.1
support: http://www.elkarte.net/community/index.php?topic=1371.0
bugs: https://github.com/Spuds/Elk_Password_Entropy/issues
author: spuds
thumbnail:  https://raw.githubusercontent.com/Spuds/Elk_Password_Entropy/master/sample_images/strong.png
download: https://github.com/Spuds/Elk_Password_Entropy/releases/download/v1.0.1/elk_password_entropy.zip
images:
  - ACP: https://raw.githubusercontent.com/Spuds/Elk_Password_Entropy/master/sample_images/settings.jpg
  - Strong: https://raw.githubusercontent.com/Spuds/Elk_Password_Entropy/master/sample_images/strong.png
  - Poor: https://raw.githubusercontent.com/Spuds/Elk_Password_Entropy/master/sample_images/poor.jpg
  - Weak: https://raw.githubusercontent.com/Spuds/Elk_Password_Entropy/master/sample_images/fail.jpg
---

## Introduction:
This measures the effectiveness of a password in resisting guessing and brute-force attacks. In its usual form, it estimates how many trials an attacker who does not have direct access to the password would need, on average, to guess it correctly. The strength of a password is a function of length, complexity, and unpredictability.

Unlike basic entropy checks which grades based on the set of symbols (a-zA-Z0-9etc) in potential use at each position, this goes further and takes in to account patterns that people will tend to follow and also compares entered passwords against a list of know common passwords that are in use and theretofore vulnerable to attacks. https://tech.dropbox.com/2012/04/zxcvbn-realistic-password-strength-estimation/

## Features:
-  Enable or disable the addon from the control panel
-  Require users to enter a password that meets a set threshold (good/strong/etc)
-  Show a strength meter on most pages where a password can be reset (profile, authentication, registration)
-  Hovering over the password meter will show the estimated time for a computer to crack a given password with a brute force attack

## Installation:
{% include install_std.MD %}

### License:
{% include license.MD param="MPL 1.1" %}

This addon uses the https://github.com/bjeavons/zxcvbn-php library which is released under the The MIT License (MIT)