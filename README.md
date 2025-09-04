### Marcial-blog · 用键帽敲下的生活火花

> 写代码、写字、写下和世界击掌的瞬间。

- **框架**: Hugo（Theme: `CaiJimmy/hugo-theme-stack`）
- **定位**: 记录编程学习与日常感悟的个人博客
- **在线**: 参考下方部署章节（支持 GitHub Pages）

---

## 亮点速览
- **极速**: 纯静态构建，打开就像 Ctrl+P
- **专注**: 极简侧边栏 + 目录 + 暗色切换
- **可写**: Markdown 写作，前置参数即所见即所得

---

## 快速开始

```bash
# 1) 本地预览
hugo server -D
# 打开: http://localhost:1313/my-blog/

# 2) 生成静态文件
hugo
# 输出在 public/
```

---

## 写作指南（最常用）

- **新文章**（示例）
```bash
hugo new post/hello-world.md
```
- **Front Matter 最小示例**
```toml
---
title: "Hello World"
date: 2025-09-04T00:00:00+08:00
draft: false
---
```
- **资源引用**
  - 图片放 `static/` 后，用绝对路径：`/my-blog/your-image.png`（见“子路径与头像”）
  - 或使用短代码：`{{< figure src="/my-blog/your-image.png" alt="描述" >}}`

---


---

## 目录结构一眼懂
- `content/`：文章与页面
- `static/`：静态资源（图片、图标、下载文件）
- `assets/`：若使用 Hugo 资源管线（SCSS、图像处理）
- `config/_default/`：站点配置（含 `params.toml`、`config.toml`）
- `public/`：构建产物（自动生成）

---

## 部署到 GitHub Pages（模块化懒人版）

1. 确保 `config/_default/config.toml` 中的 `baseurl` 指向你的仓库 Pages 地址：
   - `https://<username>.github.io/<repo>/`
2. 构建：`hugo`
3. 将 `public/` 的内容推送到 Pages 分支（如 `gh-pages`），或使用 GitHub Actions 自动化。

---

## 主题与版本
- Theme: `github.com/CaiJimmy/hugo-theme-stack/v3`
- 当前依赖见 `go.mod`

> 温馨提示：Hugo 自 v0.143.0 起，内置 `gist` 短代码已弃用。若旧文使用：
> - 参考官方说明迁移（用自定义短代码或直接嵌入脚本）。

---

## 常见问题（FAQ）
- **本地图片 404？**
  - 先确认放在 `static/`；
  - 运行在子路径时，用 `src="/my-blog/xxx.png"`；
  - 部署在根路径则用 `src="/xxx.png"`。
- **头像不显示？**
  - 见“子路径与头像”，确认 `local=false` 且 `src` 含子路径前缀。
- **中文排版**
  - 已启用 `hasCJKLanguage = true`，统计与摘要更准确。

---

## 许可
- 代码：见 `LICENSE`
- 文章与图片：默认保留作者所有权，转载请注明出处。

---

## 致谢
- Hugo 与 Stack 主题作者
- 每一位打开本博客的你

> 写字如写程序：一次提交，持续集成。愿你在这里发现灵感的断点。 