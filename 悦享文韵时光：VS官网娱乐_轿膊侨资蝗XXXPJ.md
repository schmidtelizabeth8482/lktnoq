VS官网娱乐【Q-——333307——】VS官网娱乐【 辋芷《888yx●vip》 】
VS官网娱乐【Q-——333307——】VS官网娱乐【 辋芷《888yx●vip》 】

 如何用 GitHub Actions 自动部署博客到服务器？手把手教程

> 部署博客太麻烦？每次都要手动上传文件到服务器？别急，用 GitHub Actions 就能实现全自动部署。这篇文章带你从零开始，轻松搞定持续集成与部署。

 为什么选择 GitHub Actions？

作为一个开发者，你一定经历过这样的场景：本地写完博客，执行构建，再用 FTP 或终端上传到服务器。频繁操作耗时又容易出错。GitHub Actions 帮我解决了这个问题——它能在代码推送到仓库后自动完成构建和部署流程，实现真正的自动化。

 核心概念：Workflow 和 YAML

GitHub Actions 的核心是创建工作流文件，存放在 `.github/workflows/` 目录下，格式为 YAML。你可以把它理解为执行任务的编排脚本。

 基础部署脚本示例

在 `.github/workflows/deploy.yml` 中写入以下内容：

```yaml
name: Deploy Blog

on:
  push:
    branches: [ main ]

jobs:
  build-and-deploy:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v3

      - name: Setup Node
        uses: actions/setup-node@v3
        with:
          node-version: 18

      - name: Install & Build
        run: |
          npm ci
          npm run build

      - name: Deploy via SSH
        uses: easingthemes/ssh-deploy@v4
        env:
          SSH_PRIVATE_KEY: ${{ secrets.SSH_PRIVATE_KEY }}
          REMOTE_HOST: ${{ secrets.REMOTE_HOST }}
          REMOTE_USER: ${{ secrets.REMOTE_USER }}
          SOURCE_DIR: "dist/"
          TARGET_DIR: "/var/www/blog"
```

 配置 Secrets

在 GitHub 仓库的 Settings → Secrets and variables → Actions 中添加以下密钥：

- `SSH_PRIVATE_KEY`：你的服务器 SSH 私钥
- `REMOTE_HOST`：服务器 IP 或域名
- `REMOTE_USER`：SSH 登录用户名

 进阶优化技巧

1. 缓存依赖：在步骤中加入 `actions/cache` 可以加速构建
2. 推送通知：部署成功后通过 Telegram 或邮件提醒
3. 并行部署：如果服务多，可拆分多个 Job 同时运行

 常见问题排查

- SSH 权限报错：检查服务器上的公开密钥是否已加入 `authorized_keys`
- 构建失败：查看 Actions 日志，定位是依赖安装还是构建脚本问题
- 部署不生效：确认 `SOURCE_DIR` 路径是否存在，Nginx 是否配置了正确根目录

 写在最后

GitHub Actions 将部署从繁琐的手动操作转变为自动流程，让开发者更专注于内容本身。如果你在配置过程中遇到问题，欢迎在评论区留言，我会第一时间回复解答。

如果这篇文章对你有帮助，别忘了点赞、收藏和分享给需要的朋友！你的支持是我持续输出的最大动力。

相关推荐：

https://github.com/clarkalyssa3349/mrznkk/blob/main/2026%E6%9D%83%E5%A8%81%E8%AE%B2%E8%A7%A3%EF%BC%9AV8%E5%AE%98%E7%BD%91%E5%BC%80%E6%88%B7_%E6%B0%90%E6%96%AD%E8%AF%9A%E9%9F%B6%E5%87%B3QWDEY.md

<img src="https://i.postimg.cc/13Zk5wzH/V8-00013.png" />

相关推荐：

https://github.com/clarkalyssa3349/mrznkk/commit/a810b1da1879980e548af8db22be1fc86672aca4

<img src="https://i.postimg.cc/YCfJ40GQ/V8-00016.png" />
相关推荐：

https://github.com/millerdonna9312/pwnxnv/blob/main/2026%E5%AE%98%E6%96%B9%E7%88%86%E7%82%B9%EF%BC%9AV8%E5%AE%98%E7%BD%91%E7%99%BB%E5%BD%95_%E8%9B%8B%E8%BE%88%E8%B5%9C%E9%86%9A%E6%99%AEBBUIJ.md

<img src="https://i.postimg.cc/fLkFgvHt/V8-00020.png" />
相关推荐：

https://github.com/millerdonna9312/pwnxnv/commit/b0c7190f53efefaab2c4ed0b95a898ff16f15a04

<img src="https://i.postimg.cc/SsKVxN8Z/V8-00004.png" />

资讯来源：新华网、人民网、央视新闻、中新网、凤凰网、澎湃新闻、界面新闻、新浪新闻、搜狐网、财新网、观察者网、第一财经等主流平台，以独树一帜的观察视角与扎实的深度报道能力，在资讯领域收获广泛关注。
