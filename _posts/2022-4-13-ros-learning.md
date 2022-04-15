---
layout:     post
title:      "古月居ros入门21讲 遇到的问题"
subtitle:   "ros problem and note"
date:       2022-04-13 23:30:00
author:     "Lxsy"
catalog: false
header-style: text
tags:
  - ros



---

good reference：https://blog.csdn.net/takedachia/category_11584500.html

# 创建功能包

* 不能直接新建个文件夹，而是要在工作区的src路径下，运行如下命令

  ```bash
  catkin_create_pkg pkg_name 依赖包
  ```

# 关于什么时候注册需要加<>

advertise和serviceClient

# yaml写参数

注意要在`：`后加空格，否则会识别不出来

```yaml
A: 3
B: 2

Group:       
  A: 2
  B: "hello"
```

