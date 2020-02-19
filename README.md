# Getting Started With Hackintoshes

**Read this before posting**

## How to get started

Well here on r/hackintosh we have a couple requirements from users before posting:
* Search before posting
* Read the sidebar (About section on mobile)
* Read the [FAQ](https://www.reddit.com/r/hackintosh/wiki/faq)
* Read the rules
* Follow posting format

Problem is many of the visitors here are on mobile where the sidebar is obscured and difficult to find, so this post will be a starting point for new users. **This is not a substitute for the other resources**

So how do you actually get started? Well few things:
* Knowing **if** your hardware is compatible
* Finding a guide that is right for you
* ~~Consume 2L of Green Apple Vodka before starting~~
* Read FAQ, rules and posting format before posting questions

## Hardware Compatibility

Bascially every question about hardware compatibilty is answered in our FAQ and sidebar:

* [Basic Compatibility Guide - FAQ](https://www.reddit.com/r/hackintosh/wiki/faq#wiki_ok.21_i_fulfil_some_points.2C_what_now.3F)
   * Extensive list on hardware compatibility
* [Anti-Hackintosh Buyers Guide](https://khronokernel-5.gitbook.io/anti-hackintosh-buyers-guide/)
   * Extensive list on what doesn't work or should be avoded
* [Wireless Buyers Guide](https://khronokernel-7.gitbook.io/wireless-buyers-guide/)
   * Extensive list on supported Wireless cards
* [GPU Buyers Guide](https://khronokernel-3.gitbook.io/catalina-gpu-buyers-guide/)
   * Extensive list on supported GPUs

Don't know how to check what hardware you have? [Speccy](https://www.ccleaner.com/speccy) is a great tool to find most of the important info, but manufactuer's website will be the most detailed in most instances

## Install Guides

We have a plentiful amount of guides to choose from:

**Intel Desktops**:
* [r/hackintosh Vanilla Guide](https://hackintosh.gitbook.io/-r-hackintosh-vanilla-desktop-guide/)
   * For windows and Linux support, pair this guide with the [Internet Recovery Guide](https://internet-install.gitbook.io/macos-internet-install/)
* [OpenCore Vanilla Desktop Guide](https://khronokernel-2.gitbook.io/opencore-vanilla-desktop-guide/)
   * macOS and Windows support already included

**Intel Laptops**:
* [The Vanilla Laptop Guide](https://fewtarius.gitbook.io/laptopguide/)
   * For windows and Linux support, pair this guide with the [Internet Recovery Guide](https://internet-install.gitbook.io/macos-internet-install/)
* [OpenCore Laptop Guide](https://1revenger1.gitbook.io/laptop-guide/)

With laptops, we generally recommend going Clover first as there's a lot more work involved currently with laptop support on OpenCore.

**AMD Desktops**:
* [OpenCore Vanilla Desktop Guide](https://khronokernel-2.gitbook.io/opencore-vanilla-desktop-guide/)
   * macOS and Windows support already included
   * Clover support has been deprecated on AMD, for older versions of macOS see the [AMD Vanilla guide](https://vanilla.amd-osx.com/)
   
**Deprecated guide**:

* [Original Vanilla Guide](https://www.reddit.com/r/hackintosh/comments/68p1e2/ramblings_of_a_hackintosher_a_sorta_brief_vanilla/)
* [AMD OSX Vanilla](https://vanilla.amd-osx.com/)
* [Rehaman's Laptop guide](https://www.tonymacx86.com/threads/guide-booting-the-os-x-installer-on-laptops-with-clover.148093/)


## But wait a minuite, what the hell is the difference between OpenCore and the other guides? 

Well with hackintoshes we're currently in the middle of a transition period between 2 boot loaders, OpenCore and Clover. Clover is what most guides online are based off of, but the new shiny toy is OpenCore. So what are the differences and which should you choose for your next build?

* OpenCore requires more work to setup, though easier to maintain and is much more likely to survive updates. This is thanks to being much more "Mac-like" compared to its predecessors
* Clover is generally easier to setup, but is much more likely to break with even simple secuirty updates. This is due to a heavily outdated form of kext injection which should've been killed in OS X 10.7. Understand that support will not last forever, and to even maintain support currently requires a lot of hacks
* Much better overal secuirty and better compatibility with newer hardware on OpenCore(many Z390 and X299 boards are unbootable on clover, and features like FileVault work much better on OpenCore with Apple Secureboot feature coming soon)
* Better laptop support on Clover as many autopatches are availible, with Opencore you need to run external programs such as [SSDTTime](https://github.com/corpnewt/SSDTTime) and put a bit more effort into understanding what you're trying to do
* More info online for Clover as its been aroud much longer(but also a lot of outdated or outright false info as well), though Opencore Guide's [troubelshooting page](https://khronokernel-2.gitbook.io/opencore-vanilla-desktop-guide/troubleshooting/troubleshooting) has made this much easier
* Future AMD CPU support is directly tied to OpenCore as [AMD OSX](https://amd-osx.com) will not be updating patches for Clover. 10.15.1 is the highest supported OS on Clover while OpenCore supports all versions of it including betas.

##  FAQ, Rules and Posting Format

Before asking any questions, we **highly encourage you to read the [FAQ](https://www.reddit.com/r/hackintosh/wiki/faq)**. It contains ***tons*** of information regarding compatibility, requirements, guides, more guides, and even more guides, etc. 

And for Opencore users, there's an extensive [troubleshooting page](https://khronokernel-2.gitbook.io/opencore-vanilla-desktop-guide/troubleshooting/troubleshooting) that covers most issues, with a [OpenCore reference manual](https://github.com/acidanthera/OpenCorePkg/blob/master/Docs/Configuration.pdf) for the engineers in the audience.

And if your questions are still not answered even after a google search, then you're ready to post. Main things to keep in mind:

**Rules**:
* **No profanity**
   * Don't need to really explain, just treat others with repect
* **No links to torrents of P2P of copyright material**
   * For legal reason, we'd like to avoid this
* **Questions Must Have Adequate Information**
   * See posting format below
* **Search Before Posting**
   * We try to avoid having the same question repeated over and over as this clutters the subreddit
* **No distro/beast tools**
   * Don't support tools such as Uni/Multibeast, Niresh, they're harmful and difficult to debug. More info here: [Tonymacx86 Stance](https://github.com/khronokernel/Tonymcx86-stance)
* **No self-promotion**
   * This is a community to learn, not a pay for hack service. Keep talks like that in DMs
* **No Mac posts**
   * This subreddit is meant for non-Apple hardware running macOS, please keep Mac hardware talks in their repective subreddit
   
**Posting Format**

```
CPU:
GPU:
RAM:
Motherboard/Laptop model:
Audio Codec:
Ethernet Card:
Wifi/BT Card: (if available)
What guide/tool followed: [Links and/or names, links preferably]
What part I got an issue with: [Describe your issue WITH pictures attached if possible]
What files/config I am using: [Link to cloud host preferable, don't post the entire config in your post]
Extra Info: [Add something you need to point out about your setup]
```

And reminder, **be as specific as possible in your post**. Please don't say "hack machine borked, how fix" with no other info. This community does want to help you but please try to think from the other perspective of how the helper would feel. It also means users ho had similar issues will be able to throw their 2 cents in.

We also have discord servers to ask help in, same rules apply there so don't think you can get off easy there:

* [r/Hackintosh Paradise](https://discord.gg/Wxam8aH)(Main server, primarily Intel)
* [AMD OSX Server](https://discord.gg/qudxDed)(Primarily AMD)
