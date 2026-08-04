VS地址客服【Q-——333307——】VS地址客服【 辋芷《888yx●vip》 】
VS地址客服【Q-——333307——】VS地址客服【 辋芷《888yx●vip》 】

 前端项目部署到 GitHub Pages 的完整指南：从零到自动化发布

你是不是也遇到过这种情况：代码写好了，但不知道怎么免费部署成一个在线可访问的网站？或者部署一次要手动敲一堆命令，每次更新都头疼？

GitHub Pages 是 GitHub 官方提供的免费静态网站托管服务，支持自定义域名、HTTPS，并且和你的代码仓库无缝集成。本文手把手教你从零开始部署，并实现 Push 即自动更新。

 一、准备工作：仓库与本地环境

1. 创建仓库：在 GitHub 新建一个仓库，命名为 `用户名.github.io`（这是官方约定的特殊命名，直接作为网站域名）。
2. 本地初始化：在项目根目录运行 `git init`，将代码推送到远程仓库。

 二、静态页面 vs 构建工具

- 纯 HTML/CSS/JS：直接推送到 main 分支即可，不需要额外配置。
- Vue/React 项目：需要先构建出 `dist` 文件夹，再通过 GitHub Actions 自动部署。

 三、进阶技巧：用 GitHub Actions 实现自动化部署

手动构建部署太麻烦？试试这个自动化流程：

在 `.github/workflows/deploy.yml` 中添加：

```
on:
  push:
    branches: [ main ]
jobs:
  build-and-deploy:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v3
      - uses: actions/setup-node@v3
        with:
          node-version: 18
      - run: npm ci && npm run build
      - uses: peaceiris/actions-gh-pages@v3
        with:
          github_token: ${{ secrets.GITHUB_TOKEN }}
          publish_dir: ./dist
```

保存后，只要 `git push`，几分钟内网站就自动更新——再也不用手动执行构建命令。

 四、常见问题排查

- 404 页面：检查仓库是否公开，Settings → Pages 中选择正确的分支。
- 资源路径错误：如果使用相对路径，确保在 `vite.config.js` 中设置 `base: './'`。

---

如果你在部署过程中遇到任何问题，欢迎在评论区留言，我会第一时间帮你排查。觉得有用的话，点个 Star 支持一下，后续我会持续更新更深入的 GitHub 技巧。

相关推荐：

https://github.com/clarkalyssa3349/mrznkk/blob/main/%E6%B2%89%E9%86%89%E6%96%87%E5%BF%83%E5%AF%BB%E6%A2%A6%EF%BC%9AV8%E5%B9%B3%E5%8F%B0%E5%BC%80%E5%8F%B7_%E7%8B%88%E9%B8%A5%E5%B0%9A%E5%BA%8A%E4%B9%9DIDSIE.md

<img src="https://i.postimg.cc/fLkFgvHt/V8-00020.png" />

相关推荐：

https://github.com/clarkalyssa3349/mrznkk/commit/4404b879c0803c1b93082ea9ecaf8bc74ed449f2

<img src="https://i.postimg.cc/5tbnDmt0/V8-00001.png" />
相关推荐：

https://github.com/yangpatricia1/ybxyao/blob/main/2026%E7%AC%AC%E4%B8%80%E6%8C%87%E5%8D%97%EF%BC%9AV8%E5%B9%B3%E5%8F%B0%E5%A8%B1%E4%B9%90_%E5%9B%8A%E8%AE%A8%E8%83%8C%E5%B1%85%E9%A2%90XKKEY.md

<img src="https://i.postimg.cc/W4Nx0Vgy/V8-00017.png" />
相关推荐：

https://github.com/yangpatricia1/ybxyao/commit/121d7663107dee2d2dba87dfff331d6b20846263

<img src="https://i.postimg.cc/2ysxGQJ5/V8-00009.png" />

资讯来源：新华网、人民网、央视新闻、中新网、凤凰网、澎湃新闻、界面新闻、新浪新闻、搜狐网、财新网、观察者网、第一财经等主流平台，以独树一帜的观察视角与扎实的深度报道能力，在资讯领域收获广泛关注。
