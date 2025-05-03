---
title: "在 GitHub Pages 上部署 Jekyll 静态博客"
date: 2019-04-18T15:34:30-04:00
toc: true
categories:
  - 博客
tags:
  - Jekyll
---

本篇文章将简单介绍一下如何使用 Minimal Mistakes 主题在 GitHub Pages 上部署 Jekyll 静态博客。 虽然搭建静态博客的过程比较折腾，但可以免费使用 GitHub 提供的静态网页托管服务。

# 组件一览

# 搭建步骤
## 创建 GitHub Pages
### 简化版操作
1. 打开 [Minimal Mistakes](https://github.com/mmistakes/minimal-mistakes) 的[模板创建页面](https://link.zhihu.com/?target=https%3A//github.com/mmistakes/mm-github-pages-starter/generate)；
2. 在 Repository name 中输入`用户名.github.io`，其他设置默认，然后点击`Create repository from template`按钮完成创建；
3. 在仓库的设置中自定义仓库名称；
4. 在仓库的设置中打开 GitHub Pages 功能；
5. 完成创建后，可以使用`用户名.github.io/自定义仓库名`访问博客。

## 安装本地预览环境
1. 从 [Ruby 官网](https://rubyinstaller.org/downloads) 下载 Ruby+Devkit，选择推荐版本，以默认设置安装；
2. 通过`gem install jekyll bundler`指令来安装 Jekyll 和 Bundler gems；
3. 在计划存放博客的文件夹打开命令行终端，执行以下指令构建新的 blog site，并在本地运行：
`jekyll new myblog`
`cd myblog`
`bundle exec jekyll serve`
4. 浏览器中打开地址 [127.0.0.1:4000](127.0.0.1:4000)，即可查看生成的 Jekyll 博客站。

## 编写博客
### 用 Jekyll Admin 在线编写
1. 执行`gem install jekyll-admin`指令进行安装；
2. 在`_config.yml`中添加 `- jekyll-admin`；
3. 在`Gemfile`中添加 `gem "jekyll-admin"`；
4. 执行`bundle exec jekyll serve`指令启动 jekyll；
5. 直接访问 [http://127.0.0.1:4000/admin](http://127.0.0.1:4000/admin) 就可以看到 [Jekyll Admin](https://jekyll.github.io/jekyll-admin) 的使用界面；

## 使用主题

---


###### 参考资料
- [Jekyll • 简单静态博客网站生成器 - 将纯文本转换为静态博客网站](https://jekyllcn.com)
