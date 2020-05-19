## hexo-theme-starry

Welcome!

Language:

1. English
2. [中文](https://github.com/meethigher/hexo-theme-starry/blob/master/README.zn.md)

![Starry]( https://d33wubrfki0l68.cloudfront.net/a01d67aa4c9ed9597c21e06eaa91ca499a3f2d3c/fc9cc/themes/screenshots/starry.jpg )

I finished it in my spare time，preview：[I'm Kit Chen](https://meethigher.top/)

Starry is developed by `Less` and `Ejs`.

You can't use it directly, unless you have installed `Less`

```npm
$ npm install hexo-renderer-less --save
```

 Install searchdb

```npm
$ npm install hexo-generator-searchdb --save
```

Install hexo-neat

```npm
$ npm install hexo-neat --save
```

Install hexo-generator-index-pin-top

```npm
$ npm install hexo-generator-index-pin-top --save
```

If you want to top it, you set it like this

```markdown
---
title: xxx
date: xxx
tags: xxx
top: true
---
```

If you want to close one post's comments

```markdown
---
title: xxx
date: xxx
tags: xxx
comments: false
---
```

Generate about

```npm
$ hexo new page about
```

Article format

```
---
title: helloworld
date: 2020-05-19 09:26:20
tags: xxx
top: true
---

此处是文章简介

<!--more-->

此处是文章内容

```


This is my _config.yml

```npm
# Hexo Configuration
## Docs: https://hexo.io/docs/configuration.html
## Source: https://github.com/hexojs/hexo/

# Site 网站配置
title: 言成言成啊
subtitle: Kit Chen's Blog
description: 言成的个人博客网站,寓意为相逢在更高处
keywords: 让我们相逢在更高处,个人博客,个人网站,言成言成啊,学习,生活,个人博客
author: 言成
language: zh-CN
## 时区
timezone:
## hexo3.9.0+以上支持禁用meta_generator标签
meta_generator: false

# URL
## 如果你的网站是放在子文件夹下，root路径就可以设置成/xxx/，否则的话，直接/就行
url: https://meethigher.top/blog/
root: /blog/
## permalink: :year/:month/:day/:title/
permalink: :year/:title/
permalink_defaults:

# Directory 目录
source_dir: source
public_dir: public
tag_dir: tags
archive_dir: archives
category_dir: categories
code_dir: downloads/code
i18n_dir: :lang
skip_render:

# Writing
new_post_name: :title.md # File name of new posts
default_layout: post
titlecase: false # Transform title into titlecase
external_link: true # Open external links in new tab
filename_case: 0
render_drafts: false
post_asset_folder: true
relative_link: false
future: true
highlight:
  enable: true
  line_number: true
  auto_detect: true
  #我将tab设置成了2个空格，可以自定义
  tab_replace:   
  
# Home page setting 主页设置
# path: Root path for your blogs index page. (default = '')
# per_page: Posts displayed per page. (0 = disable pagination) 分页设置为0的时候表示禁用
# order_by: Posts order. (Order by date descending by default) -date表示按时间排序
index_generator:
  path: ''
  per_page: 10
  order_by: -date
tag_generator:
  per_page: 10
  enable_index_page: true
## 禁用archive分页
archive_generator:
  per_page: 0
  yearly: false
  monthly: false
# Category & Tag
default_category: uncategorized
category_map:
tag_map:

# Date / Time format
## Hexo uses Moment.js to parse and display date
## You can customize the date format as defined in
## http://momentjs.com/docs/#/displaying/format/
date_format: YYYY-MM-DD
time_format: HH:mm:ss

# Pagination 分页
## Set per_page to 0 to disable pagination 我设置了主页和标签页，每页显示10个
per_page: 10
pagination_dir: page

# Extensions
## Plugins: https://hexo.io/plugins/
## Themes: https://hexo.io/themes/
theme: starry

# Deployment
## Docs: https://hexo.io/docs/deployment.html
deploy:
  type:

# 站内搜索功能
# 安装插件npm install hexo-generator-searchdb --save
search:
  path: meethigher.json
  field: post
  content: true
  format: raw

# hexo-neat
# 安装插件npm install hexo-neat --save
# 博文压缩
neat_enable: true
# 压缩html
neat_html:
  enable: true
  exclude:
# 压缩css  
neat_css:
  enable: true
  exclude:
    - '**/*.min.css'
# 压缩js
neat_js:
  enable: false
  mangle: true
  output:
  compress:
  exclude:
    - '**/*.min.js'
# 评论配置，下面的内容，换成自己的
# http://blog.poetries.top/2018/11/20/hexo-comment/具体可参照这个大佬的博客
gitalk:
  enable: false
  githubID: meethigher
  repo: meethigher.github.io #在github上建一个public的库，不一定是github.io，也可以是comments，总之随意了
  owner: meethigher
  ClientID: 84xxxxxx
  ClientSecret: a0xxxxxx
  adminUser: meethigher #指定可初始化评论账户
  distractionFreeMode: true #类似于Facebook的分散注意力模式
```


Enjoy using it!

E-mail：meethigher@qq.com/meethigher@gmail.com
