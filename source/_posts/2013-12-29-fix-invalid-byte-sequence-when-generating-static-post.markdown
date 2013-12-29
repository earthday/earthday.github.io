---
layout: post
title: "Fix 'invalid byte sequence' when generating static post"
date: 2013-12-29 22:05
comments: true
categories: 
---

## Error happens
好久没有玩这个东东了，最近在学习Ruby/RoR，所以突然对这个来了兴趣，但是却在运行```rake generate```时遇到了下列错误
```
λ rake generate
## Generating Site with Jekyll
identical source/stylesheets/screen.css
Configuration from D:/github/earthday.github.io/_config.yml
Building site: source -> public
YAML Exception reading 2013-04-20-welcome.markdown: invalid byte sequence in GBK D:/github/earthday.github.io/plugins/backtick_code_block.rb:13:in `gsub': invalid
 byte sequence in GBK (ArgumentError)
```

## 解决办法
外事不决问Google，于是就找到了这个问题的解决办法。参见[http://kumu-linux.github.io/blog/2013/04/06/octopress-plus-github/](http://kumu-linux.github.io/blog/2013/04/06/octopress-plus-github/).
就是在命令行中设置：
```
set LANG=zh_CN.UTF-8
set LC_ALL=zh_CN.UTF-8
```

OKay，既然好久没来了，就更新一篇，留个脚印。。哈哈。。
