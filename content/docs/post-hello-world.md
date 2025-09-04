---
title: content/post/hello-world/index.md 参数说明
draft: true
---

- 作用：示例文章，展示常见 Front Matter 字段。
- 前置参数：
```yaml
---
title: Hello World
description: Welcome to Hugo Theme Stack
slug: hello-world
date: 2022-03-06 00:00:00+0000
image: cover.jpg
categories: [Example Category]
tags: [Example Tag]
weight: 1
---
```
- 字段：
  - `title/description/slug/date`：基本信息
  - `image`：封面（同目录下资源）
  - `categories/tags`：分类与标签
  - `weight`：影响排序（值越小越靠前）
- 最小示例：
```yaml
---
title: 一篇新文章
date: 2025-09-04
draft: false
---
``` 