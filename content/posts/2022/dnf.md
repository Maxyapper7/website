---
title: "Dnf Package Manager"

date: 2022-11-15
url: /dnf/
draft: false
searchHidden: false
ShowToc: true
author: "Max Allred"
description: "This guide tells you what and how to use the DNF package manager"
categories: [
    "Linux"
]
tags: [
    "DNF",
    "Package Manager",
    "RHEL"
]
cover:
    image: "images/2022/dnf.jpg"
    alt: "<alt text>" # alt text
    caption: "<text>" # display caption under cover
    relative: false # when using page bundles set this to true
    hidden: true # only hide on current single page
---

## What is DNF
DNF is a package manger. Much like APT it finds and installs packages from a thing called repositories. DNF is mainly used on Red Hat Linux (RHEL) and what it is based off of. DNF doesn't have as many packages as APT does mainly because it is newer than APT. Also dnf is painfully slow out of the box put there are a few way to speed it up. Note that DNF just gets and installs packages and NOT the repository.

## DNF Commands 

### Install
```
sudo dnf install <package>

#This command finds and installs a package
#This must be used as sudo
#Ex: sudo dnf install neofetch
```

### Search
```
dnf search <package>

#This command searchs any active repositories for the package
#It does not need to be run as sudo
#Ex: dnf search OpenJDK
```

### Update
```
sudo dnf update

#This command finds and installs any updates
#This needs to be run as sudo
#Note: Unlike apt, dnf upgrade does the same thing
```

### Remove
```
sudo dnf remove <package>

#This command finds and uninstalls a package
#This must be run as sudo
#Ex: sudo dnf remove neofetch
```

### List Installed
```
dnf list installed

#This command lists any install packages
#This doesn't need to be run as sudo
```

### History
```
dnf history

#This command lists the last 25 commands you did
#This does not need to be run as sudo
```

### Autoremove
```
sudo dnf autoremove

#This command remvoes any packages that arn't used anymore
```


## Video
{{< rawhtml >}}    
    
{{< /rawhtml >}}

