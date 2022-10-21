---
title: "How to install ventoy"

date: 2022-10-20
url: /howtoinstallventoy/
draft: false
ShowToc: true
author: "Max Allred"
description: "The guide tells you what and how to use ventoy"
categories: [
    "Windows",
    "Linux"
]
tags: [
    "Ventoy"
]
cover:
    image: "images/2022/howtoinstallventoy.jpg"
    alt: "" # alt text
    caption: "" # display caption under cover
    relative: false # when using page bundles set this to true
    hidden: true # only hide on current single page
---

## What is Ventoy?

Ventoy is a tool that can boot multiple ISO's off of one flashdrive. For example other tools such as rufus or eatcher can only have one ISO per flashdrive. And when you want a new ISO on a that flashdrive you have to reflash it. On the other hand ventoy you can just drag and drop ISO's onto the flash drive and it makes them bootable.

## How to install Ventoy

You will need:

- Flashdrive
- Computer

### Windows

1. Plug in your USB drive.

2. First you need to download the .exe file from [ventoy's](https://github.com/ventoy/Ventoy/releases) website.

3. Extract the .zip file run the executable.

4. **Make sure the USB is correct** and click install. 

5. Move ISO's to your flash drive and your done.

### Linux

1. Plug in your USB drive.

2. First you need to download the archive file from [ventoy's](https://github.com/ventoy/Ventoy/releases) website.

3. Extract the .tar file and go into the folder.

4. Open a terminal inside the folder and run the command `sudo bash VentoyWeb.sh`

5. Open a web browser and go to [localhost:24680](http://localhost:24680/).

6. **Make sure the USB is correct** and click install. 

7. After it has completed the install, go to the terminal hit `ctrl + c` to stop ventoy.

8. Move ISO files to your flash drive and your done.

## FAQ

- How big does my USB Need to be?

I would say that it needs to at least 32gb but 64 or 128gb is what I would recommend.

- How do I install a theme onto ventoy

I will create a video/artical showing any customazation optines.

## Video Walkthrough
