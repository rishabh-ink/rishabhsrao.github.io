---
comments: true
date: 2012-07-15 00:12:43
layout: post
slug: crunchapp-wont-listen-to-you-sometimes
title: 'CrunchApp: Won''t listen to you sometimes'
wordpress_id: 267
tags:
- click
- crunch
- crunchapp
- css
- hang
- less
- not responding
---

[Crunch](crunchapp.net) is a great app for compiling [LESS CSS](lesscss.org). But sometimes it behaves oddly and doesn't respond to your actions. In such cases, deleting the temporary data does the trick:

Navigate to your user directory in Windows:

**\Application Data\Adobe\AIR\ELS\app.Crunch**

and delete all the four files:

**PrivateEncryptedData**  
**PrivateEncryptedDatai**  
**PrivateEncryptedDatak**  
**PrivateEncryptedDatav**

Now restart Crunch and happy crunching!
