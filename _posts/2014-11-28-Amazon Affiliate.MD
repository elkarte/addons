---
layout: post
title: "Amazon Affiliate"
category: enhancement
date: 2026-10-31
comments: false
pkid: "TE:AmazonAffiliate"
short: "Automatically add your affiliate tag to Amazon links, short links (amzn.eu, amzn.to, a.co) included"
license: MPL 1.1
version: 2.0.0
allhooks: yes
elkversion: 1.1 - 2.0
support: https://www.elkarte.net/community/index.php?topic=2236.0
bugs: https://github.com/radu81/ElkAmazonAffiliate/issues
author: TE, updated by radu81
thumbnail: https://raw.githubusercontent.com/radu81/ElkAmazonAffiliate/master/images/settings.png
download: https://github.com/radu81/ElkAmazonAffiliate/releases/download/v2.0.0/AmazonAffiliate_2.0.0.zip
images:
  - Settings: https://raw.githubusercontent.com/radu81/ElkAmazonAffiliate/master/images/settings.png
  - Link: https://raw.githubusercontent.com/radu81/ElkAmazonAffiliate/master/images/link.png
---

## Introduction:
Adds your Amazon affiliate tag to every link to an Amazon store, so you can earn from the links your members share.

The link text is never changed: members see the link exactly as they wrote it, only the link destination gets your tag.

## Features:
* Works in topics, personal messages, previews, search results, recent posts and signatures.
* Supports all Amazon marketplaces (amazon.it, .de, .com, .co.uk, .fr, .es...).
* Amazon short links (amzn.eu, amzn.to, amzn.asia, a.co) are resolved to the real product page, so they get your tag too. Results are cached, also when the forum cache is disabled.
* Product links are cleaned to the short `/dp/ASIN` form; search and store pages keep their parameters.
* Affiliate links get `rel="sponsored nofollow"`.
* Optional Amazon icon next to affiliate links.
* English and Italian language files.

## Options:
Admin > Configuration > Add-on Settings
* Amazon affiliate ID (tracking tag), e.g. mysite-21
* Replace tracking tags already present in links
* Resolve Amazon short links
* Show the Amazon icon

### Note:
Short link resolution needs outgoing connections from your server to the Amazon shortener (cURL or allow_url_fopen).
Upgrading from 1.0 on ElkArte 1.1 is supported: use Upgrade in the package manager, the old hooks are removed and your affiliate ID is kept.

## Installation:
{% include install_std.MD %}

### License:
{% include license.MD param="MPL 1.1" %}
