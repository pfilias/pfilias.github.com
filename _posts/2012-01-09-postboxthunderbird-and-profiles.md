---
layout: post
title: Postbox/Thunderbird and profiles
date: 2012-01-09 13:11
comments: true
categories: []
---
So, I recently went through an exercise where I archived old mail in my <a href="http://www.gmail.com">GMail</a> account. My inbox was ENORMOUS, like 80000+ emails. In doing this archiving, it seems that <a href="http://www.postbox-inc.com/">Postbox</a> (an e-mail client based on <a href="http://www.mozilla.org/en-US/thunderbird/">Thunderbird</a> that costs $29.95. Seems expensive when most e-mail clients are free (come with your OS), or webmail systems do what most people need. I got into Postbox early on, so I stuck with 'em. Anyway, Postbox wouldn' t get out of a Not Responding state after I did this archive, probably because the inbox was out of sync with what was on the server.

Nevertheless, I butchered my profile on the machine, at which point, Postbox wouldn't even LAUNCH, saying that Postbox was already running. It seems that you shouldn't go into your AppData/Roaming folder and delete your profile folder. Rather, you should use the <a href="http://support.postbox-inc.com/entries/81707-the-postbox-profile-manager">Profile Manager</a> to make these changes. So, I went into Postbox's Profile Manager (same as Thunderbird) and deleted the default profile and created a new one. Right after that, Postbox didn't complain about running already and all was well in the world of Peter's e-mail.
