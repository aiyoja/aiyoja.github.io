title: 安装hexo和基本的使用
author: 弶森
tags: [Hexo]
categories: [教程]

date: 2022-06-23 10:56:00
---
搭建个人的博客，在自己的服务器上。用hexo的好处是，所有的博客可以写在markdown文件中，备份在本地，迁移起来很方便。

个人服务器配置

安装node，git

curl -sL https://rpm.nodesource.com/setup_10.x | bash - yum install -y nodejs
通过这条命令安装node和npm

git我的服务器已经有了。

git --version
可以查看有没有安装git。我的输出git version 1.8.3.1

使用npm安装Hexo
最好切换为taobao的源，下载的会快一些。

npm config set registry https://registry.npm.taobao.org
验证是否切换成功：

npm config get registry
输出淘宝源的地址https://registry.npm.taobao.org/，即切换成功。

安装Hexo

npm install -g hexo-cli
验证是否安装成功：

hexo version
输出版本信息，则安装成功。

搭建博客
创建博客的目录hexo init 目录名。我就在当前目录下创建blog的文件夹作为博客的根目录。

hexo init blog
进入刚刚的目录

cd blog
安装

npm install
第一次启动博客
生成静态页面

hexo g
启动hexo博客

hexo s
这时，访问http://ip:4000就可以看到hexo的默认主题了。

如果要想要后台运行

nohup hexo s > blog.log 2>&1 & 
介绍几种发布博客的方式
直接将markdown文件复制到blog目录下的source/_posts文件夹中。即可看到博客
新建git或svn仓库，当本地提交markdown文件到仓库时，钩子将新增加的文件复制到source/_posts文件夹下。
通过hexo工具也可以新建博客hexo new 博客。具体参照官网
通过hexo-admin工具，通过浏览器就可以管理
安装hexo-admin通过浏览器管理发布博客
安装hexo-admin

npm i hexo-admin --save
重启hexo

hexo server -d
这时，通过http://ip:4000/admin即可管理博客。也可以在这个页面的setting中生成后台的用户名和密码。复制到_config.yml就会生效，重启博客后登录后台前就需要账号密码。

域名
如参考的那位兄弟所说IP访问这么low b的访问方式，当然要优化一下。思路：通过NGINX做一个反向代理，将http://blog.hanjun.red这种二级域名代理到本机的localhost:4000。反向代理可以让自己的域名做更多的事情。

主题
安装主题
进入主题的目录blog/themes，克隆主题项目的地址

cd ./themes

git clone https://github.com/maochunguang/black-blue

更换主题：进入根目录，更改配置文件_config.yml

theme: black-blue
重新启动。

更多的关于主题的配置，请参考具体每个主题的官方说明

找了很久，推荐几个好看的。

black-blue
预览地址

GitHub 项目地址

安装教程

Diaspora（动漫大图）
预览地址

GitHub 项目地址

安装教程

Melody
预览地址

GitHub 项目地址

安装教程

岛
项目地址

效果预览

中文说明

NexT
butterfly
Nexmoe