---
title: "a little contribution"
date: 2024-04-24T10:09:34-04:00
draft: false
---

Howdy. Lately I've been experimenting with switching the electron based software I use with versions that use system-wide electron rather than a bundled version. One of these programs being VSCodium. I like to use VSCodium as it has all of the telemetry nonsense disabled, but I also like to use the official VSCode marketplace and enable features such as syncing settings through my GitHub account.

There are patches on the AUR to enable these features on almost every version of VSCodium available, but none were compatible with the [vscodium-electron](https://aur.archlinux.org/packages/vscodium-electron) package that I've recently been trying out. As a result I took it upon myself to submit my first 2 packages to the AUR. They're farily basic forks of the [vscodium-bin-features](https://aur.archlinux.org/packages/vscodium-bin-features) and [vscodium-bin-marketplace](https://aur.archlinux.org/packages/vscodium-bin-marketplace) patches, creatively titled [vscodium-electron-features](https://aur.archlinux.org/packages/vscodium-electron-features) and [vscodium-electron-marketplace](https://aur.archlinux.org/packages/vscodium-electron-marketplace).

The changes were pretty simple. The main difference is just the install location. The vscodium-bin package gets installed to /opt/vscodium-bin, while vscodium-electron is installed to /usr/lib/vscodium. There was one other change I had to make. I didn't check EVERY vscodium-*-features/marketplace patch on the AUR, but from what I can tell the product.json that gets patched is usually located in "resources/app" but this does not exist with how vscodium-electron is compiled, and as a result the product.json is in the main install folder. Nothing too crazy.

So yeah, a little bit of time and some help from the Arch Wiki on submitting to the AUR, now people using the [vscodium-electron](https://aur.archlinux.org/packages/vscodium-electron) package can now easily access the features and marketplace from the proprietary build of VSCode without modifying anything themselves. Might just be something small, but I feel happy with my contribution and hope others find it useful.