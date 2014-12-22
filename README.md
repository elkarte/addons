##Introduction
You finished your addon and now want to add it to the [addon site](http://addons.elkarte.net), great!  
  
To do so you need to make a PR to the elkarte/addons repo, the how to fork a repo, make a local copy, apply your changes, and submit the PR are not part of this
guide. There are many guides on how to do this and it all depends on what tools you have chosen. This help text assumes you know how to make a PR.  
  
To add your addon to the listing, you need to commit just a single file under the _posts directory. The file must follow the naming convention of
YYYY-MM-DD-Addon Name The date should be the intial release date of your addon, that date is only used to create the permalink to the file.  
  
The above file must contain the following sections (see any of the existing files in the _posts directory for examples)  
```
---  
front matter  
---  
  
detailed description  
``` 
###Front Matter
The front matter is what makes everything cool happen. The front matter must be the first thing in the file and must take the form of valid YAML set between
triple-dashed lines. Meaning the information contained between the --- & --- tags is in YAML format and is specially processed by Jekyll.   
Don't want to learn YAML?, good neither did I and you don't have either, just follow along.  
  
###Example front matter
```
---  
layout: post  
title:"Title of addon"  
category: name  
date: YYYY-MM-DD  
comments:false  
short:"A short description of the addon"  
license: license  
version: x.x.x  
allhooks:boolean  
elkversion:1.0  
support: valid link ornull  
bugs: valid link ornull  
author: thats you  
thumbnail: valid link ornull  
download: valid link  
images:  
  -Some name: link to it  
  -Another name: link to it  
---  
  
Markdown text  
  
## Installation:  
{% include install_std.MD %}  
  
## License:  
{% include license.MD param="BSD"%}  
```
###Front Matter Details
* layout: post  
	* The name following layout is a template file to use when the page is rendered. Currently there is only one choice and that is post. Others may be added at
some point.
* title: "Title of addon"  
	* The name of the addon. This is used in the template titles and listings.
* category: name  
	* This categorises the type of the addon, used to help group similar items for navigation. Currently this must be one of the following.
	* admin, utility, feature, enhancement, smiley, bbc, security, other
* date: YYYY-MM-DD  
	* 2014-12-20 for example. This date is used to determine the order addons are shown. If you make an important code update, just change the date and it will float to the top.
* comments: false  
	* Not currently enabled, but at some point discus comments may be enabled.
* short: "A short description of the addon"  
	* This is your short description of the addon. It will appear in the main listing to provide a short description of what the addon does.
* license: license  
	* Type of license you are releasing the work under. Typical values here are BSD, MPL 1.1, Apache, MIT, GPL etc. If its a common open source license the OSI logo will appear next to it in the listing.
* version: x.x.x  
	* Current version of the addon, use what you like, 1.0.0 or V1 Beta 4, etc. (Although semantic versioning makes it easier for users to know whats the latest)
* allhooks: boolean  
	* Use yes or true if the addon is all hook based. This will display a thumbs up on the details page.
	* If some edits are required, set this to no or leave it out of the front matter entirely. Addons requiring edits will set a simple notice on the details page.
* elkversion: 1.0  
	* If a specific minimum version of ElkArte is needed to run the addon, set it here, like 1.0.2
* support: valid link or null  
	* If you have a support thread at ElkArte, or elsewhere, link to it. This will set the Support button on the addons page. Discard it or leave it blank if you have no support options.
* bugs: valid link or null  
	* If you have an issue / bug tracker, add the link here. For example if you use Github link to your issues page for the addon. Leave it out if you don't have a
issue tracker or just prefer to use the support thread. A link here sets the Issues button in the template
* author: thats you  
	* Do I really have to explain this one, if so how did you get here?
* thumbnail: valid link or null  
	* This is the url to an image that is seen as a thumbnail on the main listing page.
	* It does not have to be thumbnailed sized, the css of the page takes care of that for you.
	* The link can be to any valid location, including Github repos (use raw). You may also choose to save your images directly in the addons repo, for this add them under the assets folder in their own sub folder. Then simply use a relative link such as ```/assets/foldername/imagename.xyz```
* download: valid link  
	* Where to get the file, can be anywhere really. Can link to a Github release, master.zip or even add it to the addons repo under the ```/assets/foldername/addonname.zip``` (use a relative link as above) This sets the Download button in the templates.
* images: ...  
	* This needs to be in a YAML array format, which means images: followed by a new line, then space space dash space item: link (repeat)
	* Again the format of each image line is ```space space dash space some name: link```. some name is used as the alt tag value in the template, the link is the location of the image
	* Images are shown below your detailed addon description, it should be the screen shots of the addon in action.
	* The location follows the same rules as the thumbnail, so if wanted you can add them to the assets folder and use relative location links.
* Markdown Text  
	* This is the detailed body describing your addon. Valid markdown, plain text or even html can be used, the choice is yours, although markdown text is the preferred method.
	* This is the text that appears on the addon details pages
  
Two helper templates are provided, one is the generic addon installation instructions and the other is the license block. To use the installation template add  
```
## Installation:  
{% include install_std.MD %}  
```
For the license template use the following with a param of  
* BSD, BSD 2, BSD 3, MPL 1.1, MPL 2.0, MIT, Apache 2.0, I like fish fingers and custard., GPL 2, GPL 3, GNU 2, GNU 3, LGPL, LGPL 3 If you use a different license
add your own block or make a PR to add it to license.MD in the _includes directory
```
### License:  
{% include license.MD param="MPL 1.1"%} 
```
