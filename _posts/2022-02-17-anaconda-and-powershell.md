---
layout:     post
title:      "anaconda环境在powershell未配置下显示import error的解决问题"
subtitle:   "anaconda with powershell"
date:       2022-02-24 17:00:00
author:     "Lxsy"
catalog: false
header-style: text
tags:
  - python
  - 环境配置
  - anaconda



---

之前一直使用powershell作为我的terminal。

在vscode上，我已经选定了我的conda环境，并且没有报错包吧不存在的问题，然而，在powershell中用命令行方式执行时，却一直报错没有sklearn库

在经历了反复的删除重装库之后，仍然没有解决问题

于是我尝试换一个conda环境，进行安装库，换了之后，还是不太行，并且惊奇地发现powershell又给我转到base环境里了，于是决定用anaconda prompt来进行安装

安装之后，尝试仍然无果，但是鬼使神差地，我在anaconda运行该包例程竟然能运行！

于是我开始搜索是不是powershell的问题，一查，果然如此

解决方案是在powershell输入如下命令

```shell
conda init powershell
```

之后就没有任何问题啦！
