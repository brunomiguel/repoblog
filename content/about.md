---
title: "About"
description: "Updates and highlights about userrepository, a mostly AUR-based binary repository for Arch and Arch-based distributions"
date: "2021-06-30"
draft: false
aliases:
  - "about-us"
  - "contact"
author: "Bruno Miguel"
#menu:
#  about:
#    name: About
#    title: About
#    url: /about
#    weight: 1
#  subpage:
#    parent: about
#    name: Subpage
#    title: Subpage
#    url: /about/subpage
#    weight: 10
---

This is the blog for the binary repository for Arch / Arch-based Linux distributions. Here, you can read the latest news about the repo and whatever Arch-based subject I might write, and know the latest highlighted package.

## Enable the repository

Create the file <mark>`/etc/pacman.d/userrepository`</mark> and add:

{{< highlight ini >}}
Server = https://userrepository.eu
SigLevel = Optional TrustAll
{{< /highlight >}}

Now, edit <mark>`/etc/pacman.conf`</mark> and put in it the following content:

{{< highlight ini >}}
[userrepository]
Include = /etc/pacman.d/userrepository
{{< /highlight >}}

The last step is running pacman:

{{< highlight sh >}}
sudo pacman -Syu
{{< /highlight >}}

## List all packages from the repo

To list all the packages from the repository, you must first enable it with the above steps. After that, run:

{{< highlight sh >}}
sudo pacman -Sl userrepository
{{< /highlight >}}


