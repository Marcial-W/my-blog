---
title: content/page/archives/index.md 参数说明
draft: true
---

- 作用：归档页，使用主题提供的 `archives` 布局。
- 前置参数：
```yaml
---
title: "归档"
date: 2025-09-01
layout: "archives"
slug: "archives"
menu:
  main:
    weight: 2
    params:
      icon: archives
---
```
- 字段：
  - `title`：页面标题
  - `date`：页面日期（可用于排序）
  - `layout`：固定为 `archives`
  - `slug`：URL 片段
  - `menu.main.*`：加入主菜单 