---
title: content/page/search/index.md 参数说明
draft: true
---

- 作用：站内搜索页。
- 前置参数：
```yaml
---
title: "搜索"
slug: "search"
layout: "search"
outputs: [html, json]
menu:
  main:
    weight: 3
    params:
      icon: search
---
```
- 字段：
  - `layout`：固定 `search`
  - `outputs`：需包含 `json` 以生成索引
  - `menu.main.*`：加入主菜单 