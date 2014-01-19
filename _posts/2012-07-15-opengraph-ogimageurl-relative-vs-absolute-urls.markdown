---
comments: true
date: 2012-07-15 20:56:11
layout: post
title: "OpenGraph Image URLs"
excerpt: "<code>og:image:url</code> values &mdash; <code>relative</code> vs. <code>absolute</code> URLs"
categories: tech
---

I was creating an event page for [Youth For Seva](http://youthforseva.org)'s Annual Day '12 at [http://rishabhsrao.github.com/yfs-ad-2012/publish/index.html](http://rishabhsrao.github.com/yfs-ad-2012/publish/index.html) and ran into a problem with [Facebook](https://developers.facebook.com/docs/opengraph)'s [OpenGraph](http://ogp.me)'s <code>og:image:url</code> [meta tag](http://en.wikipedia.org/wiki/Meta_element). It appears that it can&rsquo;t take relative [URLs](http://en.wikipedia.org/wiki/Uniform_Resource_Locator). Bummer! Others have also asked about it [here](http://stackoverflow.com/questions/9858577/open-graph-can-resolve-relative-url) and [here](https://groups.google.com/forum/?fromgroups#!topic/open-graph-protocol/GKfaDWUVwaw). It has to be absolute. I&rsquo;m gonna try giving a relative URL for now &mdash; no choice. Hope it gets implemented in the future.

The [Facebook Like Linter Tool](http://developers.facebook.com/tools/lint) said,


> **Object Invalid Value**: Object at URL 'http://rishabhsrao.github.com/yfs-ad-2012/publish/index.html' of type <code>profile</code> is invalid because the given value <code>img/yfs-logo-only-120.png</code> for property <code>og:image:url</code> could not be parsed as type <code>url</code>.

---
