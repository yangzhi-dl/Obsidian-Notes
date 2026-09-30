---
title: 知识库索引
type: index
created: 2026-07-05
updated: 2026-07-30
---

# 🌳 ObNotes 知识地图

> 本页面是整个知识库的入口。记录活跃项目、领域入口、工作入口和待整理内容。

---

## 当前重点

- [[projects/Obsidian自生长知识库/index|Obsidian 自生长知识库]] — 知识库架构初始化
- [[projects/投资入门/index|投资入门]] — 系统学习投资知识

---

## 领域入口

- [[wiki/工具/index|🛠️ 工具]] — Obsidian、Claude Code、效率工具
- [[wiki/技术/index|🏗️ 技术]] — 编程、架构、AI Agent
- [[wiki/学习/index|📖 学习]] — 学习方法、认知科学
- [[wiki/投资/index|💰 投资]] — 指数、ETF、资产配置
- [[wiki/视频创作/index|🎬 视频创作]] — 选题、脚本、剪辑
- [[wiki/写作表达/index|✍️ 写作表达]] — 沟通、文案、汇报
- [[wiki/通用/index|🌐 通用]] — 跨领域通用方法

---

## 工作入口

- [[inbox/index|📥 收集箱]]
- [[raw/index|📂 原始资料]]
- [[projects/index|📋 项目]]
- [[outputs/index|📤 输出]]
- [[archive/index|🗄️ 归档]]
- [[wiki/使用指南|📖 使用指南]]

---

## 知识生命周期

```
inbox(收集)
  ↓
raw(原始资料)
  ↓
seed(AI初步加工)
  ↓
reviewed(人工确认)
  ↓
evergreen(长期稳定)
  ↓
deprecated(标记过时)
```

---

## 待整理

- Inbox 待处理资料
- Seed 状态笔记需要人工确认
- 长期未更新内容
- 缺少来源的笔记
- 存在重复风险的笔记

---

## 最近更新

（人工维护区域 — 记录近期重要变更）

- **2026-07-30** — 知识库架构大重构：引入领域优先结构，新增 inbox/projects/outputs/archive/templates

---

## 迁移后知识分布

现有 wiki 知识已按领域重新组织：

### 工具领域
- [[wiki/工具/概念/双向链接|双向链接]]
- [[wiki/工具/概念/本地优先|本地优先]]
- [[wiki/工具/概念/原子笔记|原子笔记]]
- [[wiki/工具/概念/图谱视图|图谱视图]]
- [[wiki/工具/概念/MOC|MOC]]
- [[wiki/工具/概念/个人知识管理|个人知识管理]]
- [[wiki/工具/实体/Obsidian|Obsidian]]
- [[wiki/工具/实体/Obsidian Web Clipper|Obsidian Web Clipper]]
- [[wiki/工具/来源/来源-Web Clipper 配置指南|来源-Web Clipper 配置指南]]

### 技术领域
- [[wiki/技术/概念/需求全流程|需求全流程]]
- [[wiki/技术/概念/需求澄清|需求澄清]]
- [[wiki/技术/概念/技术评审清单|技术评审清单]]
- [[wiki/技术/概念/灰度发布与回滚|灰度发布与回滚]]
- [[wiki/技术/概念/项目复盘|项目复盘]]
- [[wiki/技术/来源/来源-architecture_full|来源-architecture_full]]

### 学习领域
- [[wiki/学习/概念/代码阅读方法论|代码阅读方法论]]
- [[wiki/学习/概念/提问的艺术|提问的艺术]]
- [[wiki/学习/概念/费曼学习法|费曼学习法]]
- [[wiki/学习/概念/按需阅读|按需阅读]]
- [[wiki/学习/概念/问题雷达|问题雷达]]
- [[wiki/学习/来源/来源-代码阅读与学习方法论|来源-代码阅读与学习方法论]]

---

## 使用原则

- 领域优先 — 每个知识点归属一个主领域
- 来源可追踪 — 每个结论追溯原始资料
- 项目与知识分离 — wiki 存放通用知识，projects 存放具体项目
- 不以笔记数量为目标
- AI 内容需要人工审核

---

## 可选 Dataview 查询

> 以下查询需要安装 Dataview 插件，不安装不影响知识库其他功能。

### 所有概念页
```dataview
TABLE tags, created, updated AS "最近更新"
FROM "wiki"
WHERE type = "concept"
SORT updated DESC
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
