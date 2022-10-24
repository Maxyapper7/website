---
title: "How to Install a Grub Theme on Fedora Linux"

date: 2022-10-20
url: /installgrubthemeonfedora/
draft: false
searchHidden: true
ShowToc: true
author: "Max Allred"
description: "This guide tells you how to install a grub theme on fedora"
categories: [
    "Linux"
]
tags: [
    "Fedora",
    "Grub2",
    "Customization"
]
cover:
    image: "images/2022/installgrubthemeonfedora.jpg"
    alt: "<alt text>" # alt text
    caption: "<text>" # display caption under cover
    relative: false # when using page bundles set this to true
    hidden: true # only hide on current single page
---
## What is a grub and what is a grub theme?
Grub is a bootloader. A bootloader is the thing that starts the operating system. It is the first program that is started when the system turns on. Then it gives controll over to the kernal. You may see it when booting up. It's the thing that might say what linux your on and any other operating systems installed. But note that not every linux distro shows this by default. Then what is a grub theme? A grub theme is something that covers up the default look of grub.

## How to install a grub theme

1. Go to [Gnome-look.org](https://www.gnome-look.org) and click on gnome themes or click right [here](https://www.gnome-look.org/browse?cat=109&ord=latest) and download any theme you like.

2. Go to your downloads folder and extract the file. Then open a terminal up in your downloads folder.

3. Run the command `sudo mkdir /boot/grub2/themes` This will make a themes folder.

4. Run the command `sudo mv <theme> /boot/grub2/themes/` This will move the theme into the folder we just created.

5. Run the command `sudo cp /etc/default/grub /etc/default/grub.bkup` This is going to make a backup of the grub config file.

6. Finally run `sudo nano /etc/default/grub` and do the following:
```
# Comment out the line that says:
GRUB_TERMINAL_OUTPUT="console"

# Add this line to the bottom of the file:
GRUB_THEME=/boot/grub2/themes/<theme>/theme.txt
```
7. Run this command `sudo grub2-mkconfig -o /boot/efi/EFI/fedora/grub.cfg` and your done. This command refreshes the grub file.

## FAQ

- Does this work for other linux distros?

Yes and No. Fedora uses grub2 but some other linux distros use just grub. So you could but it would take changing some of the steps.

- Are there any grub alternatives?

Yes there is BURG, GAG, LILO, and Syslinux just to name a few.

- Does GRUB stand for something?

Yes, Grand Unified Bootloader

- It's not working, help.

There are a few things that arn't working. First this guide could be out of date. The theme your using might not be compatible. Or there is something wrong with your grub config file.
