---
layout: post
title: "ASP.NET MVC 5 Tips and Tricks"
date: 2015-09-28 00:09:00
comments: true
categories: tech
tags: [asp.net, mvc, razor]
excerpt: Some random tips that I've found useful while working with ASP.NET MVC 5.
---
Here're a bunch of random tips that I've found useful while working with ASP.NET MVC 5:

* Use the `OutputCache` action filter to cache the output.
* Use the `HandleError` action filter for error pages.
* Use `@Styles.Render(...)` and `@Scripts.Render(...)` to render `<link>` and `<script>` tags.
* Use `@RenderSection(“name”, required: false)` instead of `@if(IsSectionDefined(“name”)) { ... }`.
* Use `@Html.AntiForgeryToken` and `ValidateAntiForgeryToken` action filter to avoid [CSRF](https://www.owasp.org/index.php/Cross-Site_Request_Forgery_(CSRF)) attacks.
* `@Html.Partial()`'s second argument can contain "template" data.
* Use `BundleTable.EnableOptimization = true` for cache busting and minification. See `App_Start/BundleConfig.cs`.
* `ScriptBundle` and `StyleBundle` can also `.Include` CDN paths.
* `_ViewStart.cshtml` is used to specify common properties across all views.
