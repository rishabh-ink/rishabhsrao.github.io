---
layout: post
title: "Internet Explorer &mdash; table rendering bug"
date: 2014-01-11 08:59:59
comments: true
categories: tech
tags: [ie, table, missing, border, borders, empty, cell]
excerpt: Tables render with missing borders on empty cells.
---

The other day I came across a strange issue in Internet Explorer. Empty cells in a `<table>` element were being rendered with missing borders. As you can see in the screenshot below, the empty cells have missing borders&hellip;

![](/img/posts/2014-01-31-internet-explorer-table-rendering/table-rendering-bug.PNG)

After some googling, I came across a [Stack Overflow question](http://stackoverflow.com/questions/57002/css-to-make-an-empty-cells-border-appear/5172978 "CSS to make an empty cell's border appear?") discussing the same issue. With full credit to the answers given there, I am summarizing the potential solutions here.

Firstly, on the server-side, add an `&nbsp;` inside all empty `<td>` elements. For a client-side jQuery solution, this can be done using&hellip;

{% highlight javascript %}
jQuery("td:empty").html("&nbsp;");
{% endhighlight %}

Note: `&nbsp;` has issues with screen&ndash;readers, so using a&hellip;

{% highlight html %}
<span style="zoom: 1"></span>
{% endhighlight %}

&hellip; is also suggested.

An alternate solution is to add these two attributes&hellip;

* [`frame="box"`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/table#attr-frame)
* [`rules="all"`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/table#attr-rules)

&hellip; on the `<table>` element.

In addition to the above solutions, removing the void between two `<td>` elements might also help. You can find a clean workaround by Harry Roberts ([CSSWizardy.com](http://csswizardry.com)) where he suggests to use [empty HTML comments](https://github.com/csswizardry/csswizardry-grids/wiki#classes-in-markup) to fill the void.

Hopefully, this should help resolve the issue.
