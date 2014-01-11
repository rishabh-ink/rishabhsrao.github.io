---
comments: true
date: 2012-07-15 20:56:11
layout: post
slug: opengraph-ogimageurl-relative-vs-absolute-urls
title: OpenGraph og:image:url relative vs. absolute URLs
wordpress_id: 273
categories:
- Technical
- Tips &amp; Tricks
tags:
- absolute
- facebook
- html
- html5
- Markup Languages
- Meta element
- og:image:url
- Open Graph protocol
- opengraph
- relative
- Search engine optimization
- Uniform Resource Locator
---

I was creating an event page for [Youth For Seva](http://youthforseva.org)'s Annual Day '12 at [http://rishabhsrao.github.com/yfs-ad-2012/publish/index.html](http://rishabhsrao.github.com/yfs-ad-2012/publish/index.html) and ran into a problem with [Facebook](https://developers.facebook.com/docs/opengraph)'s [OpenGraph](http://ogp.me)'s og:image:url [meta tag](http://en.wikipedia.org/wiki/Meta_element). It appears that it can't take relative [URLs](http://en.wikipedia.org/wiki/Uniform_Resource_Locator). Bummer! Others have also asked about it [here](http://stackoverflow.com/questions/9858577/open-graph-can-resolve-relative-url) and [here](https://groups.google.com/forum/?fromgroups#!topic/open-graph-protocol/GKfaDWUVwaw). It has to be absolute. I'm gonna try giving a relative URL for now - no choice. Hope it gets implemented in the future.

P.S.: [Facebook Like Linter Tool](http://developers.facebook.com/tools/lint) said:


> **Object Invalid Value**: Object at URL 'http://rishabhsrao.github.com/yfs-ad-2012/publish/index.html' of type 'profile' is invalid because the given value 'img/yfs-logo-only-120.png' for property 'og:image:url' could not be parsed as type 'url'.
