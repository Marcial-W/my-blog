---
title: content/_index.md 参数说明
draft: true
---

- 作用：站点主页入口在菜单中的配置。
- 前置参数：
```yaml
menu:
  main:
    name: 主页
    weight: 1
    params:
      icon: home
```
- 字段：
  - `menu.main.name`：菜单显示名
  - `menu.main.weight`：排序（小在前）
  - `menu.main.params.icon`：图标名（主题内置）
- 最小示例：
```yaml
---
menu:
  main:
    name: 主页
    weight: 1
    params:
      icon: home
---
``` 