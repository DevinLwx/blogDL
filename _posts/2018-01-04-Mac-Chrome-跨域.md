---
layout:     post
title:      Mac chrome 跨域
subtitle:   跨域处理
date:       2018-01-04
author:     DL
header-img: img/tool/post-bg-cross-domain.png
catalog: true
tags:
    - 工具
    - 跨域
---

## 前言
首先要说的是，我的版本是63的，也就是说是49以后的版本，所以49以后版本的朋友可以用我的这个方法，如果还是之前的老版本，网上其他的通用方法应该就是OK的

## 第一步
创建一个文件夹，这个文件夹是用来保存关闭安全策略后的用户信息的，名字可以随意取，位置也可以随意放
注：我的名称chromeCrossDomain，路径是/Users/lidabiaoge/chromeCrossDomain

## 第二步
打开控制台，输入下面这段代码
```
open -n /Applications/Google\ Chrome.app/ --args --disable-web-security  --user-data-dir=/Users/lidabiaoge/chromeCrossDomain
```
<div class="show-return">
    <img alt="" src="/blogDL/img/tool/cross-domain-bash.png">
</div>

## 完成
成功后弹窗
<div class="show-return">
    <img alt="" src="/blogDL/img/tool/cross-domain-finish.png">
</div>
