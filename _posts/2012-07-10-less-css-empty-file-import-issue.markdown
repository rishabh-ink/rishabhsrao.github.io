---
comments: true
date: 2012-07-10 21:01:08
layout: post
title: "{less} CSS empty file import issue"
excerpt: "&hellip; and a workaround."
categories: tech
---

Looks like [{less} CSS](lesscss.org) silently fails when you try to import an empty .less file. The issue is documented here: [https://github.com/cloudhead/less.js/issues/853](https://github.com/cloudhead/less.js/issues/853).

A workaround is to declare a dummy variable or something inside the empty <code>.less</code> file.
