---
layout: post
title: "OS X下中文设置"
categories: [中文配置]
tags: [OS X, 中文配置]
comments: True
---

前一阵子一直没有在我的MBA上做任何有关于中文的操作，所以貌似没有什么动力去搞中文的问题。
就算是`ls`的时候一直出乱码，我也都忍了，反正也没有什么重要的信息。
但是因为最近整理出来了这个中文的jekyll + github博客，所以需要开始在vim下输入中文了，中文终端显示问题就必须解决了。

## Bash环境配置（罪恶之源）

其实最主要的环境配置就两行。

    export LC_ALL=en_US.UTF-8
    export LANG=en_US.UTF-8

这样Bash就不会默认使用latin编码来解读文字了。

## 终端环境配置（没那么重要）

我一直使用[item2]作为我的终端，所以下面这几个配置是针对iterm2的。

**Encoding: UTF-8**：经证实，完全没有必要使用GBK或者其他的中文编码，所以设置为UTF8就好了。

![UTF-8 encoding][iterm-encoding]

**兰亭黑体**：我不确认是否所有的mac都自带这个字体，但是我自己不记得手动安装过这个字体。选择它也纯粹是处于好看的考虑。

![兰亭黑体设置][iterm-font]

下面的截图是兰亭黑体的实际显示效果，个人觉得还是很不错的，至少比默认的中文字体要好很多。

![兰亭黑体截图][iterm-screenshot]

[iterm-encoding]: http://i.imgur.com/4urc0ur.png

[iterm-font]: http://i.imgur.com/2y0dgiX.png

[iterm-screenshot]: http://i.imgur.com/ZAmAAG7.png
