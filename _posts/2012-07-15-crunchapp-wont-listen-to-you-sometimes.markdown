---
comments: true
date: 2012-07-15 00:12:43
layout: post
title: "CrunchApp &mdash; misbehaving"
excerpt: "Is CrunchApp misbehaving? Try this trick."
categories: tech
---

[Crunch](crunchapp.net) is a great app for compiling [LESS CSS](lesscss.org). But sometimes it behaves oddly and doesn't respond to your actions. In such cases, deleting the temporary data does the trick:

Navigate to your user directory in Windows:

{% highlight sh %}
  /Application Data/Adobe/AIR/ELS/app.Crunch
{% endhighlight %}

and delete the following four files:

* <code>PrivateEncryptedData</code>
* <code>PrivateEncryptedDatai</code>
* <code>PrivateEncryptedDatak</code>
* <code>PrivateEncryptedDatav</code>

Now restart CrunchApp and happy crunching!
