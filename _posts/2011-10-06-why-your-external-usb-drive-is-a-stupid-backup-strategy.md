---
layout: post
title: Why your external USB drive is a stupid backup strategy
---

Physical harddrives fail. They fail a lot. In the last ten years I've lost at least four drives. (Three of mine where IBM Deskstars - not good)

Fortunately, all of my drives were part of a mirror set, so I never actually lost any data. I think the last time I lost data was about 12 years ago when I coded a poorly thought out shell script to rename a number of files. I ended up with one file after running that. Oops! (I'm not counting not being able to find stuff. I once needed to find some code for a client, but had to have access to the physical drives I'd taken out of my old server for that. I managed to find an okay version of the code. Shame I wasn't using bitbucket or github back then!)

Anyway, today I get asked by a friend to look at her USB drive which isn't appearing as a drive on windows. I can see that the USB device is connected, but the drive itself is asking to be initialised if I look at it with Drive Manager. And diskpart just fails when I try and get any details.

Next step is to remove it from the USB case and try it in one of my machines, but the failure of this drive got me thinking. I know a lot of people who use an USB drive to store their stuff on. And not just as a backup - it's their main storage facility. Which is okay, but only if you don't mind losing everything on it.

If you've got a few files you don't want to lose (less than a couple of Gig's worth), I'd recommend something like Dropbox, Google Drive or even Microsofts Live Mesh. But if you've got half a terabyte of photos and videos, then at a minimum get a second drive and make sure they're backed up on that. At least then, when one fails you've got the other around to make a copy of.

Even better would be a little NAS drive. Can be as simple as a mirror-set (RAID 
-1 which is two drives that automatically keep a copy of each other) or as complex as RAID-6/RAID1+0 (which involves parts of files shared across many drives or a combination mirro/stripe configuration). You'll need to do some reading to figure out what is most appropriate for your situation though.

Also don't be fooled into thinking that if you've got RAID-5 that your data is safe. With drives getting larger than a couple of terabytes, it's statistically likely that you'll lose data even with a RAID-5 array in event of one disk failing. If you are buying a NAS device, look for it supporting one of either RAID-1+0 (otherwise called RAID-10) or RAID-6.

But two things to remember;
1. Physical drives always fail, and...
2. your backup is only as good as your last restore.