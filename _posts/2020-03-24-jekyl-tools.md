---
title:      jekyll 从零到一
date:       2020-03-24
author:     萧国
catalog: true
categories: 技术
tags:
    - jekyll
---
记录从零到一开始研究使用jekll + github 生成个人博客的点点滴滴。

<!-- more -->


## jekll 本地调试博客页面
> 解决每一篇博客都要同步到github上，然后才可以渲染查看页面的不便，需要在本地更新完博客之后，就可以预览和调试

### 安装jekyll的先决条件
* Ruby 2.4.0 或更高版本，包含所有用于开发的头文件（可通过* 执行 ruby -v 指令检查 ruby 版本）
* RubyGems （可通过执行 gem -v 指令检查版本）
* GCC and Make （以防你的系统中没有安装这些工具，请通过执行 gcc -v,g++ -v 和 make -v 指令进行检查，gcc 需要安装command line，如果电脑上已经安装完xcode，一般情况下命令行工具和gcc、make都会安装完成）


如果上述工具没有安装完成，请参考以下两个链接：
* [Jekyll 先决条件](https://www.jekyll.com.cn/docs/installation/#requirements)
* [Mac - 先决条件安装](https://www.jekyll.com.cn/docs/installation/macos/)

### 安装jekyll
1. 安装一个完整的Ruby 开发环境。
2. 安装 Jekyll 和 bundler gems。
``` gem install jekyll bundler ```
3. 在 ./myblog 目录下创建一个全新的 Jekyll 网站。
``` jekyll new myblog ```
4. 进入新创建的目录。
``` cd myblog ```
5. 构建网站并启动一个本地服务器。
``` bundle exec jekyll serve ```
6. 在浏览器中打开 http://localhost:4000 网址

如果是在本地中已经clone的文件夹，只需要进入到博客所在目录，通过jekyll 启动本地服务器即可
``` jekyll s ```


### 关闭链接
ctrl-c 即可
