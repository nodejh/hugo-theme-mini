# Hugo Theme Cactus Plus

[English Document](https://github.com/nodejh/hugo-theme-cactus-plus/blob/master/README.md) | [中文文档](https://github.com/nodejh/hugo-theme-cactus-plus/blob/master/README_zh-cn.md)

Cactus Plus is a minimalistic theme for bloggers based on the theme named [Cactus](https://github.com/digitalcraftsman/hugo-cactus-theme).

**Features**

+ **More beautiful style**
+ **Tags page**
+ **Archive page**
+ **[Disqus](https://disqus.com/) comment-system**
+ **Both Google Analytics and Baidu Analytics for site analytics.**
+ **Table of Content**
+ **Twitter Card**

Here's the link to online demo: [http://nodejh.com](http://nodejh.com).


<!-- TOC depthFrom:1 depthTo:6 withLinks:1 updateOnSave:1 orderedList:0 -->

- [Hugo Theme Cactus Plus](#hugo-theme-cactus-plus)
	- [Screenshot](#screenshot)
	- [Installation](#installation)
	- [Example Site](#example-site)
	- [Posts Summary](#posts-summary)
	- [About page](#about-page)
	- [Avatar](#avatar)
	- [Hide pages](#hide-pages)
	- [Disqus](#disqus)
	- [Social link icons](#social-link-icons)
	- [Nearly finished](#nearly-finished)
	- [License](#license)

<!-- /TOC -->

## Screenshot

**home page**

![Screenshot](https://github.com/nodejh/hugo-theme-cactus-plus/blob/master/images/screenshot.png)

**tags page**

![Screenshot](https://github.com/nodejh/hugo-theme-cactus-plus/blob/master/images/tags.png)
**archive page**

![Screenshot](https://github.com/nodejh/hugo-theme-cactus-plus/blob/master/images/archive.png)

## Installation

First clone the theme to your themes directory:

```
$ cd themes
$ git clone https://github.com/nodejh/hugo-theme-cactus-plus.git
```

Take a look inside the [`exampleSite`](https://github.com/nodejh/hugo-theme-cactus-plus/tree/master/exampleSite) folder of this theme. You'll find a file called [`config.toml`](https://github.com/nodejh/hugo-theme-cactus-plus/blob/master/exampleSite/config.toml).

To use it, copy the [`config.toml`](https://github.com/nodejh/hugo-theme-cactus-plus/blob/master/exampleSite/config.toml) in the root folder of your Hugo site. Feel free to change strings as you like to customize your website.

And you may replace your site `archetypes/default.md` with [`hugo-theme-cactus-plus/archetypes/default.md`](https://github.com/nodejh/hugo-theme-cactus-plus/tree/master/archetypes/default.md)

For more information read the official [setup guide](//gohugo.io/overview/installing/) of Hugo.

## Example Site

There is an example site with config file and markdown files in [`exampleSite`](https://github.com/nodejh/hugo-theme-cactus-plus/tree/master/exampleSite) directory.

## Posts Summary

Summary will show follow the post title title in home page.

And if you want to use description property that in post's fromt matter to instated of post's content summary, set `useDescriptionReplaceSummary = true`.

To use the content summary, you may add the `<!--more-->` summary divider where you want to split the article alternatively. For org content, use # more where you want to split the article. Content that comes before the summary divider will be used as that content’s summary.By default, Hugo automatically takes the first 70 words of your content as its summary. See also [https://gohugo.io/content-management/summaries/](https://gohugo.io/content-management/summaries/).

## About page

Use the about page to introduce yourself to your visitors. You can customize the content as you like in the `/content/about/_index.md`.

## Avatar

Furthermore, you should replace the [avatar placeholder](https://github.com/nodejh/hugo-theme-cactus-plus/blob/master/static/images/) with a great image of yourself.

## Hide pages

Pages can be hidden and don't appear in the post list on the homepage if you add the variable `hidden = true` to the frontmatter. This allows you to link from elsewhere, i.e. just the menu.

## Disqus

This theme features a comment system powered by Disqus. Just add your Disqus-shortname to the [`config.toml`](https://github.com/nodejh/hugo-theme-cactus-plus/blob/master/exampleSite/config.toml) and set `enableDisqus = true`, then let readers respond to your blog posts.


## Social link icons

You can add a social link panel in the footer by adding entries to the `social` block in the [`config.toml`](https://github.com/nodejh/hugo-theme-cactus-plus/blob/master/exampleSite/config.toml). You can choose between two icon fonts:

- [Font awesome](https://fortawesome.github.io/Font-Awesome/) or
- [Mono social icons](https://github.com/drinchev/monosocialiconsfont)

Assign either `font-awesome` or `mono-social` to the `iconFont` variable. The Mono social icons offer three styles of icons: -circle, rounded, or default (empty).


## Nearly finished

In order to see your site in action, run Hugo's built-in local server.

```
$ hugo server
```

Now enter [`localhost:1313`](http://localhost:1313) in the address bar of your browser.


## License

This theme is released under the MIT license. For more information read the [license](https://github.com/nodejh/hugo-theme-cactus-plus/blob/master/LICENSE.md).
