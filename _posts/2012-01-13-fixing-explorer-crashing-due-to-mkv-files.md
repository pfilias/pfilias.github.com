---
layout: post
title: Fixing Explorer crashing due to MKV files
date: 2012-01-13 08:24
comments: true
categories: []
---
Could I have finally found the solution to my problem that has been plaguing me ever since I started messing around with MKV files? It seems that traversing around my filesystem, in folders that have an abundance of MKV files, my explorer.exe would crash, at least 66% of the time. I've tried disabling thumbnails for certain folders, and all folders. NO LUCK. I've tried installing the <a title="K-Lite Codec Pack x64" href="http://www.free-codecs.com/download/K-Lite_Codec_Pack_64-bit.htm">K-Lite Codec Pack</a> that others have mentioned would fix this problem. NO LUCK. Today, I stumbled upon <a href="http://www.nirsoft.net/utils/shexview.html">ShellExView</a>, after someone mentioned that the <a href="http://shellfix.nirsoft.net/fix_shell_problem.html?id=200&amp;dll=DivXThumbnailProvider.dll">DivX Thumbnail Provider</a> was the culprit.

First attempt at opening one of my MKV folders was a success. Let's hope this persists. Thanks NirSoft!
