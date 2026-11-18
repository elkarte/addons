# Introduction

You've finished your addon and now want to add it to the [Addon Site](https://elkarte.github.io/addons/) — great!

To do so you need to make a PR to the `elkarte/addons` repo. How to fork a repo, make a local copy, apply your changes, and submit the PR is not covered here; there are many guides on how to do this, and it all depends on what tools you have chosen. This help text assumes you know how to make a PR.

To add your addon to the listing, you need to commit just a single file under the `_posts` directory. The file must follow the naming convention `YYYY-MM-DD-Addon Name.md`. The date should be the initial release date of your addon. It is used to create the permalink, **changing it later will change the permalink**, so pick deliberately. (Hyphens instead of spaces are conventional and safer on the command line, but spaces are permitted.)

The above file must contain the following sections (see any of the existing files in the `_posts` directory for examples):

```
---
front matter
---

detailed description
```

Before submitting, preview locally with `bundle exec jekyll serve` (or watch the CI build) to confirm your YAML parses. A broken front matter is the most common reason a PR fails.

### Front Matter

The front matter is what makes everything cool happen. The front matter must be the first thing in the file and must take the form of valid YAML set between triple-dashed lines. Meaning the information contained between the `---` & `---` tags is in YAML format and is specially processed by Jekyll.

Don't want to learn YAML? Good — neither did I, and you don't have to. Just follow along.

### Example front matter

```yaml
---
layout: post
title: "My Addon"
pkid: "my_addon"
category: feature
date: 2024-01-15
comments: false
short: "Adds a thing to your forum."
license: MIT
version: 1.0.0
allhooks: true
elkversion: 1.0
support: https://www.elkarte.net/community/index.php?topic=123
bugs: https://github.com/you/addon/issues
author: yourhandle
thumbnail: /assets/myaddon/thumb.png
download: /assets/myaddon/myaddon.zip
images:
  - Screenshot 1: /assets/myaddon/screen1.png
  - Screenshot 2: /assets/myaddon/screen2.png
---

Markdown text

## Installation:
{% include install_std.MD %}

## License:
{% include license.MD param="MIT" %}
```

### Front Matter Details

* **layout: post**
  * The name following `layout` is a template file to use when the page is rendered. Use `post` (the standard layout). Others may be added at some point.
* **title: "Title of addon"**
  * The name of the addon. This is used in the template titles and listings.
* **pkid: "Package ID"**
  * The package id as defined in the addon's `package-info.xml` file `<id>` tag. It must match exactly, including case. This is used to link the addon to the `package-info.xml` file in the repo.
* **category: name**
  * This categorizes the type of the addon, used to help group similar items for navigation. Currently, this must be one of the following:
  * `admin`, `utility`, `feature`, `enhancement`, `smiley`, `bbc`, `security`, `avatar`, `other`
* **date: YYYY-MM-DD**
  * `2014-12-20` for example. This date is used to determine the order addons are shown. If you make an important code update, just change the date and it will float to the top. 
* **comments: false**
  * Not currently enabled, but at some point Disqus comments may be enabled.
* **short: "A short description of the addon"**
  * This is your short description of the addon. It will appear in the main listing to provide a short description of what the addon does. Keep it under ~140 characters.
* **license: license**
  * Type of license you are releasing the work under. Typical values here are BSD, MPL 1.1, Apache, MIT, GPL, etc. If it's a common open source license the OSI logo will appear next to it in the listing. The value here should match the `param=` used in the license include (see below).
* **version: x.x.x**
  * Current version of the addon, use what you like — `1.0.0` or `V1 Beta 4`, etc. Although semantic versioning makes it easier for users to know what's the latest version, so consider using it. This is also used by ElkArte to show if a new version is available, but it must follow semantic versioning.
* **allhooks: boolean**
  * Use `true` if the addon is all hook based. This will display a thumbs up on the details page.
  * If some edits are required, set this to `false` or leave it out of the front matter entirely. Addons requiring edits will set a simple notice on the details page.
* **elkversion: 1.0**
  * If a specific minimum version of ElkArte is needed to run the addon, set it here, like `1.1.8`. If the addon is compatible with all versions of ElkArte, leave it out or set it to `1.0`. The value declares a **minimum**, not a range.
* **support: valid link or null**
  * If you have a support thread at ElkArte, or elsewhere, link to it. This will set the Support button on the addons page. If you have no support options, omit the key entirely.
* **bugs: valid link or null**
  * If you have an issue / bug tracker, add the link here. For example, if you use GitHub, link to your issues page for the addon. Leave it out if you don't have an issue tracker or just prefer to use the support thread. A link here sets the Issues button in the template.
* **author: This is you**
  * Your name or GitHub handle. Do I really have to explain this one? If so, how did you get here?
* **thumbnail: valid link or null**
  * This is the URL to an image that is seen as a thumbnail on the main listing page.
  * It does not have to be thumbnail-sized; the CSS of the page takes care of that for you.
  * The link can be to any valid location, including GitHub repos (use raw). You may also choose to save your images directly in the addons repo; to do this, add them under the `assets` folder in their own subfolder, then simply use a relative link such as `/assets/foldername/imagename.xyz`.
* **download: valid link**
  * Where to get the file — it can be anywhere really. Can link to a GitHub release, `master.zip`, or even add it to the addons repo under the `/assets/foldername/addonname.zip` (use a relative link as above). This sets the Download button in the templates.
* **images: ...**
  * This needs to be in a YAML array format, which means `images:` followed by a new line, then **two spaces, dash, one space, alt text, colon, space, URL** (repeat).
  * Each image line takes the form `  - Some name: link`. `Some name` is used as the alt tag value in the template; the link is the location of the image.
  * Omitting the space after the dash is the most common YAML error — make sure the example below is followed exactly.
  * Images are shown below your detailed addon description; they should be screen shots of the addon in action.
  * The location follows the same rules as the thumbnail, so if wanted you can add them to the assets folder and use relative location links.
* **Markdown Text**
  * This is the detailed body describing your addon. Valid Markdown, plain text, or even HTML can be used — the choice is yours, although Markdown text is the preferred method.
  * This is the text that appears on the addon details pages.

**Optional fields:** If you don't have a support thread, issue tracker, or thumbnail, **omit the key entirely**. Don't use the literal string `null` unless you know your parser handles it as intended.

Two helper templates are provided: one is the generic addon installation instructions, and the other is the license block. To use the installation template, add:

```
## Installation:
{% include install_std.MD %}
```

For the license template, use the following, with `param` set to one of: `BSD`, `BSD 2`, `BSD 3`, `MPL 1.1`, `MPL 2.0`, `MIT`, `Apache 2.0`, `WTF`, `GPL 2`, `GPL 3`, `GNU 2`, `GNU 3`, `LGPL`, `LGPL 3`. The `param` value should match the `license:` field in your front matter. If you use a different license, add your own block, or make a PR to add it to `license.MD` in the `_includes` directory.

```
### License:
{% include license.MD param="MPL 1.1" %}
```
