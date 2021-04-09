---
title: hexo-generator-feed 的 atom 参数设置
# permalink: /about/
date: 2020-11-21
updated: 2020-11-21
tags:
  - 博客
# password: 
# message: 
# categories:
# keywords:
description: 配置hexo的RSS所需要参考的一些配置信息。
# top_img:
# comments: false
cover: https://cdn.jsdelivr.net/gh/hankzhangcn/CDN@master/img/hexo_封面.3aaae3y1k7u0.jpg
# toc:
# toc_number:
copyright: 
copyright_author: kwor'blog
copyright_author_href: https://www.kwor.cn
# copyright_url:
# copyright_info:
katex: false
# aplayer:
# highlight_shrink:
# aside:
---

由于atom本身默认是简短显示。所以如果作为转移数据时需要进行简单设置才能显示全文。

```yml
plugin:
- hexo-generator-feed
feed:
  type: atom  #可以设置为rss2.xml
  path: atom.xml #可以设置为rss2.xml
  limit: 0 #显示多少篇博文，0为无限制
  hub:
  content: true #是否显示全文，true为全部显示，反之为空，需要设置content_limit选项。如果为true不需要设置content_limit选项
  content_limit_delim: ' '
```

最后附有参数的所有说明

```yml
#path - Feed path. When both types are specified, path must follow the order of type value. (Default: atom.xml/rss2.xml)
#limit - Maximum number of posts in the feed (Use 0 or false to show all posts)
hub - URL of the PubSubHubbub hubs (Leave it empty if you don't use it)
#content - (optional) set to 'true' to include the contents of the entire post in the feed.
#content_limit - (optional) Default length of post content used in summary. Only used, if content setting is false and no custom post description present.
#content_limit_delim - (optional) If content_limit is used to shorten post contents, only cut at the last occurrence of this delimiter before reaching the character limit. Not used by default.
#order_by - Feed order-by. (Default: -date)
#icon - (optional) Custom feed icon. Defaults to a gravatar of email specified in the main config.
#autodiscovery - Add feed autodiscovery. (Default: true)
Many themes already offer this feature, so you may also need to adjust the theme's config if you wish to disable it.
#template - Custom template path(s). This file will be used to generate feed xml file, see the default templates: atom.xml and rss2.xml.
```