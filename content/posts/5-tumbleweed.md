---
title: "from arch to tumbleweed - first impressions"
date: 2023-08-10T10:25:21-04:00
draft: false
---

After Arch/Endeavour being my goto distro for a decade due to wanting a rolling release system, I decided to check out my other options. Arch is great, I love the AUR, but troubleshooting issues after updates can suck. It didn't happen too often for me, but when it did it was always a headache. I like tinkering but I'd rather tinker with things of my choice, not a possible issue that could result in me having to reinstall my OS, albeit due to incompetence on my part.

Prior to Arch I dipped my toes into Linux by Ubuntu and later on other .deb based distros, such as CrunchBang and others I can't remember at this point. I switched to Arch after getting tired of having to reinstall my OS every 6 months or deal with, at the time, possibly install breaking dist-upgrades. Never touched an rpm based distro, but I've read many good things about openSUSE Tumbleweed, and after doing a bit of research the past few days I decided to give it a shot as my daily driver. I formatted my laptop and installed it last night.

The official docs are great. They're very detailed and anytime I got hung up or confused about something there was always an answer readily available. The installer was very easy to use but also very customizable. Almost every setup step had an option to modify the settings more than the basic options. What I enjoyed was being able to customize what packages to install. Many of my goto programs were available in the official repos which helped reduce my post install setup.

Speaking of, booting into the system, initial impressions were very nice. Being used to the default EndeavourOS, I was surprised at how polished things were out of the box. The graphical boot screen surprised me due to being used to just seeing the verbose boot output from Arch, but I should have expecting it seeing as this is a stable version of the development branch of openSUSE.

Choosing KDE, the Plasma loading screen was also a surprise. I thought it looked pretty neat honestly. The gecko instead of the Plasma icon as the applications button was cute too.

Installing programs I wanted that weren't in the official repos was pretty easy. The docs gave easy instructions on adding popular third party repos, which let me grab a few more programs I couldn't get on the official ones. For the software I wanted that wasn't in those repos, it was as easy as installing the flatpak versions. I haven't yet installed anything from the openSUSE Build Service, but I have checked out the site and it does seem like it's a very cool alternative to the AUR. I'll definitely be looking into it more because I likely will run into software I can't find in the repos I have currently.

The guides had a section for Nvidia drivers, which I needed as I have a dual GPU laptop. Integrated Intel, dedicated Nvidia. To my surprise, the guide was a bit outdated as I didn't have to do anything manually. As soon as I opened the YaST package manager and it synced the repos, it asked me if I wanted to add the Nvidia repos and install the drivers, which it did automatically after I accepted Nvidia's licence agreement.

Setting up prime took a bit of research. The suse-prime package provided a way to switch and set defaults between nvidia, intel, and prime offloading options. I set it to use offloading at boot, and switched my session over to offloading, but now I had a problem. I relied on the prime-run command from the nvidia-prime package on Arch. Luckily, that's just a shell script. A quick search led to a guide on how to easily create that same file and make prime offloading a breeze.

So here I am, pretty much back to the state of how my Arch install was. Now to actually daily drive it for a bit and see what issues I run into and how easy I find it installing packages from outside of the official repos. So far though, I'm enjoying Tumbleweed a lot. I bought into the "rolling release but stable" hype, time to see if that stands the test of time. Initially though, I'm optimistic.