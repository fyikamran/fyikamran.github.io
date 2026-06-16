---
layout: post
title: "Jekyll on GitHub Pages"
description: "This site is built with Jekyll and hosted on GitHub Pages"
date: 2026-05-29
last_modified_at: 2026-06-16
category: Internet
tags: [Markdown, jekyll]
image: "/images/default-post.jpg"
image_alt: "Jekyll on GitHub Pages"
slug: "jekyll-gitHub-pages"
schema_file: "schema-article.html"
author: Kamran
published: true
---
This post contains all the things i learn while setting up this site using Jekyll on Github Pages.

* Content
{:toc}

## Jekyll

This is my very first post built natively with Jekyll and hosted on GitHub Pages. Writing in clean Markdown makes publishing incredibly simple.

### Why this setup is awesome:
* **No databases:** Everything runs completely flat and lightning fast.
* **No deployment scripts:** GitHub automatically rebuilds the site the second I save a file.
* **Clean URLs:** No messy dates or `.html` file extensions cluttering the address bar.

## Adding Table of Content in Jekyll
Jekyll uses kramdown by default on Github Pages, so table of content can be added to any post by simply adding {:toc} directly in the post or page markdown. You just need to add the following in the markdown, including the line starting with "*".
```
* Table of Content
{:toc}
```
