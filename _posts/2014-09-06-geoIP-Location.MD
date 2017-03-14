---
layout: post
title: "geoIP Location"
pkid: "Spuds:geoipMod"
category: feature
date: 2017-03-14
comments: false
short: "Adds an on-line member map which will shows a map pin for each IP currently on your forum"
license: MPL 1.1
version: 1.3.0
allhooks: no
elkversion: 1.0.8
support: http://www.elkarte.net/community/index.php?topic=1812.0
bugs: https://github.com/Spuds/Elk-GeoIP/issues
author: spuds
thumbnail: https://raw.githubusercontent.com/Spuds/Elk-GeoIP/master/sample_images/geoip_thumb.jpg
download: https://github.com/Spuds/Elk-GeoIP/releases/download/V1.3/elk_geoIP_13.zip
images:
  - Map: https://raw.githubusercontent.com/Spuds/Elk-GeoIP/master/sample_images/geoip_map.jpg
  - Map Settings: https://raw.githubusercontent.com/Spuds/Elk-GeoIP/master/sample_images/geoip_map_settings.jpg
  - Menu: https://raw.githubusercontent.com/Spuds/Elk-GeoIP/master/sample_images/geoip_menu.jpg
  - Registrations: https://raw.githubusercontent.com/Spuds/Elk-GeoIP/master/sample_images/regsettings.jpg
---

## Introduction:
This modification adds the ability to use the latitude & longitude of a member given their IP address. This is commonly referred to as geolocation. The mod makes use of the geoip capabilities in Nginx or Apache web servers. You **must** have this capability enabled in your web server and they **must** make the following enviroment variables available to PHP ('GEOIP_LATITUDE', 'GEOIP_LONGITUDE' 'GEOIP_CITY_COUNTRY_NAME', 'GEOIP_CITY', 'GEOIP_REGION', 'GEOIP_CITY_COUNTRY_CODE')

*A note on accuracy*: Maxmind shows that this database (which is updated on a monthly basis) is over 99.5% accurate on a country level making it a viable source for registration blocking.

When it comes to the city level accuracy this number is and 79% for the US (within a 25 mile radius). That is the best accuracy, and other countries city/region location accuracy tapper off from that. Even with that level of accuracy, it still makes for an entertaining online member map.

In some instances the IP address will not be found, or will have incomplete data. In this case the mod will make use of secondary sources to gather information.

## Features:
-  Adds an on-line member map which will show a map pin for each IP currently on your forum
-  Adds the ability to block or allow member registrations on a per country basis
-  Adds in the geoIP information under the track IP sections, allows you to see city / region (state) / country of the IP address
-  Todo add country flag to online member list

There are admin settings available with this addon, go to admin - configuration - modification settings - geoIP.

## Installation:
The package will install on all systems, however you **must** have geoip capabilities enabled in the web server and the environment variables made available to PHP. If you are on shared hosting, check with your host, or if you are on a VPS you can read more about it here: http://www.howtoforge.com/using-geoip-with-nginx-on-ubuntu-12.04 as an example of what is needed.

This addon requires a single edit to Logging.php, other than that it is all hook based.

{% include install_std.MD %}

### License:
{% include license.MD param="MPL 1.1" %}