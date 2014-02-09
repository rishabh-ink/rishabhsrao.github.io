---
layout: post
title: "Media query values"
date: 2014-02-09 23:01:59
comments: true
categories: tech
tags: [css3, media, queries, standard, device, rem]
excerpt: <code>rem</code>-based media query values for standard devices.
---
Figuring out media query values for standard devices can be confusing with so many device screens. This post is to document the values that I usually use. What I've done here is that I've taken Twitter Bootstrap's media query values as a reference point. Here, I am assuming that the base font size is `16px`.

{% highlight scss %}

// Mobile devices - Landscape (480px wide or 30rem wide)
$screen-xs: 30rem;

// Tablet devices - Portrait (768px wide or 48rem wide)
$screen-sm: 48rem;

// Tablet devices - Landscape (900px wide or 56.25rem wide)
$screen-md: 56.25rem;

// Desktop devices (1200px wide or 81.25rem wide)
$screen-lg: 81.25rem;

{% endhighlight %}

As a closing quote,

> the absence of support for @media queries is in fact the ﬁrst @media query...
> &mdash; [Bryan Rieger](https://twitter.com/bryanrieger)
