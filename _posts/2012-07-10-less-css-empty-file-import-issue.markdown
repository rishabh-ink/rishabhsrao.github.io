---
comments: true
date: 2012-07-10 21:01:08
layout: post
slug: less-css-empty-file-import-issue
title: '{less} CSS empty file import issue'
wordpress_id: 231
categories:
- Technical
- Tips &amp; Tricks
tags:
- css
- empty
- import
- less
---

Looks like [{less} CSS](lesscss.org) silently fails when you try to import an empty .less file. The issue is documented here: [https://github.com/cloudhead/less.js/issues/853](https://github.com/cloudhead/less.js/issues/853).

A workaround is to declare a dummy variable or something inside the empty .less file.
