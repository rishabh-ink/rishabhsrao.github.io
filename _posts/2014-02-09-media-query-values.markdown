---
layout: post
title: "Media query values"
date: 2014-02-09 23:01:59
comments: true
categories: tech
tags: [css3, media, queries, standard, device, rem]
excerpt: <code>em</code>-based media query values for standard devices.
---
I've converted [Twitter Bootstrap](http://getbootstrap.com)'s [media query values](http://getbootstrap.com/css/#grid-media-queries) to `em`s. Assuming the base font size is `16px`&hellip;

{% highlight scss %}

/* Small devices (tablets, 768px and up) */
$screen-sm-min: 48em;

/* Medium devices (desktops, 992px and up) */
$screen-md-min: 62em;

/* Large devices (large desktops, 1200px and up) */
$screen-lg-min: 75em;

{% endhighlight %}

Some great resources for further reading&hellip;

* [A great list of common CSS @media query breakpoints](http://www.miniarray.com/post/51474660456/a-great-list-of-common-css-media-query-breakpoints) by [{miniArray}](http://www.miniarray.com)
* [7 Habits of Highly Effective Media Queries](http://bradfrostweb.com/blog/post/7-habits-of-highly-effective-media-queries) by [Brad Frost](http://bradfrostweb.com)

As a closing quote,

> the absence of support for @media queries is in fact the ﬁrst @media query...
> &mdash; [Rethinking the Mobile Web by Yiibu (Slide 85)](http://www.slideshare.net/bryanrieger/rethinking-the-mobile-web-by-yiibu/85), [Bryan Rieger](https://twitter.com/bryanrieger)
