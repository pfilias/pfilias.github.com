---
layout: post
title: iPhone 4S Upgrade Woes RE: photos
date: 2011-10-17 11:22
comments: true
categories: []
---
I installed iOS 5 on my iPhone 4 about a <em>week earlier</em> than the Oct. 12th release date. <strong>Loved it.</strong> Used the new album creation (like tagging really) to make a bunch of "albums" that made it easy. I digress. Anyway, I picked up my 4S on Friday. I took one last backup of my iPhone 4 at 835am EST on Friday.

I restored the 4S from the backup taken at 835am.

Later in the day, I noticed my Camera Roll <strong>was empty</strong> (well, it had 4 photos I took with the new phone to test the camera's optics). <strong>NOTE: I DO NOT have iTunes set to sync my photos on the phone with anything on my computer.</strong> I just grab photos from my iPhone from time to time with either Windows' native importer (into Live Photo Gallery) or Picasa or even Lightroom.

I tried to restore my phone again from the iPhone 4 backup, but it didn't exist. I thought I'd try to make a backup of my 4S, just to see if it would end up showing all backups. iTunes only showed my iPhone 4S' backup.

I started looking through my phone and noticed that its last iCloud backup was about 1.8GB in size. When I showed its details, I noticed that it had 1.5GB of photos. Crazy!!?!?!?!? I did a little more digging and found out where iTunes stores its backup files (for Windows Vista/7) here: C:\Users\_______\AppData\Roaming\Apple Computer\MobileSync. There were 8400 files here, none with an extension.

I copied all of those files to a new folder and appended .jpg to their filenames. What this did was show me which of these were photos. <strong>Take note:</strong> There will be JPG files here from your phone's app and browser cache, but you can have Windows (or a 3rd party app like Picasa) display the photos sorted by their dimension. This way, you can see the photos you took with the phone's camera which are something like 2592x1936 (taken on an iPhone 4) in resolution. Icons from apps and the web will be smaller, like 320x240, and similarly small in resolution.

<!-- copy and paste. Modify height and width if desired. --> <a href="http://content.screencast.com/users/pfilias/folders/Snagit/media/17978748-7bc4-4b8b-999f-236080ff5ec6/10.17.2011-11.21.24.png"><img class="embeddedObject" src="http://content.screencast.com/users/pfilias/folders/Snagit/media/17978748-7bc4-4b8b-999f-236080ff5ec6/10.17.2011-11.21.24.png" width="561" height="209" border="0" /></a>
The files will look like this. The highlighted file, when copied to a new folder and adding the .jpg at the end, does in fact show up as a photo!

So, at this point, <strong>my photos have been saved</strong>, but they are not back on my camera, not in their own folder/album, and not in my camera roll, where I really want them to be.

In my digging, I also found <a href="http://iphonebackupextractor">iPhone Backup Extractor</a>. This is a clever piece of software that goes into your iOS device's backup on your computer and lets you extract out specific items, like photos, for example. <em>I AM NOT ENDORSING THIS</em>. I only tried the unregistered version, which would only pull out <strong>2 items per extract</strong>. Since I was able to manually get to my photos, I ended up not buying this app. It does look VERY useful and helpful though. Something to consider having in my IT toolbox (yep, I'm that guy...the one who helps their family and friends).
