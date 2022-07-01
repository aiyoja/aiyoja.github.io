---
title: markdown基本语法
date: 2022-06-24 17:43:04
tags:
 - Markdown
categories: 教程
---

# **目录**

- [一、前言](https://www.cnblogs.com/nickchen121/p/10821946.html#一前言)
- 二、Markdown基本语法
  - [2.1 标题](https://www.cnblogs.com/nickchen121/p/10821946.html#tid-E5pcmm)
  - [2.2 加粗](https://www.cnblogs.com/nickchen121/p/10821946.html#tid-AzkCjz)
  - [2.3 斜体](https://www.cnblogs.com/nickchen121/p/10821946.html#tid-HtMW8J)
  - [2.4 高亮](https://www.cnblogs.com/nickchen121/p/10821946.html#tid-zYsfQR)
  - [2.5 上标](https://www.cnblogs.com/nickchen121/p/10821946.html#tid-mykKM2)
  - [2.6 下标](https://www.cnblogs.com/nickchen121/p/10821946.html#tid-ryDYZM)
  - [2.7 代码引用（>式）](https://www.cnblogs.com/nickchen121/p/10821946.html#tid-rE6FGX)
  - [2.8 代码引用（```式）](https://www.cnblogs.com/nickchen121/p/10821946.html#tid-KRazcW)
  - [2.9 代码引入（`式）](https://www.cnblogs.com/nickchen121/p/10821946.html#tid-kjezaQ)
  - [2.10 插入链接（链接显示）](https://www.cnblogs.com/nickchen121/p/10821946.html#tid-4xdcbr)
  - [2.11 插入链接（链接描述显示）](https://www.cnblogs.com/nickchen121/p/10821946.html#tid-eayDT5)
  - [2.12 插入图片（链接）](https://www.cnblogs.com/nickchen121/p/10821946.html#tid-tp735j)
  - [2.13 插入图片（图片路径）](https://www.cnblogs.com/nickchen121/p/10821946.html#tid-tj85DE)
  - [2.14 有序列表](https://www.cnblogs.com/nickchen121/p/10821946.html#tid-4SeY8P)
  - [2.15 无序列表](https://www.cnblogs.com/nickchen121/p/10821946.html#tid-NmGW8F)
  - [2.16 分割线](https://www.cnblogs.com/nickchen121/p/10821946.html#tid-HNp5QF)
  - [2.17 表格而且第二行必须得有，并且第二行的冒号代表对齐格式，分别为居中；右对齐；左对齐）：](https://www.cnblogs.com/nickchen121/p/10821946.html#tid-NYDi2p)
  - [2.18 数学公式（行内嵌）](https://www.cnblogs.com/nickchen121/p/10821946.html#tid-DhWd2R)
  - [2.19 数学公式（块状）](https://www.cnblogs.com/nickchen121/p/10821946.html#tid-4rMY8J)
- [三、总结](https://www.cnblogs.com/nickchen121/p/10821946.html#三总结)


Python从入门到放弃完整教程目录：https://www.cnblogs.com/nickchen121/p/10718112.html



# 一、前言

- **由于有些语法无法在博客园展示，推荐使用Typora解锁全套，下载地址：https://www.typora.io/**
- **推荐使用jupyter，使用方法：https://www.cnblogs.com/nickchen121/p/10722733.html**
- **markdown数学公式大全，https://www.cnblogs.com/nickchen121/p/11746655.html**

Markdown是一种可以使用普通文本编辑器编写的标记语言，通过简单的标记语法，它可以使普通文本内容具有一定的格式。 --摘自百度百科

没想到一向不太靠谱的百度百科这次竟有了如此精辟的解释。之前项目一直使用`word`撰写文档，有比较大的弊病：

- 只能对纯文本文件进行版本控制，而word是二进制格式
- 格式繁杂，经常需要中断写作来控制格式
- 代码与文档分离，给写文档造成更大的阻力

而假如单纯的使用txt，就没有一点格式了，用html虽然既有格式又能加入版本控制，但是需要花费较多的时间在标签上，而且标签占了文档的较大百分比，不易阅读。

所以，最终的解决方案就是 **Markdown** ，作为一种轻量级的标记语言，能在非常短的时间内掌握。而且不仅可以用于写文档，还可以写博客、写简书、做一些随手笔记。Markdown文件以.md结尾，可以导出为html和PDF（需要使用的工具支持）。它是一种语法（个人认为是简化版的html），但是和html不同的是，各种解析器对其会有不同的表现。比如我的IDEA Markdown插件会把分割线显示成一条细灰线，Cmd Markdown则是显示一条虚线。所以建议保持使用一种Markdown工具和尽量使用标准语法。

# 二、Markdown基本语法

## 2.1 标题

代码：



python

```python
# 一级标题
## 二级标题
### 三级标题
#### 四级标题
##### 五级标题
###### 最小只有六级标题
```

效果：

过于粗暴，不予以展示，你复制粘贴即知晓！！！

## 2.2 加粗

代码：



python

```python
**我被加粗了**
```

效果：

**我被加粗了**

## 2.3 斜体

代码：



python

```python
*我倾斜了了*
```

效果：

*我倾斜了了*

## 2.4 高亮

代码：



python

```python
==我高亮了==
```

效果：

我高亮了

## 2.5 上标

代码：



python

```python
2^2^
```

效果：

22

## 2.6 下标

代码：



python

```python
H~2~o
```

效果：

H2o

## 2.7 代码引用（>式）

代码：



python

```python
> hello markdown!
```

效果：

> hello markdown!

代码：



python

```python
> hello markdown!
>> hello markdown!
```

效果：

> hello markdown!

> > hello markdown!

## 2.8 代码引用（```式）

代码：



python

```python
# 不要复制这一句话，并且去掉下面的反斜杠，谢谢！
\`\`\`python
print('hello nick')
\`\`\`
```

效果：



python

```python
print('hello nick')
```

## 2.9 代码引入（`式）

代码：



python

```python
# 不要复制这一句话，并且去掉下面的反斜杠，谢谢！
\`print('hello nick')\`
```

效果：

```
print('hello nick')
```

## 2.10 插入链接（链接显示）

代码：



python

```python
<https://www.cnblogs.com/nickchen121/p/10718112.html>
```

效果：

https://www.cnblogs.com/nickchen121/p/10718112.html

## 2.11 插入链接（链接描述显示）

代码：



python

```python
[nickchen博客](https://www.cnblogs.com/nickchen121/p/10718112.html "nickchen博客")
```

效果：

nickchen博客

## 2.12 插入图片（链接）

代码：



python

```python
![数据类型总结-搞笑结束.jpg?x-oss-process=style/watermark](https://imgmd.oss-cn-shanghai.aliyuncs.com/Python从入门到放弃/数据类型总结-搞笑结束.jpg?x-oss-process=style/watermark '描述信息')
```

效果：

[![img](https://imgmd.oss-cn-shanghai.aliyuncs.com/Python%E4%BB%8E%E5%85%A5%E9%97%A8%E5%88%B0%E6%94%BE%E5%BC%83/%E6%95%B0%E6%8D%AE%E7%B1%BB%E5%9E%8B%E6%80%BB%E7%BB%93-%E6%90%9E%E7%AC%91%E7%BB%93%E6%9D%9F.jpg)](https://imgmd.oss-cn-shanghai.aliyuncs.com/Python从入门到放弃/数据类型总结-搞笑结束.jpg?x-oss-process=style/watermark)

## 2.13 插入图片（图片路径）

- 绝对路径：.md文本同目录下图片的名字，如`数据类型总结-搞笑结束.jpg?x-oss-process=style/watermark`
- 相对路径：图片在电脑中的路径地址，如`\Users\nick\mac\desktop\数据类型总结-搞笑结束.jpg?x-oss-process=style/watermark`

代码：



python

```python
![数据类型总结-搞笑结束.jpg?x-oss-process=style/watermark](数据类型总结-搞笑结束.jpg?x-oss-process=style/watermark '描述信息')

![数据类型总结-搞笑结束.jpg?x-oss-process=style/watermark](\Users\nick\mac\desktop\数据类型总结-搞笑结束.jpg?x-oss-process=style/watermark '描述信息')
```

效果：

![](http://img.aiyou.ga/pg/qrcode_for_gh_d48a28881167_258.jpg)



https://www.cnblogs.com/nickchen121/p/\Users\nick\mac\desktop\数据类型总结-搞笑结束.jpg?x-oss-process=style/watermark)

## 2.14 有序列表

代码：



python

```python
1. one
2. two 
3. three
```

效果：

1. one
2. two
3. three

## 2.15 无序列表

代码：



python

```python
* one
* two
* three
```

效果：

- one
- two
- three

## 2.16 分割线

代码：



python

```python
---
```

效果：

------

## 2.17 表格而且第二行必须得有，并且第二行的冒号代表对齐格式，分别为居中；右对齐；左对齐）：



python

```python
name | age | sex 
:-:|:-|-:
tony|20|男
lucy|18|女
```

效果：

| name  | age  |  sex |
| :---: | :--- | ---: |
| nick  | 19   |   男 |
| jason | 18   |   女 |

## 2.18 数学公式（行内嵌）

代码：



python

```python
内嵌数学公式$\sum_{i=1}^{10}f(i)\,\,\text{thanks}$
```

效果：

内嵌数学公式∑10i=1f(i)thanks∑i=110f(i)thanks

## 2.19 数学公式（块状）

代码：



python

```python
$$
\sum_{i=1}^{10}f(i)\,\,\text{thanks}
$$
PYTHON 复制 全屏
```

效果：





∑i=110f(i)thanks∑i=110f(i)thanks



# 三、总结

以上所述就是Markdown的基本标签，虽然不多，但是可以解决大部分情况。
