---
layout: post
title: "Attachment Image Resizing"
pkid: "Spuds:air_elk"
category: utility
date: 2017-02-10
comments: false
short: "Automatically resizes uploaded attachments to set limits"
license: MPL 1.1
version: 1.0.2
allhooks: yes
elkversion: 1.0-1.1
support: http://www.elkarte.net/community/index.php?topic=1372.0
bugs: https://github.com/Spuds/Elk_Resize_Attachment_Images/issues
author: spuds
thumbnail:
download: https://github.com/Spuds/Elk_Resize_Attachment_Images/releases/download/V1.0.2/elk_ResizeAttachedImages_102.zip
images:
---

## Introduction:
Automatically resizes attached images that are larger than a defined width X height bounding or those that are larger than the allowed maximum size KB as defined in your admin panel.

Will resize attachment imagess (.jpg, .png, .gif, or .bmp) to fit within the bounds specified.  The image format will be maintained unless it is unable to fit the resized image within the max allowed file size specified.  In this case, if the optional change format is enabled, the system will convert the image to JPEG for better compression.

## Features:
-  The ability to set a max width and height for attached images, images are resized proportionately
-  The ability to allow converting image formats only if its required to maintain the file within the specified max file size
-  Allows the post form to attach files up the the maximum allowed by the server, this allows uploading of larger images and then having them resized on the server.

## Installation:
{% include install_std.MD %}

### License:
{% include license.MD param="MPL 1.1" %}