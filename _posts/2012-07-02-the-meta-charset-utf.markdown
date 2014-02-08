---
comments: true
date: 2012-07-02 23:27:14
layout: post
title: "The meta charset mysteries"
excerpt: "Why to <code>UTF-8</code> charset should be set on your HTML pages?"
categories: tech
---

The Mozilla documentation for the [meta element - charset](https://developer.mozilla.org/en/HTML/Element/meta#attr-charset) states the following in its Notes section:

> It is good practice, and strongly recommended, to define the character set using this attribute. If no character set is defined for a page, several cross-scripting techniques may become practical to harm the page user, like the [UTF-7 fallback cross-scripting technique](http://code.google.com/p/doctype/wiki/ArticleUtf7). Always setting this meta will protect against these risks.

It also states that:

> Authors are encouraged to use UTF-8.

Specifying a charset, for example,

{% highlight html %}
    <meta charset="utf-8">
{% endhighlight %}

in the <code>head</code> of your HTML document helps protect against cross-site scripting attacks.

Here's an example of an attack on Google: [Google's XSS Vulnerability](http://shiflett.org/blog/2005/dec/googles-xss-vulnerability).

[Paul Irish](http://paulirish.com) talks about this in his [The Fundamentals, Primitives and History of HTML5](http://paulirish.com/2011/primitives-html5-video) video.

Also, according to the Mozilla docs, it's important to place the charset declaration within the first 512 bytes of your HTML file as some browsers only look at these first bytes before choosing a character set for the page.
