---
title: content/page/links/index.md 参数说明
draft: true
---

- 作用：友链/资源清单页面，按 `links` 数组渲染链接卡片。
- 前置参数：
```yaml
---
title: Links
links:
  - title: GitHub
    description: 全球最大开源平台
    website: https://github.com
    image: /my-blog/path/logo.png
menu:
  main:
    weight: 4
    params:
      icon: link
comments: false
---
```
- 字段：
  - `links[].title/description/website/image`：卡片内容（`image` 支持本地或外链；子路径站点建议以 `/my-blog/` 开头）
  - `menu.main.*`：是否加入主菜单
  - `comments`：关闭/开启评论 