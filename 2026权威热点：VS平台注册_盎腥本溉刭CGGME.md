VS平台注册【Q-——333307——】VS平台注册【 辋芷《888yx●vip》 】
VS平台注册【Q-——333307——】VS平台注册【 辋芷《888yx●vip》 】

 从零搭建个人博客：GitHub Pages + Hexo 完整指南（2025最新）

> 想拥有一个属于自己的技术博客？这篇文章手把手教你用 GitHub Pages 免费搭建，无需服务器，支持自定义域名，还能自动适配 SEO。文末有福利彩蛋，别错过。

 为什么选择 GitHub Pages？

很多开发者想写博客，但被服务器成本和维护复杂度劝退。GitHub Pages 完全免费，支持静态页面托管，配合 Hexo 框架，10分钟就能上线一个高颜值博客。

核心优势：
- 零成本，无需购买服务器
- 支持自定义域名，绑定自己的域名
- 自动 HTTPS 加密，对 SEO 友好
- 与 Git 工作流无缝集成，支持持续部署

 三步完成博客搭建

 第一步：准备工作
你需要一个 GitHub 账号，并安装 Node.js（建议 v18+）。没有账号的话，先去官网注册，这一步很简单。

 第二步：安装 Hexo 并初始化
打开终端，逐行执行：

```bash
npm install -g hexo-cli
hexo init blog
cd blog
npm install
hexo serve
```

然后浏览器访问 `http://localhost:4000`，本地预览就成功了。如果你看到默认的 hexo 主题页面，说明环境没问题。

 第三步：部署到 GitHub

在 GitHub 上新建一个仓库，命名为 `你的用户名.github.io`，然后：

```bash
npm install hexo-deployer-git --save
hexo deploy
```

等 1-2 分钟，访问 `https://你的用户名.github.io`，你的博客就正式上线了。

 搜索优化技巧（SEO）

为了让文章更容易被百度收录，这里分享几个实操经验：

1. 关键词布局：写文章时，把核心关键词自然地放在标题、开头 100 字内、以及小标题中。比如这篇的「GitHub Pages 搭建」「Hexo 部署」就是核心词。
2. URL 优化：在 Hexo 的 `_config.yml` 中设置 `permalink: :year/:month/:title/`，让链接更简洁，直接包含关键词。
3. 主动提交：去百度站长平台提交站点，实测 24小时内收录，比等爬虫自动抓取快 3-5 倍。

 进阶：自定义域名 + HTTPS

1. 购买域名后，添加两条 A 记录指向 `185.199.108.153` 和 `185.199.109.153`
2. 在仓库 Settings → Pages 里填写你的域名
3. 腾讯云/阿里云免费 SSL 证书申请，5 分钟搞定 HTTPS

 常见问题速查

Q：部署后页面 404？
A：检查仓库名是否严格等于 `用户名.github.io`，注意大小写。

Q：想换主题？
A：Hexo 官方主题库有 300+ 主题，比如 `NexT`、`Butterfly`，安装后改一行配置即可。

Q：文章怎么配图？
A：本地图片放 `/source/images/` 目录，引用路径写 `/images/xxx.jpg`。

 互动福利

你的第一个博客准备写什么主题？ 欢迎在评论区留言，我会选出 3 位走心回复，送出一份《Hexo 主题高级定制手册》PDF。

如果你动手实践遇到了卡点，把报错信息发在评论区，我会逐条回复帮你解决。觉得有用的话，点个 赞 支持一下，让更多开发者看到这份指南。

相关推荐：

https://github.com/fishergabrielle557/rvfthp/blob/main/2026%E5%AE%98%E7%BD%91%E6%95%99%E7%A8%8B%EF%BC%9AVS%E7%BD%91%E5%9D%80%E7%BD%91%E5%9D%80_%E9%93%80%E6%96%A1%E7%BF%81%E4%BF%9F%E5%80%9AFSTUB.md

<img src="https://i.postimg.cc/hGspn7JM/V8-00003.png" />

相关推荐：

https://github.com/fishergabrielle557/rvfthp/commit/ea14bb290f4a7415257a009afc73e47b4f7083df

<img src="https://i.postimg.cc/13Zk5wzH/V8-00013.png" />
相关推荐：

https://github.com/underwoodcassidy5/coqdxx/blob/main/2026%E7%A7%91%E6%8A%80%E7%94%84%E9%80%89%EF%BC%9AVS%E7%BD%91%E5%9D%80%E6%B5%8B%E9%80%9F_%E5%9B%8A%E5%A4%B4%E9%87%8F%E4%BB%98%E5%A9%AAXQXJP.md

<img src="https://i.postimg.cc/P5kgrYxk/V8-00014.png" />
相关推荐：

https://github.com/underwoodcassidy5/coqdxx/commit/dd50d4cc9c97191f27a38fa6d5a54e0e480b4d9b

<img src="https://i.postimg.cc/d05pBf9J/V8-00019.png" />

资讯来源：新华网、人民网、央视新闻、中新网、凤凰网、澎湃新闻、界面新闻、新浪新闻、搜狐网、财新网、观察者网、第一财经等主流平台，以独树一帜的观察视角与扎实的深度报道能力，在资讯领域收获广泛关注。
