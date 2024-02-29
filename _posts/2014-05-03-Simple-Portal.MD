---
layout: post
title: "Simple Portal"
pkid: "[SiNaN]:SimplePortal"
category: feature
date: 2024-02-09
comments: false
short: "Adds a portal to your forum, block, article and page support"
license: BSD
version: 1.0.3
allhooks: no
elkversion: 1.1.7
support: https://www.elkarte.net/community/index.php?topic=1399.0
bugs: https://github.com/SimplePortal/SimplePortal_ElkArte/issues
author: Simple Portal Team
thumbnail:
download: https://github.com/SimplePortal/SimplePortal_ElkArte/releases/download/1.0.3/elk_simple_portal-1.0.3.zip
images:
---

## Introduction:
SimplePortal is always developing, and is produced with the user in mind first. User feedback is the number one method of growth for SimplePortal, and our users are always finding ways for Simpleportal to grow. SimplePortal stays competitive with other portal software by adding numerous user-requested features such as articles, block types and the ability to completely customize the portal page.

All this and SimplePortal has remained Simple! SimplePortal is built for simplicity and ease of use; ensuring the average forum administrator can install SimplePortal, configure a few settings, and show off the brand new portal to the users in minutes. Confusing menus, undesired pre-loaded blocks and settings that cannot be found are all avoided as much as possible. Because when it comes down to it, SimplePortal is YOUR portal, and should reflect your taste as much as possible.

## Features:
### ElkArte Unique Features
This version adds **unique functionality** that is available only under the ElkArte platform including:

- Drag and drop block arrangement so each user can customize their portal page
- New block management.  You can simply add custom blocks by placing a block module in the spblocks directory, the new block will be found and made available. Code edits are a thing of the past.
- Modern CSS flexbox layout in place of tables
- Independent article system, supporting BBC, HTML, PHP and Markdown for your writing needs.  It also supports inline attachments for a full Blog feel.
- Drag and drop capabilities in the Admin Panel, you can easily move a block to a new area.
- Improved mobile capabilities, you can define which blocks appear on mobile devices.

### Blocks
Blocks are small display areas you can add to the portal page or to forum pages. You can use blocks to add links for your users, or to show who is online. With Simple Portal, the content part of any page can have LEFT and RIGHT blocks in left and right sidebars, and TOP and BOTTOM blocks between the sidebars above and below the central main content area. There are also overall HEADER and FOOTER blocks that you can load with your content.

There are many built in blocks available, so you can come up with a layout that suits your site. Examples of blocks that are available are: Admin Info, Recent Attachments, Stats, Board News, Custom PHP, Custom HTML, Polls, Shoutbox, Recent Topics, User Info and many more.

Users can also drag and drop the blocks to create a layout that works with their particular tastes or screens, etc.

### Articles
With the article system enabled, you can easily publish them directly on the Portal, no block is necessary. You can also show articles on any SimplePortal Page, or wherever you have blocks displayed, using an article block.

You can create your articles using BBCode, HTML, Markdown or even PHP depending on your needs. You can attach images to your articles and place them inline or aligned to the left or right to give them a blog look and feel.

Articles are assigned to and organized by categories. You can easily create many different categories, and your users can then browse articles by category. No blog system would be complete without a comment functionality and SimplePortal makes that easy.

### Pages
The Simple Portal Custom page is something like the Simple Portal Portal Page. It has areas for blocks surrounding a central area. The center area of a Simple Portal Custom Page is like a Simple Portal Block. The center area is similar to a custom BBC, HTML, Markdown, or PHP block.

When you create or edit a new Simple Portal Page, you will choose from BBC, HTML, Markdown, or PHP. You will input your text, and save your page. You can discover the URL of the new page by looking at the pages list.

If you want links to your new page to appear somewhere that others can see, you will have to place these links yourself. But don't worry -- this part is simple.

### Profiles
Profiles can be defined for Permissions (who can see something), Styles (How the item is styled) and Locations (What ares of the site the item is visible).  These profiles are then be applied to any Block/Page/Article so you can easily and quickly setup multiple areas.  Changing the profile instantly changes all items that use it.  For example if you want to change the style, update a style profile and all areas using that profile will be updated to the new look.

## Installation:
{% include install_std.MD %}

### License:
{% include license.MD param="bsd" %}
