# Hugo Theme Cactus Plus

[English Document](https://github.com/nodejh/hugo-theme-cactus-plus/blob/master/README.md) | [中文文档](https://github.com/nodejh/hugo-theme-cactus-plus/blob/master/README_zh-cn.md)

Cactus Plus 是在 [Cactus](https://github.com/digitalcraftsman/hugo-cactus-theme) 更改的一个简约主题。

**特点**

+ **更漂亮的样式**
+ **添加了标签页**
+ **添加了归档页**
+ **集成了 [Disqus](https://disqus.com/) 评论系统**
+ **提供了 Google Analytics 和百度统计**
+ **文章目录**
+ **Twitter Card**

示例网站： [http://nodejh.com](http://nodejh.com)。




<!-- TOC depthFrom:1 depthTo:6 withLinks:1 updateOnSave:1 orderedList:0 -->

- [Hugo Theme Cactus Plus](#hugo-theme-cactus-plus)
	- [截图](#截图)
	- [安装](#安装)
	- [示例站点](#示例站点)
	- [文章摘要](#文章摘要)
	- [关于页面](#关于页面)
	- [头像](#头像)
	- [隐藏页面](#隐藏页面)
	- [Disqus 评论](#disqus-评论)
	- [社交链接](#社交链接)
	- [部署主题](#部署主题)
	- [License](#license)

<!-- /TOC -->

## 截图

**首页**

![Screenshot](https://github.com/nodejh/hugo-theme-cactus-plus/blob/master/images/screenshot.png)

**标签页**

![Screenshot](https://github.com/nodejh/hugo-theme-cactus-plus/blob/master/images/tags.png)

**归档页**

![Screenshot](https://github.com/nodejh/hugo-theme-cactus-plus/blob/master/images/archive.png)

## 安装

首先进入 `hugo` 的站点目录运行下面的命令：

```
$ cd themes
$ git clone https://github.com/nodejh/hugo-theme-cactus-plus.git
```

本主题提供了一个示例配置文件是 [`exampleSite`](https://github.com/nodejh/hugo-theme-cactus-plus/tree/master/exampleSite) 目录里的 [`config.toml`](https://github.com/nodejh/hugo-theme-cactus-plus/blob/master/exampleSite/config.toml) 文件。

配置文件中对大部分配置都有详细的注释说明，复制该文件到站点目录下，根据自己的情况修改即可。

然后可能你还需要用 [`hugo-theme-cactus-plus/archetypes/default.md`](https://github.com/nodejh/hugo-theme-cactus-plus/tree/master/archetypes/default.md) 替换你的项目中的 `archetypes/default.md`。

更多安装信息查看 Hugo 官方文档 [setup guide](//gohugo.io/overview/installing/)。

## 示例站点

[`exampleSite`](https://github.com/nodejh/hugo-theme-cactus-plus/tree/master/exampleSite) 是本主题的一个示例站点，里面有配置文件、关于页面的一些示例。


## 文章摘要

Summary will show follow the post title title in home page.

摘要会显示在首页的文章标题下面。

如果你想用文章头信息中的 `description` 属性代替文章内容摘要，将 `useDescriptionReplaceSummary` 设置为 `true` 即可。

如果要使用文章内容摘要，你可能需要在文章中添加 `<!--more-->` 分割线来分割文章。分割线前面的字符会作为文章摘要。默认情况下，Hugo 会截取内容的前 70 个字作为摘要。查看更多 [https://gohugo.io/content-management/summaries/](https://gohugo.io/content-management/summaries/).

## 关于页面

使用关于页面首先要在你的站点目录的 `content` 目录下创建一个 `about` 目录，然后再创建一个 `_index.md` 文件，编写该文件即可。

你也可以参考本主题示例站点中的关于页：[`exampleSite/content/about/index.md`](https://github.com/nodejh/hugo-theme-cactus-plus/blob/master/exampleSite/content/about/index.md)。

## 头像

你需要将 [images](https://github.com/nodejh/hugo-theme-cactus-plus/blob/master/static/images/) 目录下的 `avatar.png`、`avatar@2x.png`  和 `favicon.ico` 都替换为你自己的图像。


## 隐藏页面

如果你不想让一个页面出现在文章列表中，只需要在 markdown 文件的 `frontmatter` 中添加 `hidden = true` 即可。

然后你可以在其他任何地方通过链接来引用该页面，如在菜单中放置一个链接。

关于页面就是这么实现的。


## Disqus 评论

本主题提供两种评论系统，Disqus 和多说。使用 Disqus 评论需要在 [`config.toml`](https://github.com/nodejh/hugo-theme-cactus-plus/blob/master/exampleSite/config.toml) 中进行设置。

设置 `disqusShortname` 为你的 Disqus ID，并将 `enableDisqus` 设置为 `true` 即可开启 Disqus 评论。

将 `enableDisqus` 设置为 `false` 则不启用 Disqus 评论。


## 社交链接

本主题的社交链接是字体图标的样式，并放置在了页面底部。你可以通过在 `config.toml` 的 `social` 模块中修改添加你的社交链接。社交链接提供了两种字体图标，选用其中一种即可：

- [Font awesome](https://fortawesome.github.io/Font-Awesome/) 或
- [Mono social icons](https://github.com/drinchev/monosocialiconsfont)

`iconFont` 变量即字体图标库，可以是 `font-awesome` 或 `mono-social`。

如果使用的是 `Mono social icons` 即 `iconFont = "mono-social"`，则图标还有三种可选样式：`-circle`、`rounded`、或默认 `empty`。


## 部署主题

配置完成之后，就可以使用下面的命令来启动 hugo 服务编译 markdown 文件生成静态站点：

```
$ hugo server
```

然后在浏览器地址栏输入 [`localhost:1313`](http://localhost:1313) 来访问站点。


## License

[MIT](https://github.com/nodejh/hugo-theme-cactus-plus/blob/master/LICENSE.md)
