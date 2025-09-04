---
title: content/post/math-typesetting/index.md 参数说明
draft: true
---

- 作用：在文章中启用 KaTeX 数学公式。
- 前置参数：
```yaml
---
title: Math Typesetting
description: Math typesetting using KaTeX
date: 2023-08-24 00:00:00+0000
math: true
---
```
- 字段：
  - `math: true`：为当前文章启用数学渲染
- 站点级开启：在 `params.article` 中设置 `math = true`
- 语法：
  - 行内：`\( a^2+b^2=c^2 \)`
  - 区块：`$$ E=mc^2 $$` 