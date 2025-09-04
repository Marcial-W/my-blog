---
title: content/post/image-gallery/index.md 参数说明
draft: true
---

- 作用：创建交互式图片画廊（PhotoSwipe）。
- 要点：图片需与 Markdown 同目录（页面 Bundle），不支持外链图。
- 前置参数最小示例：
```yaml
---
title: Image gallery
image: 2.jpg
---
```
- 正文语法：
```markdown
![Image 1](1.jpg) ![Image 2](2.jpg)
```
- 字段：
  - `image`：封面图（同目录） 