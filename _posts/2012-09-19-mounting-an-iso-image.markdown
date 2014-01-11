---
comments: true
date: 2012-09-19 19:44:17
layout: post
slug: mounting-an-iso-image
title: Mounting an ISO image
wordpress_id: 287
categories:
- Technical
- Tips &amp; Tricks
tags:
- iso
- ISO image
- linux
- mount
- shell
---

Mounting an ISO image as a drive is simple:

    
    mkdir <strong><path-to-where-you-want-to-mount></strong>
    sudo mount -o loop <strong><your-image.iso></strong> <strong><path-to-where-you-want-to-mount></strong>


That's it! Your ISO image will now be mounted and available at the above path.
