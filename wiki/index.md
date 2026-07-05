---
title: 知识库索引
type: index
created: 2026-07-05
updated: 2026-07-05
---

# 🌳 知识库索引

> 本页由 AI 自动维护，记录 wiki/ 下所有页面的索引。

---

## 📥 来源（已处理的原始资料）

- [[来源-Web Clipper 配置指南]] — Obsidian Web Clipper 配置指南
- [[来源-代码阅读与学习方法论]] — 代码阅读技巧与学习心态总结

---

## 🧠 核心概念

- [[双向链接]] — 笔记间的连接纽带
- [[本地优先]] — 数据所有权与控制权
- [[个人知识管理]] — PKM 方法论与实践
- [[图谱视图]] — 知识网络可视化
- [[原子笔记]] — 最小知识单元原则
- [[MOC]] — 内容地图导航法
- [[代码阅读方法论]] — 如何高效阅读源码
- [[提问的艺术]] — 写出让人愿意帮你的好问题
- [[费曼学习法]] — 能讲清楚才算真理解
- [[按需阅读]] — 不需要全部看懂
- [[问题雷达]] — 持续积累踩坑经验

---

## 👤 实体

- [[Obsidian]] — 本地优先 Markdown 笔记应用
- [[Obsidian Web Clipper]] — 浏览器剪藏扩展

---

## 📊 综合分析

- [[使用指南]] — 自生长知识库完整操作手册

---

## 📈 统计

| 项目 | 数量 |
|------|------|
| 来源页 | 2 |
| 概念页 | 11 |
| 实体页 | 2 |
| 综合分析 | 1 |
| 已处理的 raw 文件 | 代码阅读与学习方法论 |
| 最后更新 | 2026-07-05 |

---

## 🔍 Dataview 动态查询

> 以下表格由 Dataview 插件自动生成，基于页面 frontmatter 实时更新。

### 所有概念页
```dataview
TABLE tags, created, updated AS "最近更新"
FROM "wiki/概念"
SORT updated DESC
```

### 所有实体页
```dataview
TABLE tags, created
FROM "wiki/实体"
SORT created DESC
```

### 最近创建的页面
```dataview
TABLE type, created AS "创建日期"
FROM "wiki"
SORT created DESC
LIMIT 10
```

### 按标签统计
```dataview
TABLE length(rows) AS "页面数"
FROM "wiki"
FLATTEN tags AS tag
GROUP BY tag
SORT length(rows) DESC
```
