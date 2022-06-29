---
title: Typora+PicGo+七牛云 个人博客发布方案
date: 2022-06-24 17:27:24
tags:
 - Hexo
 - Markdown
 - GitHub
categories: 教程
---

## 开篇

开篇
天下没有免费的午餐，所以我们要尽情白嫖。



注意：本篇推荐的是Typora+七牛云+PicGO。懂的都懂好用加免费这不嫖上一波嘿

不废话了，开的很快，坐稳了~



### 为啥子需要图床呢？

当我们使用相关工具编写好文章后，并将这图文并茂的文章上传到博客时，发现图片是看不了的，这个时候我们就需要图床啦。

注意：`本篇推荐的是Typora+七牛云+PicGO,懂的都懂便宜简单`

> 废话不多说，直接开打！！！

## 配置图床

## 下载PICGO

[PicGO官网](https://github.com/Molunerfinn/PicGo/releases)

博主有个小小毛病，喜欢上最新，开干就完事。

![image-20220220151438861](http://img.slcp.top/myblog/image-20220220151438861.png)

### 注册账号

[七牛云官网](https://www.qiniu.com/)

废话不多说，一般注册都是右上角，上图。

![image-20220220152200371](http://img.slcp.top/myblog/image-20220220152200371.png)

首先需要实名认证，实名认证完后会分配免费的存储空间

![image-20220220152827384](http://img.slcp.top/myblog/image-20220220152827384.png)

![image-20220220153339141](http://img.slcp.top/myblog/image-20220220153339141.png)

![image-20220220152840162](http://img.slcp.top/myblog/image-20220220152840162.png)

### 创建空间

想看其他的就来这，和阿里云的模板基本上一样。

![image-20220220153801815](http://img.slcp.top/myblog/image-20220220153801815.png)

进入对象存储页面后，先需要新建空间

![image-20220220153643625](http://img.slcp.top/myblog/image-20220220153643625.png)

> 建议服务器哪的就选哪个区

![image-20220220154114998](http://img.slcp.top/myblog/image-20220220154114998.png)

创建好后，在空间管理页面就可以看到刚才创建的空间了。

![image-20220220154336922](http://img.slcp.top/myblog/image-20220220154336922.png)

![image-20220220154457495](http://img.slcp.top/myblog/image-20220220154457495.png)

注意：`七牛云一开始会提供30天的测试域名， 后面需要添加已备案的域名。也就是自定义域名`

## 配置七牛云图床

- AccessKey和SecretKey：可以在七牛云控制台，秘钥管理页面找到你的配置
- 存储空间名：填写前面创建的空间名称
- 访问地址：对应前面提交的测试域名
- 存储区域：七牛云的存储区域（华东 z0，华北 z1，华南 z2，北美 na0，东南亚 as0 ），根据你空间所在的区域，填对应的代码

![image-20220220155538110](http://img.slcp.top/myblog/image-20220220155538110.png)

测试

![image-20220220155626888](http://img.slcp.top/myblog/image-20220220155626888.png)

## 配置TYPORA

[Typora官网](https://typora.io/)

下载好之后，点击【文件】—–【偏好设置】，如下：

![image-20220220160249952](http://img.slcp.top/myblog/image-20220220160249952.png)

> 注意：记得设置路径，一开始是默认路径

验证

![image-20220220160447569](http://img.slcp.top/myblog/image-20220220160447569.png)

然后就OK啦！！！



https://slcp.top/article/read/46

恭喜你，又卷死一堆人！！！
————————————————
版权声明：本文为CSDN博主「Slcp」的原创文章，遵循CC 4.0 BY-SA版权协议，转载请附上原文出处链接及本声明。
https://blog.csdn.net/Sunshine_Mr_Sun/article/details/123205807
