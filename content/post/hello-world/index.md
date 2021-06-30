+++
author = "Bruno Miguel"
title = "Hello World"
date = "2021-06-30"
description = "I am very delighted to finally announce the userrepository blog."
tags = [
    "userrepository",
    "news",
    "upcoming",
]
categories = [
    "news",
]
favorite = false
draft = false
disableSummary = true
+++

I am delighted to **finally** announce the availability of the **userrepository blog**!

Launching a blog for the repository was something I was considering for over six months. However, due to personal circumstances and, well, life, the idea got put in a drawer. That was only until the 29th of June 2021, when I started dabbling with static site generators.

## The toolkit

After a bit of fussing, I chose **[Hugo](https://gohugo.io/) as the generator.** Hugo was my choice as the generator because I was already familiar with it, and it feels accessible for a non-dev like me.

**[Anubis](https://github.com/mitrichius/hugo-theme-anubis) was my theme choice to build upon my own.** The original theme is under the [MIT license](https://github.com/Mitrichius/hugo-theme-anubis/blob/master/LICENSE) and so is my fork of Anubis.

The source code for this blog is available at [Github](https://github.com/brunomiguel/userrepository-blog). You are welcome to fork it, make PRs and report issues.

## What the blog will cover

I will **write about the occasional update about the repo**. These blog posts can include, among other subjects, new packages, changes to the build system, scheduled reboots, etc.

**Featured packages** will be another type of blog post published. I will highlight an available package on the repo that I feel will bring value to its users.

Comments about changes to / news regarding [Arch Linux](https://archlinux.org/), quick tips and screenshots for the VM running the repository will also be found on the occasion.

## Screenshots

Speaking of VM screenshots, here are two:

[![first screenshot](../../hello-world/vm1.jpg)](../../hello-world/vm1.jpg)

[![second screenshot](../../hello-world/vm2.jpg)](../../hello-world/vm2.jpg)

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