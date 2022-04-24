---
title: Hexo + Typora + Github
date: 2022-04-24 11:27:44
categories: Tools
tags:
---

### Hexo博客搭建

#### HEXO安装与配置

主要参考知乎的[GitHub+Hexo 搭建个人网站详细教程](https://zhuanlan.zhihu.com/p/26625249)

在访问xxx.github.io的时候会出现404的错误。在网上看了一圈没发现大多数解决方法都没什么用，后面想了下可能是deploy那里的问题

现在github默认的分支都是main分支了，用下面这个方式配置虽然在操作的过程中没有报错，但是实际上是在main分支的基础上又建了一个新的master分支，每次push的内容都存放在master分支里，而默认的是main分支，**把master修改成main就可以了**。可以参考这个问题[关于hexo更新到GitHub后博客内容未变问题](https://blog.csdn.net/Lu_xiuyuan/article/details/112056997)

<img src="https://cdn.jsdelivr.net/gh/batman47steam/typora-pic/images/image-20220424105333065.png" alt="image-20220424105333065"/>



#### 图床设置

完成上面的操作以后，基本就可以访问自己的xxx.github.io这个网页了，下面考虑一下搭建图床的事情，因为之前使用typora的时候就是使用了github当图床，所以这一步还是比较简单的。可以设置typora的图片偏好是自动上传，或者先保存在相对路径，自己后面在选择上传到图床

如果忘记了可以参考这个[使用GitHub PicGod搭建图床](https://blog.csdn.net/weixin_41301576/article/details/121645453)

#### 数学公式

上传了第一篇博客以后发现typora的数学公式没办法渲染，会直接显示`$F$`

目前主要参考这篇文章[Hexo使用数学公式](https://yixin-oss.gitee.io/daytoy/2021/06/29/Hexo%E4%BD%BF%E7%94%A8%E6%95%B0%E5%AD%A6%E5%85%AC%E5%BC%8F/)

#### categories about tags相关的设置

参考这篇文章[Hexo 博客 NexT 主题下如何添加分类、标签](https://www.cnblogs.com/cscshi/p/15196102.html)

#### 删除已经创建的博客

参考这个[如何删除一篇已经发布的文章](https://blog.csdn.net/qq_34243930/article/details/109046120)

#### 对next主题一些额外的配置

图片放大，设置pjax等[Hexo Next 主题详细配置之一](https://www.techgrow.cn/posts/755ff30d.html#%E5%90%AF%E7%94%A8-Pjax)

#### 头部模板

在`./scaffolds/post.md`里直接加上categories，就不用每次新建完以后再自己添加了

#### 更改网站图标

https://zhuanlan.zhihu.com/p/426080861
