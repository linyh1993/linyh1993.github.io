# linyh1993.github.io

Linyh 的个人博客，使用 Astro 构建，支持中文和英文：

- `/`：中文，默认语言
- `/en/`：English

## 本地开发

```bash
pnpm install
pnpm dev
```

Windows 本地构建：

```bash
pnpm build:local
pnpm preview
```

`pnpm build` 保留给 GitHub Actions 和 Linux 构建环境使用。

## 写文章

将 Markdown 或 MDX 文件放入 `src/content/posts/`，然后填写 frontmatter：

```md
---
title: "文章标题"
pubDatetime: 2026-10-28T12:00:00+08:00
description: "文章摘要"
tags:
  - tech
---
```

## 部署

推送到 `main` 分支后，`.github/workflows/deploy.yml` 会自动执行构建并发布到 GitHub Pages。

## 技术栈

- Astro
- TypeScript
- Tailwind CSS
- Pagefind
- GitHub Pages
