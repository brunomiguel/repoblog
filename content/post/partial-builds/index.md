+++
author = "Bruno Miguel"
title = "Changes to the build process"
date = "2021-09-10"
description = "Userrepository stopped building the full set of packages once a day and now only builds updated packages every 6 hours"
tags = [
    "userrepository",
    "changes",
]
categories = [
    "news",
]
favorite = false
draft = false
disableSummary = false
+++

Until a few days ago, all the packages available at userrepository.eu were built in batch. Given the number of packages is over 800, it took more than 10 hours (yes, 10 hours) to complete each daily full build.

Now, a new option in the build script only builds the updated packages. Not only that, all `*-git` packages are also built with this new option. I made this decision because the lack of version updates on these AUR packages doesn't mean there isn't an update to them.

The script runs every 6 hours and takes about 4h30m to complete.

To finish this blog post, a thank you note to [Fosshost](https://fosshost.org) for kindly increasing the resources on the VM.
