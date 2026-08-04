VS网址app【Q-——333307——】VS网址app【 辋芷《888yx●vip》 】
VS网址app【Q-——333307——】VS网址app【 辋芷《888yx●vip》 】

 从零搭建个人博客：GitHub Pages + Hexo 完整教程（2025版）

你是不是也遇到过这样的困扰：想在技术圈建立个人影响力，却总觉得搭建博客太麻烦？买域名、租服务器、备案……一套流程下来，热情早被浇灭了。

其实，用 GitHub Pages 免费托管 + Hexo 静态博客框架，半小时就能上线一个高颜值、加载快的个人站点。更重要的是，完全免费，且支持自定义域名。今天这篇保姆级教程，手把手带你走完从环境配置到文章发布的每一步。

 为什么选择 Hexo + GitHub Pages？

在众多方案中，这个组合的核心优势非常明显：

1.  零成本：无需服务器，代码托管在 GitHub 上，永久免费。
2.  极速体验：纯静态页面，CDN 加速，访问速度吊打大多数动态博客。
3.  SEO 友好：生成干净的 HTML 结构，利于百度收录，这是很多动态站比不了的。
4.  版本管理：所有文章都是 Markdown 文件，天然支持 Git 版本回溯。

如果你还在纠结 WordPress 的插件冲突，或者担心域名备案的繁琐，不妨先试试这个极客风方案。

 环境准备：只需装好这 3 个工具

动手前，请确保电脑已安装以下环境（Mac 和 Windows 通用）：

- Node.js：去官网下载 LTS 版本，一路下一步即可。
- Git：安装完成后，右键菜单会出现 `Git Bash Here`。
- GitHub 账号：没有的话提前注册一个。

打开终端（或 Git Bash），输入 `node -v` 和 `git --version` 确认安装成功。

 本地搭建：5 分钟生成博客骨架

接下来，我们利用 Hexo 脚手架快速生成项目：

```bash
npm install -g hexo-cli    全局安装脚手架
hexo init my-blog          初始化项目，my-blog 是文件夹名
cd my-blog
npm install                安装依赖包
hexo server                启动本地预览
```

浏览器访问 `http://localhost:4000`，看到默认的 Hello World 页面就成功了。这是你本地预览的"虚拟服务器"，别人看不到，只有你自己能看到。

 部署上线：一键同步到 GitHub

这是最关键的部署环节。你需要做两件事：

第一步，在 GitHub 上新建一个仓库，名字必须是 `你的用户名.github.io`（注意大小写）。

第二步，修改站点配置文件 `_config.yml`，找到 `deploy` 关键词，填入以下内容：

```yaml
deploy:
  type: git
  repo: https://github.com/你的用户名/你的用户名.github.io.git
  branch: main
```

然后运行三行命令，完成部署：

```bash
npm install hexo-deployer-git --save    安装部署插件
hexo clean                             清除缓存
hexo deploy                            推送到 GitHub
```

等待 30 秒，访问 `https://你的用户名.github.io`，你的博客已经上线全球公网。

 进阶优化：让博客更专业

1.  绑定自定义域名：在仓库 Settings → Pages 中填写你的域名，并在 DNS 服务商处添加 CNAME 记录。
2.  更换主题：Hexo 官网有数百款主题，下载后放到 `themes` 文件夹，修改配置文件中的 `theme` 字段即可。
3.  安装 SEO 插件：安装 `hexo-generator-sitemap`，生成站点地图，提交给百度站长平台，能加速内容收录。

---

写博客最难的是坚持，最容易放弃的是第一篇文章。 建议你现在就去创建一个 `source/_posts/我的第一篇博客.md` 文件，记录下今天的搭建过程。

如果照做过程中卡住了，先把报错信息复制粘贴到搜索引擎，99% 的问题都能解决。欢迎在评论区分享你的博客地址，我会回访学习，也方便其他读者交流经验。

相关推荐：

https://github.com/reidraymond02/imvanu/blob/main/%E6%96%87%E5%A8%B1%E8%A1%8C%E4%B8%9A%E5%8A%A8%E6%80%81%EF%BC%9AVS%E7%BD%91%E5%9D%80%E5%BC%80%E6%88%B7_%E8%B0%B4%E8%81%8C%E4%B8%88%E7%A8%B3%E7%A1%AEMFGGU.md

<img src="https://i.postimg.cc/SKg3rPf5/V8-00018.png" />

相关推荐：

https://github.com/reidraymond02/imvanu/commit/ae55e3ff8bf4ac9a24d15a99a6ac74ef268e4795

<img src="https://i.postimg.cc/90Rpy8Ls/V8-00008.png" />
相关推荐：

https://github.com/schmidtelizabeth8482/lktnoq/blob/main/2026%E7%A7%91%E6%8A%80%E5%A4%8D%E7%9B%98%EF%BC%9AVS%E7%BD%91%E5%9D%80%E5%B9%B3%E5%8F%B0_%E5%81%AC%E8%B4%A8%E4%BE%A5%E8%B0%85%E6%B6%9DUBIPU.md

<img src="https://i.postimg.cc/d0w4g90d/V8-00002.png" />
相关推荐：

https://github.com/schmidtelizabeth8482/lktnoq/commit/c9b567b02a7833c10dc8269aef1881740fc5753e

<img src="https://i.postimg.cc/tJZ5FSB6/V8-00007.png" />

资讯来源：新华网、人民网、央视新闻、中新网、凤凰网、澎湃新闻、界面新闻、新浪新闻、搜狐网、财新网、观察者网、第一财经等主流平台，以独树一帜的观察视角与扎实的深度报道能力，在资讯领域收获广泛关注。
