# 我的 Hugo 博客

这是一个使用 Hugo 静态网站生成器构建的个人博客网站。

## 特性

- ⚡ 使用 Hugo 构建，速度超快
- 🎨 采用 PaperMod 主题，界面简洁美观
- 📱 响应式设计，支持移动设备
- 🚀 部署在 Cloudflare Pages，全球 CDN 加速
- 📝 支持 Markdown 写作

## 技术栈

- **静态网站生成器**: [Hugo](https://gohugo.io/)
- **主题**: [PaperMod](https://github.com/adityatelange/hugo-PaperMod)
- **部署平台**: [Cloudflare Pages](https://pages.cloudflare.com/)
- **版本控制**: Git + GitHub

## 本地开发

### 安装 Hugo

Windows (使用 winget):
```bash
winget install Hugo.Hugo.Extended
```

macOS (使用 Homebrew):
```bash
brew install hugo
```

### 克隆仓库

```bash
git clone https://github.com/AKMYAN/my-hugo.git
cd my-hugo
git submodule update --init --recursive
```

### 本地预览

```bash
hugo server
```

网站将在 `http://localhost:1313` 运行。

### 构建网站

```bash
hugo
```

生成的静态文件将保存在 `public/` 目录中。

## 部署

网站通过 Cloudflare Pages 自动部署。每次推送到 `main` 分支时，都会自动触发构建和部署。

### 构建配置

- **构建命令**: `hugo`
- **构建输出目录**: `public`
- **根目录**: `/`

## 添加新文章

```bash
hugo new content posts/new-post.md
```

编辑生成的 Markdown 文件，设置 `draft = false` 后即可发布。

## 目录结构

```
.
├── archetypes/          # 内容模板
├── content/             # 网站内容
│   ├── posts/          # 博客文章
│   └── about.md        # 关于页面
├── themes/             # 主题文件
├── static/             # 静态资源
├── hugo.toml           # Hugo 配置文件
└── README.md           # 项目说明
```

## 许可证

MIT License

## 联系方式

- GitHub: [@AKMYAN](https://github.com/AKMYAN)
- Website: [blog.926948.xyz](https://blog.926948.xyz)
- Email: one@ztmy.net