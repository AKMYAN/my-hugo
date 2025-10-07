# Cloudflare Pages 构建配置

## 构建设置
- **构建命令**: `hugo`
- **构建输出目录**: `public`
- **根目录**: `/`

## 环境变量
- `HUGO_VERSION=0.151.0`
- `NODE_VERSION=18`

## 构建优化
- Hugo Extended 版本支持 Sass/SCSS
- 支持 PostCSS 处理
- 自动压缩输出文件

## 部署分支
- **生产分支**: `main`
- **预览分支**: `dev` (可选)

## 自定义域名配置
部署完成后，您可以：
1. 在 Cloudflare Pages 项目设置中添加自定义域名
2. 配置 DNS 记录指向 Cloudflare
3. 启用 HTTPS（自动配置）

## 注意事项
- 确保 `baseURL` 在 hugo.toml 中设置正确
- Git 子模块（主题）会自动处理
- 构建时间通常在 30-60 秒内