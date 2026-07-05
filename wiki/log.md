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

### 首次知识整理 — Obsidian 概念编译

**输入来源：**
- `关于Obsidian.md`（根目录已有笔记）
- `raw/Web Clipper 配置指南.md`

**新建页面：**

| 类型 | 页面 | 说明 |
|------|------|------|
| 来源 | [[来源-Web Clipper 配置指南]] | Web Clipper 配置摘要 |
| 概念 | [[双向链接]] | 笔记间双向连接 |
| 概念 | [[本地优先]] | 本地优先数据哲学 |
| 概念 | [[个人知识管理]] | PKM 方法论 |
| 概念 | [[图谱视图]] | 知识网络可视化 |
| 概念 | [[原子笔记]] | 最小知识单元 |
| 概念 | [[MOC]] | 内容地图导航 |
| 实体 | [[Obsidian]] | Obsidian 应用 |
| 实体 | [[Obsidian Web Clipper]] | 浏览器剪藏扩展 |

**变更概要：**
- 从 `关于Obsidian.md` 中提取出 6 个核心概念 + 1 个实体
- 从 `raw/Web Clipper 配置指南.md` 中提取出 1 个来源页 + 1 个实体
- 所有新页面均包含完整的 YAML frontmatter（兼容 Dataview）
- 页面之间已建立双向链接网络

### 第二次整理 — 代码阅读与学习方法论

**输入来源：**
- `raw/随记/2026-07-05-代码阅读与学习方法论.md`

**新建页面：**

| 类型 | 页面 | 说明 |
|------|------|------|
| 来源 | [[来源-代码阅读与学习方法论]] | 文章摘要 |
| 概念 | [[代码阅读方法论]] | 代码阅读顺序与技巧 |
| 概念 | [[提问的艺术]] | 四段式提问法 |
| 概念 | [[费曼学习法]] | 通过教来学 |
| 概念 | [[按需阅读]] | 不需要全部看懂 |
| 概念 | [[问题雷达]] | 踩坑经验积累系统 |

**变更概要：**
- 从一篇随记中提取出 5 个核心概念
- 所有页面包含完整 YAML frontmatter + 双向链接
- 已更新 index.md、hot.md、manifest.json
