---
title: Switching from Mac OS to linux
layout: post
---

After six years of being OS X / Mac OS based at work, I've recently switched to Linux. The motivations were several:

* I haven't been happy with the direction Apple has been taking with their professional laptop hardware in the last few years. The newer 13" Macbook Pros are pretty conservative on specs (the retina screens basically haven't improved resolution since 2012, and they haven't adopted 8th generation Intel processors yet) and odd design choices (the touchbar, limiting ports).
* The philosophical difference between using a highly opinionated walled garden like the Apple ecosystem versus a more open platform like Linux. My career has been made on open source software and if I can pull off a Linux work laptop and still be productive, I would like to do that.
* We deploy everything at work to Linux and so it would be better alignment betwen the dev environment and the deployment environment.

I actually waffled with this issue for about _two years_, which is why I am still using my late 2012 13" Macbook Pro Retina. Now the fact that this machine is still my workhorse is a testament to how nice a machine it is. The Retina display was revolutionary for the time: 2560 x 1600 resolution, with built-in 2x scaling by default. 16GB memory, 256GB SSD drive. Lots of useful ports (HDMI, USB3, Thunderbolt, SD card). All-day battery life. I really love the hardware. OS X / MacOS was fine, I was never in love with it but it's fine.

Nevertheless, it is finally starting to feel its age. Things are starting to be noticeably slower. It's starting to feel heavier in the bag, too. :-) This spring I finally decided I was going to try something new, and I started researching alternatives.

# Choosing the Right Laptop and Vendor

My hardware requirements:

* 13" laptop. I'm schlepping to meetings all day long, and commuting on a bike. I want portability.
* A vendor that supports Linux. As my work laptop, I need it to work. I'm no stranger to futzing with Linux - I've been using it since 1994 - but I don't need that hassle to be in the way of me getting my work done.
* 512GB SSD, because I am constantly running out of space on my 256GB one.
* 16GB memory minimum.
* Good support for virtualization. Every once in a while, I need to dip into Windows world for work. Plus, it's sometimes useful to have VMs around to mimic certain environments. This mainly affects memory and processor choices.
* All-day battery life. Pulling out my adapter and finding an outlet during the workday ranges from slightly annoying (in conference rooms at the office or coffee shop) to dang near impossible (in the airport or at a conference).

With that, I set out to research vendors. I quickly got down to two: Dell and System76. I was intrigued by System76 as one of the best-known Linux-specific laptop vendors. They offer a wide range of pretty good hardware options, but the weakest part of their lineup is on the small end, where I needed to be shopping. Their 13" option (the Galago Pro) has comically bad battery life (reports are around 2.5 hours), so they were ruled out. Shame too, because they had the best ports setup on their laptops, and I like the idea behind the company. There are other linux-specific vendors out there but they all feel less established than System76, to the point where I'm not sure I'd be comfortable committing work funds to them.

Then we have Dell. Their 13" XPS Developer Edition ships with Ubuntu and has impressive specs. They've been doing this for several years now, and the XPS often gets named as best linux laptop. The form factor is ultra portable - it looks more like an 11" laptop thanks to their tiny bezel and 16:9 aspect ratio. It's noticeably smaller than my MBP. It's not perfect - the ports are limited, for one - and it's certainly not cheap, and Ubuntu isn't everyone's favorite Linux distribution, but overall it was the best option for me.

So, I ordered a Dell XPS 13" 9370 Developer Edition with an Intel Core i7, 16GB RAM, a 512GB SSD, and a UHD touchscreen (3840x2160).

# Making the Switch: Getting Set Up

Switching to a Linux desktop still isn't for the faint of heart. Linux advocates tend to understate the knowledge and work required to really make Linux your everyday computing environment. As I said before, I've been working with Linux for 25 years now, and I'm a huge Linux fan, but part of the reason I sat on this decision for 2+ years is because I know it's not going to be an out-of-the-box experience.

I had a minimally usable system out of the box, in that I could get online and use a browser, which is really a good chunk of my work these days. But I still spent a lot of time over the next few days getting the system into shape for full duty.

I've [written elsewhere]({% post_url 2018-06-16-xps-9370-ubuntu-16.04-notes %}) in some depth the specific setup issues I encountered. My overall summary would be: it's not terrible and if you're familiar with Linux you can manage it, but even from a vendor that officially supports Linux, there were plenty of required tweaks.

# Software Solutions and Alternatives

My biggest concern about the switch was whether or not I was going to have good solutions for the critical software and workflows I rely upon every day to get my job done. I really wanted to find a way to be 100% Linux native and not rely on a Windows VM for anything if possible.

Here are the software things I depend on today, and which will need Linux versions or alternatives:
* Browser. I'm all Chrome all the time under Mac OS. However, with Firefox showing signs of a comeback and Chrome becoming increasingly bloated, I'm going to try to use this switch as an oppotunity to switch to Firefox for my daily browser, as well.
* Google Drive
* Lastpass.
* Slack.
* Evernote.
* Microsoft Office.
* Spotify.
* Atom.
* Terminal.
