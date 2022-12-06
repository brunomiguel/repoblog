+++
author = "Bruno Miguel"
title = "Reaching 2000 packages"
date = "2022-12-06"
description = "The number of packages provided by Userrepository continues to increase"
tags = [
    "userrepository",
    "news",
    "packages",
    "mark",
]
categories = [
    "news",
]
favorite = false
draft = false
disableSummary = false
+++

Almost ten months have passed since the last blog post. During that time, the number of packages continued to grow, reaching 1895 at the time of this writing. Some new additions are kernels, OCR software, icon packages, etc.

The repository will not reach the 2000 packages mark as the year ends. That's OK, but it leaves me a little sad because that was a personal goal for this project. It's one of the effects of package curation. The most important thing is to provide valuable packages for users of Arch Linux and Arch-based Linux distributions.

During this time, I had to make some changes to the build system due to decreased I/O performance on the server where the VM is hosted. Now, the buildbot takes care of non _*-git_ packages first to check if they have updates and build them if they do, and then compiles every _*-git_ package in the repository. This change allowed me to save some build time, taking, on average, nine hours to build all updated "regular" packages and all the _*-git_ packages.

Currently, the build script only runs once per day. As soon as the performance issues (out of my control) are solved, I intend to run it at least twice daily. Sadly, I don't have an ETA for the provider to fix the performance issues, but I'm hopeful it will be soon.