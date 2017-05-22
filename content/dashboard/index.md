---
date: '2016-03-09T19:56:50+01:00'
title: Dashboard-WETHOD
weight: 20

---


## Hello WETHOD

L_et's create our first content file for yo_ur documenion. Open a terminal and add the following command for each new file you want to add. Replace `&amp;amp;lt;section-name&amp;amp;gt;` with a general term that describes your document in detail.

```
hugo new &amp;amp;lt;section-name&amp;amp;gt;/filename.md

```

Visitors of your website will find the final document under `www.example.com/&amp;amp;lt;section-name&amp;amp;gt;/filename/`.

Since it's possible to have multiple content files in the same section I recommend to create at least one `index.md` file per section. This ensures that users will find an index page under `www.example.com/&amp;amp;lt;section-name&amp;amp;gt;`.

## Homepage

To add content to the homepage you need to add a small indicator to the frontmatter of the content file:

```
type: index

```

Otherwise the theme will not be able to find the corresponding content file.

## Table of contents

You maybe noticed that the menu on the left contains a small table of contents of the current page. All `&amp;amp;lt;h2&amp;amp;gt;` tags (`## Headline` in Markdown) will be added automatically.

## Admonitions

Admonition is a handy feature that adds block-styled side content to your documentation, for example hints, notes or warnings. It can be enabled by using the corresponding [shortcodes](http://gohugo.io/extras/shortcodes/) inside your content:

This will print the following block:

NONE

The shortcode adds a neutral color for the note class and a red color for the warning class. You can also add a custom title:

This will print the following block:

NONE