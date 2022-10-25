---
title: "{{ replace .Name "-" " " | title }}"

date: {{ now.Format "2006-01-02" }}
url: /{{ .Name }}/
draft: false
searchHidden: false
ShowToc: true
author: "Max Allred"
description: ""
categories: [
    ""
]
tags: [
    ""
]
cover:
    image: "images/2022/{{ .Name }}.jpg"
    alt: "<alt text>" # alt text
    caption: "<text>" # display caption under cover
    relative: false # when using page bundles set this to true
    hidden: true # only hide on current single page
---

## Video
{{< rawhtml >}}    
    
{{< /rawhtml >}}

