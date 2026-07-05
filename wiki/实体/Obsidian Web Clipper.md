---
title: Obsidian Web Clipper
type: 实体
created: 2026-07-05
updated: 2026-07-05
tags: [工具, 浏览器扩展, obsidian]
related: [[Obsidian]], [[个人知识管理]]
source: [[来源-Web Clipper 配置指南]]
---

# Obsidian Web Clipper

> **Obsidian Web Clipper** 是 Obsidian 官方出品的浏览器扩展，用于将网页内容一键剪藏到 Obsidian vault 中。

## 概述

Obsidian Web Clipper 支持 Chrome/Edge/Firefox 浏览器，可将网页文章保存为 Markdown 文件并自动存入指定目录，是 PKM 工作流中"收集"环节的重要工具。

## 配置要点

1. 安装浏览器扩展，连接到本地 Obsidian vault
2. 设置默认保存路径为 `raw/文章/`
3. 配置 YAML frontmatter 模板（含 title、type、source_url、created、tags）
4. 剪藏后按 `Ctrl+Shift+D` 下载所有图片到本地

## 工作流集成

在 PKM 工作流中，Web Clipper 负责**输入**环节：

```
浏览网页 → 点击 Web Clipper → 自动保存到 raw/文章/ → 说"整理一下" → AI 消化 → wiki 更新
```

## 相关实体

- [[Obsidian]] — 所属工具生态
- [[来源-Web Clipper 配置指南]] — 详细配置说明

## 参考来源

- [[raw/Web Clipper 配置指南.md]] — 原始配置文档
