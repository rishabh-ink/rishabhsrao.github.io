---
layout: post
title: "Deleting the node_modules folder in Windows"
date: 2015-02-16 23:58:00
comments: true
categories: tech
tags: [windows, node, nodejs, robocopy]
excerpt: Having trouble deleting the `node_modules` folder?
---
Windows has a file path limit of 260 characters. You can [read more](http://stackoverflow.com/questions/1880321/why-does-the-260-character-path-length-limit-exist-in-windows) about it. The other day, I was trying to delete the `node_modules` folder on Windows, when it threw an error saying that Windows cannot perform the delete operation because the path is too long.

After searching the web, I found that PowerShell's `robocopy` command can indeed handle long paths. So, here's what I did:

```
mkdir empty_folder
robocopy empty_folder node_modules /s /mir
rmdir empty_folder
rmdir node_modules
```

In essence, you create an empty folder and mirror it recursively over the `node_modules` folder.
