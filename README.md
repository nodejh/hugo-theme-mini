# Cactus Plus


[English Documention](https://github.com/nodejh/hugo-theme-cactus-plus/blob/master/README.md) | [中文文档](https://github.com/nodejh/hugo-theme-cactus-plus/blob/master/README_zh-cn.md)


Cactus Plus is a minimalistic theme for bloggers based on the theme named [Cactus](https://github.com/digitalcraftsman/hugo-cactus-theme).

**Noteworthy updates of this Hugo theme are :**

+ **a tags page**
+ **an archive page**
+ **both [Disqus](https://disqus.com/) and [Duoshuo](http://duoshuo.com/) comment-system**
+ **both Google Analytics and Baidu Tongji for site analytics.**

Here's the link to online demo: [http://nodejh.com](http://nodejh.com).

## Screenshot

**home page**

![Screenshot](https://github.com/nodejh/hugo-theme-cactus-plus/blob/master/images/screenshot.png)

**tags page**

![Screenshot](https://github.com/nodejh/hugo-theme-cactus-plus/blob/master/images/tags.png)

**archive page**

![Screenshot](https://github.com/nodejh/hugo-theme-cactus-plus/blob/master/images/archive.png)

## Installation

```
$ cd themes
$ git clone https://github.com/nodejh/hugo-theme-cactus-plus.git
```

For more information read the official [setup guide](//gohugo.io/overview/installing/) of Hugo.


## Example Site

There is an example site with config file and markdown files in [`exampleSite`](https://github.com/nodejh/hugo-theme-cactus-plus/tree/master/exampleSite) directory.

### The config file

Take a look inside the [`exampleSite`](https://github.com/nodejh/hugo-theme-cactus-plus/tree/master/exampleSite) folder of this theme. You'll find a file called [`config.toml`](https://github.com/nodejh/hugo-theme-cactus-plus/blob/master/exampleSite/config.toml).

To use it, copy the [`config.toml`](https://github.com/nodejh/hugo-theme-cactus-plus/blob/master/exampleSite/config.toml) in the root folder of your Hugo site. Feel free to change strings as you like to customize your website.

## About page

Use the about page to introduce yourself to your visitors. You can customize the content as you like in the `/content/about/index.md`.

## Avatar

Furthermore, you should replace the [avatar placeholder](https://github.com/nodejh/hugo-theme-cactus-plus/blob/master/static/images/) with a great image of yourself.

## Hide pages

Pages can be hidden and don't appear in the post list on the homepage if you add the variable `hidden = true` to the frontmatter. This allows you to link from elsewhere, i.e. just the menu.

## Disqus

This theme features a comment system powered by Disqus. Just add your Disqus-shortname to the [`config.toml`](https://github.com/nodejh/hugo-theme-cactus-plus/blob/master/exampleSite/config.toml) and set `enableDisqus = true`, then let readers respond to your blog posts.


## Duoshuo

This theme features a comment system powered by Duoshuo too. Duoshuo is mainly provide for Chinese users. Just add your Duoshuo-shortname to the [`config.toml`](https://github.com/nodejh/hugo-theme-cactus-plus/blob/master/exampleSite/config.toml) and set `enableDuoshuo = true`.


## Disable Comment

Just set both `enableDisqus = false` and `enableDuoshuo = false` if you want to disable comment.



## Google Analytics

This theme use Google Analytics defalut. If you want to disable Google Analytics, just set `enableGoogleAnalytics = false` in [`config.toml`](https://github.com/nodejh/hugo-theme-cactus-plus/blob/master/exampleSite/config.toml).

## Baidu Tongji

This theme alse features Baidu Tongji for Chinese users. To use Baidu Tongji you should set `enableBaiduAnalytics = true` and set `baiduAnalytics` to your  `Baidu Tongji Code` which looks like `39843ea392201290bd6f76173d2e0000` in  [`config.toml`](https://github.com/nodejh/hugo-theme-cactus-plus/blob/master/exampleSite/config.toml).


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


## Acknowledgements

Thanks to

- [hugo-cactus-theme](https://github.com/digitalcraftsman/hugo-cactus-theme)
