---
title: "APT Package Manager"

date: 2022-10-24
url: /aptpackagemanager/
draft: false
searchHidden: false
ShowToc: true
author: "Max Allred"
description: "This guide tells you what and how to use the apt package manager"
categories: [
    "Linux"
]
tags: [
    "Debain",
    "APT",
    "Package Manager"
]
cover:
    image: "images/2022/apt.jpg"
    alt: "<alt text>" # alt text
    caption: "<text>" # display caption under cover
    relative: false # when using page bundles set this to true
    hidden: true # only hide on current single page
---

## What is APT?

Apt is a package manager. Package manager is something that uses a thing called repositroies to dowload and install packages. Apt is mainly used on debain and debain distros. And because of that apt tends to be behind a little bit behind and dosen't have the newest releases. Note that apt is just the program that gets and installes packages NOT the repositry. 

## APT commands

### Install
```
sudo apt install <package>

#This command finds and installs packages
#This also must be run as sudo
#Ex: sudo apt install neofetch
```
### Search
```
apt search <package>

#This command searchs the repositroies that you have activated
#This command does not have to be run as sudo
#Ex: sudo apt search openjdk
```
### Update & Upgrade
```
sudo apt update

#This command finds any packages that need to be updated
#This command needs to be run as sudo

sudo apt upgrade

#This command updates the packages
#This also needs to be run as sudo
#Note: You have to run sudo apt update before sudo apt upgrade
```
### Remove & Purge
```
sudo apt remove htop

#This command removes the program
#This must be run as sudo

sudo apt purge htop

#This command complete deletes all files the program created
#This also must be run as sudo
```
### List
```
apt list --upgradable

#This shows you any packages that can be updated

apt list --installed

#This will show you any installed packages
```
### Autoremove
```
sudo apt autoremove

#This will remove any packages that aren't needed anymore
```

## Video
{{< rawhtml >}}    
      
{{< /rawhtml >}}
