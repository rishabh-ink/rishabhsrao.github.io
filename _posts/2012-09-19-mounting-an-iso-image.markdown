---
comments: true
date: 2012-09-19 19:44:17
layout: post
title: "Mounting an ISO image"
categories: tech
excerpt: "A quick tip on how to mount ISO image files in GNU/Linux."
---

Mounting an ISO image as a drive is simple:

{% highlight sh %}

    mkdir path/to/where/you/want/to/mount
    sudo mount -o loop your-image.iso path/to/where/you/want/to/mount

{% endhighlight %}

That&rsquo;s it! Your ISO image will now be mounted and available at the above path.
