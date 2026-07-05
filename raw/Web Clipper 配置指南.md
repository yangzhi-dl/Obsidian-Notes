---
title: Web Clipper 配置指南
type: guide
created: 2026-07-05
---

# Obsidian Web Clipper 配置指南

> 一键将网页文章保存到 `raw/文章/`，让 AI 帮你消化。

---

## 📥 安装

1. 打开浏览器（Chrome/Edge/Firefox）
2. 安装 [Obsidian Web Clipper](https://obsidian.md/clipper) 扩展
3. 点击浏览器工具栏的扩展图标

## ⚙️ 配置

### 1. 连接 Obsidian
- 首次点击扩展图标 → 选择 **连接 Obsidian**
- 确保你的 Obsidian  vault 已打开

### 2. 设置保存路径
- 在扩展设置中，将默认保存目录设为：
  ```
  raw/文章/
  ```

### 3. 推荐模板

在 Web Clipper 设置中添加以下模板：

```markdown
---
title: {{title}}
type: source
source_url: {{url}}
created: {{date}}
tags: []
---

# {{title}}

> 来源：{{url}}

## 摘要


## 核心观点


## 关键词


## 相关链接

```

---

## 🎯 使用流程

1. 看到好文章 → 点击 Web Clipper 图标
2. 自动保存到 `raw/文章/` 目录
3. 回到 Obsidian → 在 Claudian 中说 **"整理一下"**
4. AI 自动阅读文章 → 提取概念 → 创建 wiki 页面

---

## 💡 小贴士

- 剪藏后按 `Ctrl+Shift+D` 下载所有图片到本地
- 图片自动保存到 `raw/assets/` 目录
- AI 优先读取文章文本，必要时可查看图片
