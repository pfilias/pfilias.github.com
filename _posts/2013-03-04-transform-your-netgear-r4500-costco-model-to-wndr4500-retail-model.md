---
layout: post
title: Transform your Netgear R4500 (Costco model) to WNDR4500 (retail model)
date: 2013-03-04 11:45
comments: true
categories: []
---
So, in preparation for moving, I bought a new router since I needed to have both households up and online while we had a 10 day transition period, or so.

One of the features I was looking for in buying a router for this was being able to turn my Brother multifunction printer into one that was AirPrint compatible, something my household lacked. The Netgear R4500 that was for sale (may still be) at Costco seemed to fit the bill. It was both cheap, $130-$140, and available (in the store).

When I hooked it up and followed the directions to get the printer set up to be AirPrint compatible, it failed. It didn't show up when trying to find it on my iPhone 5. Bummer, I thought. After doing some research, I found that the Costco model of this router had a different boardid that didn't allow it to get firmware updates from Netgear nor could it load firmware updates that were manually downloaded. I had a suspicion that this was the cause of this ReadyShare printer funny-business. I let it slide, as I had a lot of other things to deal with in this new house.

Fast forward about a month, and I re-investigated the notion of hacking the router to set its boardid so that it was, indeed, a retail version of this Netgear router, the WNDR4500. I followed the <a href="http://www.youtube.com/watch?v=Evv2pnfgXy4" target="_blank">YouTube video</a> instructions on how to do this.

To do this, you'll need the MAC address of your router. You can find this MAC address by looking at your router in the web interface, or by typing "arp -a" in a command prompt. These routers seem to start with 84.

You'll also need the <a href="http://www.myopenrouter.com/download/10602/NETGEAR-Telnet-Enable-Utility/" target="_blank">telnetenable.exe file</a> which can be found at myopenrouter.net. The directions you see in the Word document that comes with that download and in the YouTube video threw me off for a second. It has you use the login Gearguy and the password Geardog when using the telnetenable command prompt utility. At first, I was using my own web interface router login and password and it wasn't working. I re-read some info online and found that the username and password were set up by folks at Netgear to give developers access to be able to telnet into their routers for various reasons.

After you do the boardid change for your router, you'll need to download and install the firmware from Netgear for it to reflect it's now the WNDR4500 and not the R4500.

Crazy thing is, after I did this, I went back into my router's setting via the web interface and navigated to the ReadyShare Printer setup, selected my printer in the list of printers, and voila, my printer was now seen by my iPhone. All is well in Computer Ninja's house now!

NOTE: Netgear's documentation states you need to have the printer hooked up to your router with a USB cable. This isn't true. As long as the printer is part of your network, the ReadyShare printer functionality within the firmware will work!

To recap:

1. Find your router's MAC address with "arp -a" from a command prompt or the web interface. Should start with 84.

2. Download the <a href="http://www.myopenrouter.com/download/10602/NETGEAR-Telnet-Enable-Utility/" target="_blank">telnetenable.exe</a> program and extract it so you can run it from a command prompt.

3. From where you have it, you'll need to run it like this: telnetenable 192.1681.1 (unless yours is different) 84xxxxxxxxxx Gearguy Geardog

4. Telnet into your router: telnet 192.168.1.1 (if you don't have Telnet, you'll need to go into Control Panel &gt; Programs &gt; Turn on Windows Features &gt; Click Telnet

5. Once you successfully telnet, you'll get a prompt that has a #. From this, you'll need to enter this: burnboardid U12H189T00_NETGEAR

6. Reboot your router

7. Download and install the firmware you want from Netgear's website

8. Reboot your router. It'll now be listed as a WNDR4500 and you'll be able to use the web interface to do firmware updates!!
