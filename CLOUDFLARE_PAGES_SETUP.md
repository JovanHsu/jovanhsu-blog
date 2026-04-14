# Cloudflare Pages 配置参考

## GitHub 集成设置

1. 访问 https://pages.cloudflare.com
2. 点击 "Create a project"
3. 选择 "Connect to Git"
4. 选择仓库 `JovanHsu/jovanhsu-blog`
5. 选择分支 `main`

## 构建配置

- **Project name:** jovanhsu-blog
- **Production branch:** main
- **Framework preset:** Hugo
- **Build command:** `hugo --theme=introduction` (或留空，Cloudflare 会自动检测 Hugo)
- **Build output directory:** `public`
- **Root directory:** `/`

## 环境变量 (如有需要)

- HUGO_VERSION: 0.160.1

## 自定义域名

- 域名: blog.narsk.sbs
- 在 Cloudflare DNS 中添加 CNAME 记录指向 pages.cloudflare.com
- 在 Pages 设置中添加自定义域名
