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

_（对应 raw/ 中的文件）_

---

## 🧠 核心概念

_（知识库中的核心概念，每个概念一个页面）_

---

## 👤 实体

_（人物、公司、工具、项目等）_

---

## 📊 综合分析

_（跨主题分析、研究报告、问答沉淀）_

---

## 📈 统计

| 项目 | 数量 |
|------|------|
| 来源页 | 0 |
| 概念页 | 0 |
| 实体页 | 0 |
| 综合分析 | 0 |
| 待处理 raw 文件 | 0 |
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
