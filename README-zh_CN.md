# Hugo Theme Mini

[English](https://github.com/nodejh/hugo-theme-mini/tree/master/README.md) | 简体中文

一个简约的响应式 Hugo 主题。

![./images/screenshot.png](https://raw.githubusercontent.com/nodejh/hugo-theme-mini/master/images/screenshot.png)

- [在线 Demo](https://nodejh.github.io/hugo-theme-mini)
- [示例网站源码](https://github.com/nodejh/hugo-theme-mini/tree/master/exampleSite)

特性：

- 快
- 简约
- 响应式
- 归档页
- 标签页


## 1. 安装


### 1.1 使用 Hugo 模块安装 (推荐)

> ⚠️ 如果你使用的是 [二进制包](https://gohugo.io/getting-started/installing/#binary-cross-platform) 安装的 Hugo，那么你需要在电脑上安装 Go 语言。 你可以使用下面的命令检查是否安装 Go：
> ```
> $ go version
> ```
> Go 语言从 v1.14 开始支持模块. [下载 Go](https://golang.org/dl/)。

1. 在项目目录初始化 hugo 模块系统，如果之前已经执行过则忽略此步骤：

    ```bash
    $ hugo mod init github.com/<your_user>/<your_project>
    ```

2. 在 `config.yaml` 中添加主题：

    ```yaml
    theme: 
       - github.com/nodejh/hugo-theme-mini
    ```

### 1.2 使用 Git Submodule 安装


1. 在项目目录中执行下面的命令，将 hugo-theme-mini 作为 submodule：

    ```bash
    $ git submodule add https://github.com/nodejh/hugo-theme-mini.git themes/mini
    ```

2. 在 `config.yaml` 中配置主题：

    ```yaml
   theme: mini
    ```

更多信息可参考 Hugo 官方文档 [setup guide](//gohugo.io/overview/installing/)。


## 2. 开始使用

成功安装主题后，在生成网站前还需要进行少部分的配置。


### 2.1 修改配置文件

在 [`exampleSite`](https://github.com/nodejh/hugo-theme-mini/tree/master/exampleSite) 目录中有一个 [`config.yaml`](https://github.com/nodejh/hugo-theme-mini/blob/master/exampleSite/config.yaml) 的配置文件，你可以将其复制到你的项目根目录中，将一些配置项修改为你的配置。这些配置都可以随意修改。


> ⚠️ 你需要删除这行配置： `themesDir: ../../` 。

### 2.2 默认语言

你可以通过 `defaultContentLanguage` 配置设置默认语言：

```yaml
defaultContentLanguage: en
```

默认是 `en`。目前支持以下语言：

- `en`: 英语
- `zh`: 汉语
- `nl`: 荷兰语
- `fr`: 法语
- `es`: 西班牙语

更多关于多语言的信息可以参考：[Multilingual Mode](https://gohugo.io/content-management/multilingual/)。


### 2.2 评论功能

要使用评论功能，你需要添加下面的配置：

- 设置 Disqus： `disqusShortname: your-disqus-shorname`
- 启用评论：

    ```yaml
    params:
      enableComments: true
    ```

### 2.3 Google 分析

要使用 Google 分析功能，你需要添加下面的配置：

- 设置 Google Analytics ID： `googleAnalytics: your-google-analytics-id`
- 启用 Google Analytics：

    ```yaml
    params:
      enableGoogleAnalytics: true
    ```

### 2.4 Logo 和 favicon

你可以替换网站中的 Log 和 favicon，只需要将你的图片放在网站的 `static/images` 中，并分别命名为 `avatar.png` 和 `avicon.ico`。下面是项目目录示例：

```shell
- content
- static
└── images
    ├── avatar.png
    └── favicon.ico
```

### 2.5 运行网站

为了检查网站运行情况，你可以在本地启动 hugo server：

```bash
$ hugo server
```

现在你就可以在浏览器中打开 http://localhost:1313 查看你的网站了。

### 2.6 生产环境

如果要将网站部署到生产环境 (例如支持 Google Analytics)，你需要在 `hugo` 命令前增加环境变量 `HUGO_ENV=production`。例如：

```bash
HUGO_ENV=production hugo
```

注意：上面的命令对 Windows 无效。如你使用 Windows，则需要使用下面的命令：

```bash
set HUGO_ENV=production
hugo
```

## 3. 可选配置

### 3.1 Table of Content

如果要启用目录，你可以将 `showToc` 设置为 `true`：

```yaml
showToc: true
```


### 3.2 在某页面禁用评论

要在某页面禁用评论，你可以在页面的 Front Matter 中将 `enableComments` 设置为 `false`。

例如：

```yaml
---
title: Some title
enableComments: false
---
```

### 3.3 自定义 CSS 和 JS

你可以将自定义 CSS 和 JS 放在 `static` 中，也可以使用远程的 CSS 或 JS 文件。

例如：

```yaml
customCSS:
  - css/custom.css # local css in `static/css/custom.css`
  - https://example.com/custom.css # remote css
customJS:
  - js/custom.js # local js in `static/js/custom.js`
  - https://example.com/custom.js # remote js
```


### 3.4 数学排版

该主题使用了 [KaTeX](https://katex.org/) 来支持数学符号拍版。

- 全局支持数学排版：在项目的配置文件中将 `math` 设置为 `true`
- 在某页面支持数学拍版：在某页面 Front Matter 中将 `math` 设置为 `true`

### 3.5 在首页隐藏文章摘要 

如果要在首页隐藏文章摘要，你可以将 `hiddenPostSummaryInHomePage` 设置为 `true`，默认是 `false`。

例如：

```yaml
hiddenPostSummaryInHomePage: true
```

## License

[MIT](https://github.com/nodejh/hugo-theme-mini/blob/master/LICENSE.md)