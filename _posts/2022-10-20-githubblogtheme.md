---
layout: post
title:  "github博客主题"
categories: 通用技术
tags:  blog
author: huayaoit 
---

* content
{:toc}

# 关于本博客主题

* 博客采用[JekyllThemes](https://jekyllrb.com/)生成，模板使用[浩阳 ](https://github.com/Gaohaoyang)。相关文章：如何使用github搭建个人博客









## 主题结构和文件

* [Page Details](#page-details)
    * [Home](#home)
    * [Archives](#archives)
    * [Categories](#categories)
    * [Tags](#tags)
    * [Collections](#collections)
    * [About](#about)
    * [Comments](#comments)
    * [Post Contents](#post-contents)
    * [Code Highlight](#code-highlight)
    * [Light Shadow](#light-shadow)
    * [Mobile Adaptation](#mobile-adaptation)
    * [Footer](#footer)
    * [Statistical Analysis](#statistical-analysis)
* [Usage](#usage)
    * [1. Install ruby and jekyll environment](#1-install-ruby-and-jekyll-environment)
    * [2. Copy theme code](#2-copy-theme-code)
    * [3. Change parameter](#3-change-parameter)
        * [Basic info](#basic-info)
        * [Link info](#link-info)
        * [Comments info](#comments-info)
        * [Statistical analysis info](#statistical-analysis-info)
    * [4. Write post](#4-write-post)
    * [5. Local launch](#5-local-launch)
    * [6. Push to GitHub](#6-push-to-github)
* [Donate](#donate)
* [Update Log](#update-log)
* [License](#license)

## Page Details

### Home

博客首页.

### Archives

博客存档.

### Categories

博客分类.

### Tags

博客标签.

### Collections

资源收集

### About

关于我们页面.

### Comments

主题支持 [disqus](https://disqus.com/) and [duoshuo comments](http://duoshuo.com/)两种评论模式. 您只需要根据自己的需要对配置文件进行相应配置 `_config.yml`. 如下.

```yml
# comments
# two ways to comment, only choose one, and use your own short name
duoshuo_shortname: #xxx
disqus_shortname: xxx
```

### Post Contents

页面内容，如果页面内容过程，可以通过浏览器滚动条往下滚动浏览，当在内容页面最低端时，可通过点击回到顶端来到达页面的顶端.

### Code Highlight

代码突出显示

### Light Shadow

![light](http://ww3.sinaimg.cn/large/7011d6cfjw1f3be6y4vp3j209i02rweg.jpg)

当前选定导航菜单会显示为白色（本博客笔者修改了部分主题颜色，并不是白色）.

### Mobile Adaptation

响应式布局

![mobile](http://ww4.sinaimg.cn/large/7011d6cfjw1f3bebnzxkpj20ah0fzgp4.jpg)

### Footer

页脚请保留主题开发者信息

![footer](http://ww3.sinaimg.cn/large/7011d6cfjw1f3bepd8002j20hl02ct95.jpg)

### Statistical Analysis

站点访问统计支持百度和谷歌统计，如需开启只需要在_config.yml配置一下即可.

```yml
# statistic analysis 统计代码
# 百度统计 id，将统计代码替换为自己的百度统计id，即
# hm.src = "//hm.baidu.com/hm.js?xxxxxxxxxxxx";
# xxxxx字符串
baidu_tongji_id: xxxxxxxxxxxx
google_analytics_id: UA-xxxxxxxx # google 分析追踪id
```

## Usage

接下来将展示本主题如何使用.

### 1. 安装 ruby and jekyll 环境

此步骤和步骤5主要与您讨论如何在本地启动博客。如果您不想在本地启动，可以忽略这两个步骤。但我仍然强烈建议这样做。在推送到github之前，请确保没有错误.

Windows用户请直接安装 [RubyInstaller](http://rubyinstaller.org/) 环境. 按照提示执行操作即可.

安装l jekyll 命令行:

```
gem install jekyll
```

更多信息请访问Jekyll官网获取. [https://jekyllrb.com/](https://jekyllrb.com/)

苹果系统安装时遇到问题请访问： [https://jekyllrb.com/docs/troubleshooting/#jekyll-amp-mac-os-x-1011]( https://jekyllrb.com/docs/troubleshooting/#jekyll-amp-mac-os-x-1011).

如果对Jekyll感兴趣，也可以访问 [https://github.com/jekyll/jekyll](https://github.com/jekyll/jekyll).

### 2. Copy theme code

可以通过github克隆该主题.

### 3. Change parameter

主题全局参数在 `_config.yml` 中，主题浏览器图标是 `favicon.ico`.

#### 基本信息

在站点标题中显示.

```yml
# Site settings
title: HyG
brief-intro: Front-end Dev Engineer
baseurl: "" # the subpath of your site, e.g. /blog
url: "http://gaohaoyang.github.io" # the base hostname & protocol for your site
```

#### 链接信息

在站点页脚显示.

```yml
# other links
twitter_username: gaohaoyang126
facebook_username: gaohaoyang.water
github_username:  Gaohaoyang
email: gaohaoyang126@126.com
weibo_username: 3115521wh
zhihu_username: gaohaoyang
linkedIn_username: gaohaoyang
dribbble_username:

description_footer: 本站记录我前端之旅的沿途风景！
```

#### 评论信息

注册用户名： `short_name`:

请依据您使用的评论插件类型访问https://disqus.com/ or http://duoshuo.com/. 并按照网站提示进行操作.

```yml
# comments
# two ways to comment, only choose one, and use your own short name
duoshuo_shortname: #hygblog
disqus_shortname: xxxx
```

完成设置后就可以在 disqus 或 duoshuo 管理控制台中看到有关的评论信息.

#### 站点统计

注册并获取自己的统计代码ID：

可通过访问https://www.google.com/analytics/ 或 http://tongji.baidu.com/获取. 按照网站要求操作.

当然如果不需要统计，则可以不填写任何信息.

```yml
# statistic analysis 统计代码
# 百度统计 id，将统计代码替换为自己的百度统计id，即
# hm.src = "//hm.baidu.com/hm.js?xxxxxxxxxxxx";
# xxxxx字符串
baidu_tongji_id: cf850xxxxxxxxxxxxxxxx
google_analytics_id: UA-7xxxxxx-4 # google 分析追踪id
```

完成以上设置后，就可以在百度或者谷歌用户中心看到有关的UP,PV信息

### 4. 书写博客内容（发帖子）

您可以在github 上直接撰写帖子，但我非常不建议你这样做，特别是国内用户，链接github经常性抽风，推荐下面的本地调试写作后推送至github。在帖子的顶部，您必须声明layout，title，date，categories，tags，author（可选）、mathjax(可选，点击[这里](https://www.mathjax.org/) 获取更多关于 `Mathjax`的信息.

```
---
layout: post
title:  "对这个 jekyll 博客主题的改版和重构"
date:   2016-03-12 11:40:18 +0800
categories: jekyll
tags: jekyll 端口 markdown Foxit RubyGems HTML CSS
author: Haoyang Gao
mathjax: true
---
```

接下来的代码就是内容部分.
```
* content
{:toc}
```

您可以使用 4 个换行作为文章摘录分隔符。分隔符之前的单词作为摘录显示在首页中。当您进入帖子页面时，您可以阅读完整的文章。.

摘录符号配置在 `_config.yml`中, 如下:

```yml
# excerpt
excerpt_separator: "\n\n\n\n"
```

您可以使用markdown规则和typora工具来写文章，就像直接在github中写自述一样.

您可以用 连续的3个 \`\`\` 来为代码块注释.

### 5. 本地调试启动

使用如下命令启动:

```
jekyll s
```

当终端显示如下信息，表示本地调试成功:

```
Configuration file: E:/GitWorkSpace/blog/_config.yml
            Source: E:/GitWorkSpace/blog
       Destination: E:/GitWorkSpace/blog/_site
 Incremental build: disabled. Enable with --incremental
      Generating...
                    done in 6.33 seconds.
  Please add the following to your Gemfile to avoid polling for changes:
    gem 'wdm', '>= 0.1.0' if Gem.win_platform?
 Auto-regeneration: enabled for 'E:/GitWorkSpace/blog'
Configuration file: E:/GitWorkSpace/blog/_config.yml
    Server address: http://127.0.0.1:4000/
  Server running... press ctrl-c to stop.
```

然后通过访问localhost:4000 来查看您的博客。

### 6. 推送到github

如果没有问题，就可以将本地主题代码推送至github，第一次部署成功后，今后再写博客文章，只需要用markdown工具按第四步写文章的要求书写博客即可，文件命名要求格式为：YYYY-MM-DD-帖子英文标题.md，文件名中的英文标题不影响帖子顶部中文标题的使用。

## License

[MIT License](https://github.com/Gaohaoyang/gaohaoyang.github.io/blob/master/LICENSE.md)
