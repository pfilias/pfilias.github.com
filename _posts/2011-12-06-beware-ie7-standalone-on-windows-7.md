---
layout: post
title: Beware IE7 Standalone on Windows 7!!
date: 2011-12-06 21:59
comments: true
categories: []
---
So, I wanted to test something at work using IE7 as a <a href="http://www.google.com/url?sa=t&amp;rct=j&amp;q=ie7%20standalone&amp;source=web&amp;cd=2&amp;ved=0CDEQFjAB&amp;url=http%3A%2F%2Fie7-standalone.en.softonic.com%2F&amp;ei=DpDeTvecOMWrgwf88MDVBQ&amp;usg=AFQjCNGt5lJ1vaj-l-DgCbLbTY1SC-QZRg">standalone app</a> since you can't have multiple versions of it running in Windows (we'll get to this later). I had previously been using IE7 Standalone on Windows XP and loved it. I had no idea it would hose some file registrations in Windows 7.

Luckily for me, there was an <a href="http://pyrocam.com/re-register-all-dlls-to-fix-no-such-interface-supported-error-in-windows-7-after-installing-ie7-standalone/">exact post/article</a> that led me to a fix. Thanks pyrocam.com!

I did run into a few hangups while running through the registration batch file, having to kill regsvr32.exe a few times, but who cares. I can now go back into explorer.exe and right-click Computer.
