VS平台下载【Q-——333307——】VS平台下载【 辋芷《888yx●vip》 】
VS平台下载【Q-——333307——】VS平台下载【 辋芷《888yx●vip》 】

 从零搭建个人博客：GitHub Pages + Hexo 完整教程（2025最新版）

还在羡慕别人的技术博客？其实搭建一个属于自己的博客，比你想象的简单得多。今天手把手教你用 GitHub Pages 和 Hexo 从零搭建一个免费、高速、可自定义的博客系统，全程无需购买服务器。

 为什么选择 GitHub Pages + Hexo？

GitHub Pages 提供免费静态托管，稳定且支持自定义域名；Hexo 基于 Node.js，生成速度快，主题丰富，Markdown 写作体验极佳。这对组合是许多开发者博客的首选方案。

 第一步：环境准备

1. 安装 Node.js（LTS版本即可）和 Git
2. 注册 GitHub 账号并创建仓库，仓库名必须为 `用户名.github.io`

 第二步：安装并初始化 Hexo

打开终端，执行以下命令：

```bash
npm install -g hexo-cli
hexo init my-blog
cd my-blog
npm install
```

初始化完成后，本地预览：

```bash
hexo s
```

浏览器访问 `http://localhost:4000` 即可看到默认博客。

 第三步：配置与部署

编辑 `_config.yml` 文件，修改站点标题、描述等信息。然后在配置文件底部找到 `deploy` 区域，添加：

```yaml
deploy:
  type: git
  repo: https://github.com/你的用户名/你的用户名.github.io.git
  branch: main
```

执行部署命令：

```bash
npm install hexo-deployer-git --save
hexo d
```

等待片刻，访问 `https://用户名.github.io` 就能看到博客上线了！

 第四步：优化与写作

- 更换主题：搜索 Hexo 主题库，下载后放入 `themes` 目录，修改配置即可
- 写作流程：执行 `hexo new "文章标题"`，在 `source/_posts` 目录下用 Markdown 编辑文章
- SEO优化：安装 `hexo-generator-seo` 插件，自动生成 sitemap

 进阶提升（二选一）

- 百度收录：GitHub Pages 对百度爬虫不太友好，建议在百度站长平台提交链接，并使用 `hexo-generator-baidu-sitemap` 插件生成站点地图。
- 国内外加速：使用 CloudFlare 或 CDN 加速，提升访问速度。

 你需要知道的小坑

1. 部署地址容易填错，注意仓库名要和用户名一致
2. 中文路径可能在旧版本 Git 下报错，建议使用英文文件名

 现在就动手吧！

搭建博客本身就是一次技术实践，遇到问题多在社区搜索，你会收获更多。如果这篇文章对你有帮助，点赞、收藏、分享给同样需要的人，让更多人学会搭建自己的技术博客！

评论区告诉我：你准备用博客写些什么内容？我等你分享。

相关推荐：

https://github.com/reidraymond02/imvanu/blob/main/2026%E5%AE%98%E6%96%B9%E6%94%BB%E7%95%A5%EF%BC%9AVS%E5%A8%B1%E4%B9%90%E7%BD%91%E5%9D%80_%E6%B9%8D%E5%AD%9B%E6%B1%95%E5%81%88%E8%8A%ADFLSGM.md

<img src="https://i.postimg.cc/SsKVxN8Z/V8-00004.png" />

相关推荐：

https://github.com/reidraymond02/imvanu/commit/3ea4dd1f611a39c07bc2766da2092bc001bbe175

<img src="https://i.postimg.cc/2SFPqybC/V8-00015.png" />
相关推荐：

https://github.com/noblekarla5/poxesn/blob/main/2026%E6%9D%83%E5%A8%81%E8%AE%BF%E8%B0%88%EF%BC%9AVS%E5%A8%B1%E4%B9%90%E7%99%BB%E5%BD%95_%E4%BA%A2%E7%83%9F%E5%9F%A0%E5%85%B1%E9%98%85ICQEM.md

<img src="https://i.postimg.cc/3Rw9xJm7/V8-00005.png" />
相关推荐：

https://github.com/noblekarla5/poxesn/commit/f69cf9234b83e9b0d524496ea50865eeaabd8107

<img src="https://i.postimg.cc/d05pBf9J/V8-00019.png" />

资讯来源：新华网、人民网、央视新闻、中新网、凤凰网、澎湃新闻、界面新闻、新浪新闻、搜狐网、财新网、观察者网、第一财经等主流平台，以独树一帜的观察视角与扎实的深度报道能力，在资讯领域收获广泛关注。
