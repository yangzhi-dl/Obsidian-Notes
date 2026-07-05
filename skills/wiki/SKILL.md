---
name: wiki
description: LLM Wiki 自生长知识库 — 摄入、查询、维护
trigger: /wiki, 整理一下, 查一下, 检查健康度
---

# Wiki Skill

## 概述

本 Skill 定义 LLM Wiki 自生长知识库的核心操作流程。
适用于所有兼容 Agent Skills 标准的 AI 工具（OpenCode、Codex CLI 等）。

## 能力

### 1. 摄入（Ingest）

将 raw/ 中的新资料编译为 wiki 结构化知识。

**步骤：**
1. 读取 `.raw/manifest.json`，找出 `status: "pending"` 的目录
2. 扫描这些目录下的新 `.md` 文件
3. 对每个新文件：
   a. 在 `wiki/来源/` 创建摘要页（含 YAML frontmatter + [[双链]]）
   b. 提取核心概念 → 创建/更新 `wiki/概念/` 页面
   c. 识别实体 → 创建/更新 `wiki/实体/` 页面
4. 更新 `.raw/manifest.json` 标记为 `ingested`
5. 更新 `wiki/index.md` 增加新页面的链接
6. 追加记录到 `wiki/log.md`

### 2. 查询（Query）

从 wiki 中检索知识并综合回答。

**步骤：**
1. 读取 `wiki/index.md` 了解所有可用页面
2. 在 `wiki/` 下搜索与关键词相关的页面
3. 综合已有知识形成回答
4. 在回答中引用来源页面
5. 如知识不足，回溯 `raw/` 原文

### 3. 回写（Write-back）

将高质量问答/分析沉淀到 wiki。

**步骤：**
1. 在 `wiki/综合/` 创建新页面
2. 使用标准 YAML frontmatter
3. 链接到相关的概念和实体页面
4. 更新 `wiki/index.md`
5. 写入 `wiki/log.md`

### 4. 健康检查（Lint）

检查知识库一致性和完整性。

**检查项：**
- 孤儿页面（无入链的 wiki 页面）
- 断链（`[[]]` 指向不存在的页面）
- 30 天未更新的页面
- 概念重复
- index.md 覆盖度

## 触发方式

- 用户输入 `/wiki` — 显示本 Skill 的帮助信息
- 用户输入 `/wiki ingest` — 立即执行摄入
- 用户输入 `/wiki lint` — 执行健康检查
- 用户输入 "整理一下" — 执行摄入
- 用户输入 "查一下 [关键词]" — 执行查询
- 用户输入 "检查健康度" — 执行健康检查
