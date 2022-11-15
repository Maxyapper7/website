---
title: "How to update Fedora"

date: 2022-11-15
url: /updatefedora/
draft: false
searchHidden: false
ShowToc: true
author: "Max Allred"
description: "This is how to update fedora"
categories: [
    "Linux"
]
tags: [
    "Fedora",
    "Update"
]
cover:
    image: "images/2022/updatefedora.jpg"
    alt: "<alt text>" # alt text
    caption: "<text>" # display caption under cover
    relative: false # when using page bundles set this to true
    hidden: true # only hide on current single page
---

## Why Update?
You might want to update for a few reasons. First, if your on the gnome fedora spin you will be able to use gnome 43, which has some cool updates to it. There are also newer packages avalable. Fedora is a semi-rolling release distro. It usally has two updates a year. This is sort of like Debian's release shedule but it happens way more often.

## Not Update?
There are a few reasons why you should not update. First, you like a more stable experience. When ever a new version is released there are going to be bugs no matter how much bug testing when on. So if you stay but a update or two you will have a more stable experince. Two, more packages will be avalible. Some programs just won't be supported on the newer version. But this is not very common

## Updating
Note: I am going from fedora 36 to 37

1. Run the command `sudo dnf upgrade --refresh` and then reboot. This is going to update any signing keys.

2. Run the command `sudo dnf install dnf-plugin-system-upgrade` to install the dnf system upgrader. This is most likely allready installed on your system.

3. Now we need to install the new packages, to do this run `sudo dnf system-upgrade download --releasever=37`. Note: This is going to take a long time and download 2-3gb

4. Finally run the command `sudo dnf system-upgrade reboot` to update the system. This is going to take a while.


## FAQ

* I see errors when using RPM/DNF tools

To fix this backup `/var/lib/rpm/` then run the command `sudo rpm --rebuilddb`
## Video
{{< rawhtml >}}    
    
{{< /rawhtml >}}

