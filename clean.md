# Spring Cleaning

## Getting Your Machine Back to Square One

Every year, I wipe my MacBook hard drive completely + install a fresh copy of the latest operating system (currently Yosemite). Whether this is obsessive compulsive or a byproduct of being organized + focused remains unclear. I have found this not only helps remove clutter (digitally + mentally), but is also extremely motivating like a new year (or week). The key is to do it quickly + properly, so I am going to share my notes on how to prepare, mitigate side effects, back everything up, and re-install the essentials.

## Prepare

First, let’s think about + be very explicit about what we want to accomplish. Here are some initial questions that will inform our process:

1. Which essential files + settings do we need to make sure to restore after the wipe?
2. Which files can we permanently store in our backup for archival purposes, but not worry about restoring after the wipe?
3. What can we store in the cloud to make restoring easier + more reliable next time?
4. What can we delete to shrink the size of our backup + save time?
5. What tools do we need?
6. How do we do this all at once so we don’t block ourselves from being able to use our computer?

The answers to these questions will be a little different for everyone, but they serve as the format we will follow to explicitly define our goals.

If you need to get this done ASAP, you can reliably skip to [step 4](#user-content-the-wipe).

### 1. List the Essentials

Our first step is to list each essential app, document + settings you want to restore after the wipe. Hopefully, all of your apps are in `/Applications` all your documents are in `/Documents`

Passwords, browsing history, fonts

[Use iCloud Keychain](https://support.apple.com/en-us/HT204085) to sync all of your accounts + passwords for Calendar, Contacts, Mail, Messages, Wi-Fi, Facebook, and Twitter.

### Assumptions

With this step, there is an underlying assumption that there are many apps on your machine that you needed at one point. As a benchmark, only include apps you currently use on a regular basis. For me, my essentials are the following:

- TODO: still gotta do this

## 2. Delete large files

Use Finder to find the largest files (100MB+) on your current hard drive + determine whether it’s safe to delete these things. Usually these are things you downloaded and needed at one time but no longer need. This will make your back up go way faster!

## 3. Move things to the cloud

### Free ways to back up your shit

Code -> Github.com (unlimited public projects)
Documents + Media -> Google Drive 15GB free ($2/mo. for 100GB)
Photos -> Dropbox [5GB free](https://www.dropbox.com/en/help/287) ($99/yr. for 1TB)

## The Wipe

All of the previous steps may be completed *after* you have verified you have a bootable snapshot of your current hard drive on your external drive, so feel free to start here if you are in a hurry.

### What do you need?

- External hard drive larger than current hard drive usage
- [Download Yosemite from the Mac App store](https://itunes.apple.com/WebObjects/MZStore.woa/wa/viewSoftware?id=915041082&mt=12&ls=1)
- [Download Carbon Copy Cloner](https://www.bombich.com/software/download_ccc.php)

### The process

1. Use Disk Utility to create 3 partitions: 1 for the Yosemite installer, 1 that exceeds the size of your current drive **usage** by 10GB, and 1 for leftover space on the external drive
2. [Follow this tutorial](http://www.macworld.com/article/2367748/how-to-make-a-bootable-os-x-10-10-yosemite-install-drive.html) to create a bootable Yosemite installer on the first partition
3. Use Carbon Copy Cloner to back up your hardrive to the second partion (this will take a few hours; I leave mine running overnight then finish in the morning)
4. Boot into the Yosemite installer to wipe the hard drive (make sure you’re wiping your machine hard drive + not the backup you just created on your external)
5. Install Yosemite to clean hard drive on your machine
