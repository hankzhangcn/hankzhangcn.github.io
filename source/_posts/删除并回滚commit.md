---
title: 删除并回滚commit
# permalink: /about/
date: 2020-11-19
updated: 2020-11-19
tags:
  - 学习
  - git
# password: 
# message: 
# categories:
# keywords:
description: 又出bug了？回滚commit吧。
# top_img:
# comments: false
cover: https://cdn.jsdelivr.net/gh/hankzhangcn/CDN@master/img/删除并回滚commit_封面.5myjccl6c080.jpg
# toc:
# toc_number:
# copyright:
# copyright_author:
# copyright_author_href:
# copyright_url:
# copyright_info:
katex: false
# aplayer:
# highlight_shrink:
# aside:
# published: false
---


```git
git reset --hard acb28f2111234231122257dca62a1cd29d0f【想要恢复到的版本commit id】
git push origin HEAD --force
```

来自[github如何删除commit记录](https://blog.csdn.net/xiaxinkai/article/details/90743358)