---
title: "如何用hugo搭建博客"
date: 2020-03-27T19:09:49+08:00
draft: false
---

# 如何用hugo搭建博客

## 第一步
1. 去[hugo release 页面](https://github.com/gohugoio/hugo/releases)下载 hugo_xxx_Windows-64bit.zip
2. 解压hugo并将其配置到path
3. 重启终端，运行hugo version 查看版本

## 第二步
1. 进入[hugo官网](https://gohugo.io/)，点击QuickStart快速开始
2. 从Step2 开始复制粘贴代码到终端，直到Step7
   * 查看hugo版本
   ```
   hugo version
   ```
   * 创建新的网站
   ```
   hugo new site quickstart
   ```
   * 创建默认主题
   ```
   git init

   git submodule add https://github.com/budparr/gohugo-theme-ananke.git themes/ananke

   echo 'theme = "ananke"' >> config.toml
   ```
   * 创建第一篇博客
   ```
   hugo new posts/my-first-post.md
   ```
   * 预览草稿
   ```
   hugo server -D
   ```
   * 打开 config.toml 进行博客配置
   ```
   baseURL = "https://example.org/"
   languageCode = "en-us"
   title = "My New Hugo Site"
   theme = "ananke"
   ```
3. 得到一个public目录，这是博客站点
4. hugo server -D 可以预览草稿
