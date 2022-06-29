---
title: 如何用hexo新建一篇文章并编辑文章
date: 2022-06-24 17:29:00
tags:
 - Hexo
 - Markdown
 - GitHub
categories: 教程
---

# [如何用hexo新建一篇文章并编辑文章](https://www.cnblogs.com/ashenweb/p/13415790.html)

操作道具：hexo

# 第一步：新建MarkDown文件

使用CMD命令进入到你的blog

```bash
cd blog
```

新建文件

```bash
hexo new "我的第一篇博客"
```

提示新建完成，这个时候在bolg目录下的\source_posts中会多出一个md文件 **注意new和引号之间要有一个空格**

# 第二步：编写文件

使用记事本或其他编写工具打开文件，这里建议使用vscode
[网上找到的一篇关于MarkDown语法讲解文章](https://www.cnblogs.com/nickchen121/p/10821946.html)

# 第三步：生成博客

使用CMD命令进入到你的blog

```bash
cd blog
```

生成博客

```bash
hexo g
```

注意这里生成失败可能是你的MD文件语法有问题,解决方案是清除再次生成

```bash
hexo clean
然后再
hexo g
```

# 如何插入图片

在blog文件夹下找到_config.yml，记事本打开，将post_asset_folder: **false**改为post_asset_folder:**true**并保存
使用cmd命令下载插件

```bash
npm install https://github.com/CodeFalling/hexo-asset-image -- save
```

注意这里可能卡住或者失败，重新输入命令进行下载就可以了
[![img](https://img2020.cnblogs.com/blog/2114049/202008/2114049-20200801174429484-1580719407.jpg)](https://img2020.cnblogs.com/blog/2114049/202008/2114049-20200801174429484-1580719407.jpg)
**这里提示WARN不要紧**
这样你再次使用heox new的时候\blog\source_posts下就会自己生成一个同名文件夹，把需要用到的图片放入这个文件夹下，在MD文件下调用的方法是

```bash
![](a1.jpg)
```
