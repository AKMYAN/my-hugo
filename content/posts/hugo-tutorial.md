+++
date = '2025-10-07T21:20:21+08:00'
draft = false
title = 'Hugo 入门教程：从零开始构建静态网站'
tags = ['Hugo', '教程', '静态网站', 'Web开发']
categories = ['技术']
description = '详细介绍如何使用 Hugo 构建静态网站的完整教程'
+++

## 什么是 Hugo

Hugo 是一个用 Go 语言编写的静态网站生成器，以其极快的构建速度而闻名。它可以将 Markdown 文件转换为完整的 HTML 网站。

## 安装 Hugo

### Windows 用户

使用 Windows 包管理器 winget：

```bash
winget install Hugo.Hugo.Extended
```

### macOS 用户

使用 Homebrew：

```bash
brew install hugo
```

### Linux 用户

```bash
sudo apt install hugo  # Ubuntu/Debian
sudo yum install hugo  # CentOS/RHEL
```

## 创建新站点

```bash
hugo new site my-website
cd my-website
```

## 添加主题

Hugo 有丰富的主题生态系统。推荐使用 Git 子模块方式安装：

```bash
git init
git submodule add https://github.com/adityatelange/hugo-PaperMod.git themes/PaperMod
```

在 `hugo.toml` 中配置主题：

```toml
theme = 'PaperMod'
```

## 创建内容

创建新文章：

```bash
hugo new content posts/my-post.md
```

## 本地预览

启动开发服务器：

```bash
hugo server --buildDrafts
```

访问 `http://localhost:1313` 预览网站。

## 构建网站

生成静态文件：

```bash
hugo
```

生成的文件将保存在 `public/` 目录中。

## 部署选项

Hugo 生成的静态网站可以部署到多个平台：

- **Cloudflare Pages** - 免费，CDN 加速
- **Netlify** - 免费套餐，CI/CD 集成
- **GitHub Pages** - 免费，与 GitHub 深度集成
- **Vercel** - 适合前端项目

## 小贴士

1. **使用 Draft 模式** - 开发时设置 `draft = true`
2. **优化图片** - 使用适当的图片格式和尺寸
3. **SEO 优化** - 设置好 title、description 等元数据
4. **定期备份** - 使用 Git 管理源码

## 总结

Hugo 是一个强大而灵活的静态网站生成器，适合构建博客、文档站点和企业网站。其快速的构建速度和丰富的功能使其成为静态网站的理想选择。

开始你的 Hugo 之旅吧！
