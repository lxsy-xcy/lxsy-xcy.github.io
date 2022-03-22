---
layout:     post
title:      "powershell输入流重定向问题"
subtitle:   "powershell redirectionn"
date:       2022-03-22 23:30:00
author:     "Lxsy"
catalog: false
header-style: text
tags:
  - powershell


---

powershell不支持这样的重定向写法

```shell
./a.exe <in.txt >a.txt
```

因此我的解决方案是用管道代替

```shell
Get-Content in.txt | ./a.exe >a.txt
```

