+++
author = "Bruno Miguel"
title = "Featured package: emptty-git"
date = "2021-07-11"
description = "emptty-git is a blazing fast Display Manager on TTY"
tags = [
    "featured",
    "emptty-git",
    "display manager",
]
categories = [
    "featured package",
]
favorite = false
draft = false
disableSummary = false
images = ["featured-posts/emptty.jpg"]
+++

Hello, reader. Welcome to the first blog post featuring a package available for installation at the [repository](https://userrepository.eu).

As stated in the [previous post](https://userrepository.eu/post/hello-world), I will occasionally highlight a package I feel it brings value to the users. My first choice is [`emptty-git`](https://github.com/tvrzna/emptty), a really fast and simple Display Manager that runs on a TTY.

## Description

This CLI Display Manager is blazing fast and offers a few configuration options. One of these options and my personal favorite is setting the MOTD, like the one you can see in the next section.

You can also choose the TTY where it will run, set auto login, create [custom sessions](https://github.com/tvrzna/emptty/blob/master/SAMPLES.md#custom-sessions) just for emptty and a couple customization options you can check over at [Github](https://github.com/tvrzna/emptty).

## Screenshot

![second screenshot](../../featured-posts/emptty.jpg)

## How to install

{{< highlight sh >}}
sudo pacman -Syu emptty-git
{{< /highlight >}}
