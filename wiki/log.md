---
title: 操作日志
type: log
created: 2026-07-05
---

# 📋 操作日志

> 记录所有 wiki 变更操作，append-only。

---

## 2026-07-05

### 初始化
- 创建知识库基础结构：
  - `AGENTS.md` — OpenCode 原生规则文件
  - `CLAUDE.md` — 兼容层（指向 AGENTS.md）
  - `.raw/manifest.json` — 素材追踪清单
  - `raw/` — 原始资料目录（文章/随记/论文）
  - `wiki/` — 知识层目录（索引/热缓存/日志/来源/概念/实体/综合）
  - `skills/wiki/SKILL.md` — 技能定义
- 已有笔记等待首次整理：关于Obsidian.md、双向链接、20260705笔记

### 配置完善
- Git 版本管理初始化 + .gitignore
- 安装 Dataview 插件（v0.5.70） + 注册到 community-plugins.json
- 配置图片附件路径为 `raw/assets/`
- 创建 `raw/Web Clipper 配置指南.md`
- 更新 wiki/index.md 加入 Dataview 动态查询
- 更新 AGENTS.md 强调 YAML frontmatter 规范（Dataview 兼容）
