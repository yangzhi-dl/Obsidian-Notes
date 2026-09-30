---
title: 热缓存
type: cache
created: 2026-07-05
updated: 2026-07-30
---

# 🔥 热缓存

> 本文件在每次 AI 会话启动时读取，会话结束时更新。
> 记录当前知识库的状态快照，帮助 AI 快速恢复上下文。

---

## 会话状态

- **最后活跃日期**: 2026-08-03
- **知识库总页面数**: 已重构（旧目录已清理，共 15 个重复文件已删除）
- **待处理 raw 文件数**: 0
- **最近一次架构调整**: 2026-07-30 — 领域优先结构重构
- **最近一次清理**: 2026-08-03 — 删除旧目录重复文件，清理空目录

## 当前项目

- [[projects/Obsidian自生长知识库/index|Obsidian 自生长知识库]]
- [[projects/投资入门/index|投资入门]]
- [[projects/英语学习/index|英语学习]]

## 最近重点领域

- [[wiki/技术/index|技术]]
- [[wiki/投资/index|投资]]
- [[wiki/学习/index|学习]]

## 待处理

- Inbox 待处理内容
- Seed 状态笔记
- 需要更新的项目
- 缺少来源的笔记

## 最近更新

- **2026-07-30**: 知识库架构重构。引入 inbox/、projects/、outputs/、archive/、templates/。wiki 按 7 个领域组织。新 AGENTS.md、CLAUDE.md 发布。
- **2026-08-03**: 旧目录清理。删除 `wiki/概念/`、`wiki/实体/`、`wiki/来源/` 下的 15 个重复文件，清理空目录，知识库完全切换为领域优先架构。

---

## 可选 Dataview 查询

> 以下查询需要安装 Dataview 插件，不安装不影响知识库其他功能。

```dataview
TABLE file.frontmatter.status AS "状态", file.updated AS "更新"
FROM "wiki"
WHERE file.frontmatter.status = "seed"
SORT file.updated ASC
```
