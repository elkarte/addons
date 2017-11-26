---
layout: post
pkid: "Spuds:gmmMod"
title: "Google Member Map"
category: feature
date: 2017-04-25
comments: false
short: "Adds a member map where members can pin their location"
license: MPL 1.1
version: 1.0.4
allhooks: yes
elkversion: 1.0-1.1
support: http://www.elkarte.net/community/index.php?topic=1374.0
bugs: https://github.com/Spuds/Elk-Google-Member-Map/issues
author: spuds
thumbnail: https://raw.githubusercontent.com/Spuds/Elk-Google-Member-Map/master/sample_images/mm_add.jpg
download: https://github.com/Spuds/Elk-Google-Member-Map/releases/download/1.0.4/elk-Google.Member.Map.zip
images:
  - Add: https://raw.githubusercontent.com/Spuds/Elk-Google-Member-Map/master/sample_images/mm_add.jpg
  - Map: https://raw.githubusercontent.com/Spuds/Elk-Google-Member-Map/master/sample_images/mm_map.jpg
  - Profile: https://raw.githubusercontent.com/Spuds/Elk-Google-Member-Map/master/sample_images/mm_profile.jpg
---

## Introduction:
This installs a member map to your website which allows your members to pin their location on a map. It uses Google Maps 3.0 API to generate the map and place 'Push" pins.

Google Earth can also make use of the pin data. This mod allows for the exporting of user pin data in to a .kml file for those that want to use Google Earth to see their member locations.  Simply add a network link in Google Earth to point at ```http://www.example.com/forums/index.php?action=GoogleMap;sa=kml``` to get the data for Google Earth.  The capability to export .kml files is controlled by the permission to view the map, and keep in mind Google Earth will appear as a guest to your forum.

## How to Use:
In your admin panel you will need to enable it, which implies your acceptance of Google Maps terms of service.  Choose the settings that best work for your site.  There are many settings so you can fine tune the experience for your users and site.  Next, your members will need to edit their profiles and place a pin on the map to show their location and save their profile. That pin will then display on the main member map page. The admin will also need to set the map permissions so users can view the map as well as place a pin on the map.

## Features:
-  Adds a member map button to the main menu under the community dropdown
-  Adds a member profile area for users to add their pin to their profile.  This will then appear on the map.
-  Ability to search by location when placing their pin
-  Adds Profile info bubbles to the map pins
-  Ability to cluster pins together to improve map legibility.  Clusters will expand out as you zoom in on them

## Dependencies:
The Google JavaScript Maps API V3 to create the map and place pins.  This API is available for any web site that is free to consumers. By enabling and using this addon you will be acknowledging and agreeing to the Google terms of use

JSColor project http://jscolor.com/ to select the pin color in the admin interface.  JSColor is by Jan Odvárko and is released under the GNU Lesser General Public License. LGPL differs from GPL by allowing you to use JSColor even in non-(L)GPL applications.

## Installation:
{% include install_std.MD %}

### License:
{% include license.MD param="MPL 1.1" %}
