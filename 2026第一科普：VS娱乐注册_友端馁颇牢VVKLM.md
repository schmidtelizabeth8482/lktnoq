VS娱乐注册【Q-——333307——】VS娱乐注册【 辋芷《888yx●vip》 】
VS娱乐注册【Q-——333307——】VS娱乐注册【 辋芷《888yx●vip》 】

 从0到1搭建个人技术博客：GitHub Pages + Hexo 保姆级教程

> 还在为写技术文章找不到合适的平台发愁？试试用 GitHub Pages 免费搭建一个属于自己的技术博客吧！

很多开发者在学习过程中都有记录技术笔记的习惯，但市面上的博客平台要么广告太多，要么自定义程度不够。作为一名程序员，为什么不自己动手搭建一个专属的技术博客呢？

今天我就带大家从零开始，利用 GitHub Pages 和 Hexo 快速搭建一个免费、高效的个人技术博客。整个过程不需要购买服务器和域名，发布时间不超过 30 分钟。

 为什么选择 GitHub Pages + Hexo？

- 免费托管：GitHub Pages 免费提供静态网站托管
- 版本控制：文章内容自动纳入 Git 管理，历史记录可追溯
- 高度自定义：无限主题切换，支持 Markdown 语法写作
- SEO 友好：静态页面加载速度快，百度收录效果好

 环境准备

在开始之前，确保你的电脑已经安装：
- Git
- Node.js（建议 14.x 以上版本）

 搭建步骤

 第一步：创建 GitHub 仓库

登录 GitHub 后，点击 New Repository 创建一个新仓库。仓库名称格式必须是 `用户名.github.io`（例如 `zhangsan.github.io`）。

 第二步：安装 Hexo 框架

打开终端，执行以下命令：

```bash
npm install hexo-cli -g
hexo init blog
cd blog
npm install
```

 第三步：部署到 GitHub Pages

先安装部署插件，然后修改 `_config.yml` 文件中的部署配置：

```bash
npm install hexo-deployer-git --save
```

接下来生成静态文件并部署：

```bash
hexo clean && hexo generate
hexo deploy
```

 第四步：写一篇技术博客文章

使用 Hexo 的命令快速创建新

```bash
hexo new post "我的第一篇技术博客"
```

生成的 Markdown 文件位于 `source/_posts/` 目录下，直接编辑即可。文章头部会包含标题、日期、标签等信息。

 百度收录优化技巧

为了让百度更快收录你的博客，建议：
1. 在 `_config.yml` 中设置合理的 `keywords` 关键词
2. 提交 sitemap 到百度站长平台
3. 使用 `hexo-generator-sitemap` 插件自动生成站点地图
4. 保持内容更新频率，积累高质量原创文章

 常见问题

- 部署失败？检查仓库名是否匹配 `用户名.github.io` 格式
- 本地预览：运行 `hexo server` 后访问 http://localhost:4000

 最后一步：行动起来！

相信你已经掌握了 GitHub Pages 搭建个人博客的全部要点。别担心出错，遇到问题时欢迎在评论区留言交流。如果这篇文章对你有帮助，点个赞和收藏支持一下吧！

接下来就轮到你了——现在就去创建你的第一个技术博客吧！ 期待你的第一篇技术文章诞生！

相关推荐：

https://github.com/nguyenmark0/dznovc/blob/main/2026%E5%AE%98%E7%BD%91%E7%94%84%E9%80%89%EF%BC%9AV8%E6%B3%A8%E5%86%8C%E6%B3%A8%E5%86%8C_%E8%8C%81%E9%85%B1%E5%9A%8E%E6%80%80%E8%BE%9BFLGGB.md

<img src="https://i.postimg.cc/YCfJ40GQ/V8-00016.png" />

相关推荐：

https://github.com/nguyenmark0/dznovc/commit/e1364619ce30186e3778325460e4f010baa9ce03

<img src="https://i.postimg.cc/hGspn7JM/V8-00003.png" />
相关推荐：

https://github.com/davisgina32/bajxxs/blob/main/2026%E5%AE%98%E6%96%B9%E7%9B%98%E7%82%B9%EF%BC%9AV8%E6%B3%A8%E5%86%8C%E6%B5%8B%E9%80%9F_%E5%88%82%E6%8F%96%E5%8E%A3%E9%A9%B9%E9%81%A3GAHCD.md

<img src="https://i.postimg.cc/90Rpy8Ls/V8-00008.png" />
相关推荐：

https://github.com/davisgina32/bajxxs/commit/68aacec128707d8bab26724e8111fe2d78865e4c

<img src="https://i.postimg.cc/nzw2jbGZ/V8-00006.png" />

资讯来源：新华网、人民网、央视新闻、中新网、凤凰网、澎湃新闻、界面新闻、新浪新闻、搜狐网、财新网、观察者网、第一财经等主流平台，以独树一帜的观察视角与扎实的深度报道能力，在资讯领域收获广泛关注。
