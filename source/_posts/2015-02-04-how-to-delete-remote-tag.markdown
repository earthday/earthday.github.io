---
layout: post
title: "How to delete remote tag"
date: 2015-02-04 01:01
comments: true
categories: git
---

一不小心在错误的commit上打了tag，并且已经提交到了remote的repo上，那么怎么办哪？

```
git tag -d tag_name
git push origin :refs/tags/tag_name
```

把上述命令中的tag_name变换成那个打错的tag名称即可。

## References
1. [http://nathanhoad.net/how-to-delete-a-remote-git-tag](http://nathanhoad.net/how-to-delete-a-remote-git-tag)
