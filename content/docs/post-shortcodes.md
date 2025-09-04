---
title: content/post/shortcodes/index.md 参数说明
draft: true
---

- 作用：展示主题内置短代码（视频、引述、Gist 等）。
- 前置参数：
```yaml
---
title: Shortcodes
description: Useful shortcodes that can be used in Markdown
date: 2023-08-25 00:00:00+0000
image: cover.jpg
---
```
- 常用短代码示例：
```markdown
{{< bilibili "BV1d4411N7zD" >}}
{{< youtube "0qwALOOvUik" >}}
{{< video "https://www.w3schools.com/tags/movie.mp4" >}}
{{< quote author="A" source="B" url="https://example.com" >}}内容{{< /quote >}}
```
- 注意：官方 `gist` 短代码已弃用（>= v0.143.0），建议改为自定义短代码或脚本嵌入。 