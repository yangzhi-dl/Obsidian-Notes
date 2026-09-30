# 迁移计划 — 2026-07-30

## 当前目录概况

- 根目录: ObNotes
- 已有主目录: .raw, .obsidian, .claude, .claudian, diary, notes, raw, wiki, skills, external data
- Git 仓库: 是，未提交的修改和未跟踪文件存在

## 发现的旧目录

- `raw/` — 原始资料，有子目录 `文章/`, `随记/`, `研究/(空)`
- `wiki/` — 结构化知识，有子目录 `来源/`, `概念/`, `实体/`, `综合/(空)`
- `notes/` — 用户创建的独立笔记(Markdown语法、表达能力)
- `diary/` — 日记

## 计划创建的目录

### 一级目录
- `inbox/` — 收集箱
- `archive/` — 归档
- `templates/` — 模板
- `projects/` — 项目
- `outputs/` — 输出

### raw 领域子目录
- `raw/工具/`
- `raw/技术/`
- `raw/学习/`
- `raw/投资/`
- `raw/视频创作/`
- `raw/写作表达/`
- `raw/通用/`

### wiki 领域子目录(每个7领域×5子目录)
- `wiki/{领域}/`
- `wiki/{领域}/来源/`
- `wiki/{领域}/概念/`
- `wiki/{领域}/实体/`
- `wiki/{领域}/综合/`
- `wiki/{领域}/来源/_index.md`
- `wiki/{领域}/概念/_index.md`
- `wiki/{领域}/实体/_index.md`
- `wiki/{领域}/综合/_index.md`

### 项目
- `projects/Obsidian自生长知识库/`
- `projects/投资入门/`

### 其他
- `.raw/logs/`

## 计划进行的安全迁移

### 1. raw 内容迁移
| 源文件 | 目标 | 说明 |
|--------|------|------|
| `raw/文章/architecture_full.md` | `raw/技术/文章/architecture_full.md` | 技术架构内容 |
| `raw/随记/2026-07-05-代码阅读与学习方法论.md` | `raw/学习/随记/2026-07-05-代码阅读与学习方法论.md` | 学习方法内容 |
| `raw/Web Clipper 配置指南.md` | `raw/工具/文章/Web Clipper 配置指南.md` | 工具配置内容 |

### 2. wiki 概念迁移
| 源文件 | 目标领域 | 说明 |
|--------|---------|------|
| 双向链接, 本地优先, 原子笔记, 图谱视图, MOC, 个人知识管理 | wiki/工具/概念/ | Obsidian 工具概念 |
| Obsidian, Obsidian Web Clipper | wiki/工具/实体/ | 工具实体 |
| 代码阅读方法论, 提问的艺术, 费曼学习法, 按需阅读, 问题雷达 | wiki/学习/概念/ | 学习方法概念 |
| 需求全流程, 需求澄清, 技术评审清单, 灰度发布与回滚, 项目复盘 | wiki/技术/概念/ | 技术架构概念 |
| 来源-architecture_full | wiki/技术/来源/ | 技术来源摘要 |
| 来源-代码阅读与学习方法论 | wiki/学习/来源/ | 学习来源摘要 |
| 来源-Web Clipper 配置指南 | wiki/工具/来源/ | 工具来源摘要 |

### 3. notes/ 处理
- notes/Markdown语法/Markdown语法.md → 进入 raw/通用/ 或 保留原位置
- notes/个人笔记-联系表达能力/练习表达能力.md → 进入 raw/写作表达/随记/ 或 保留原位置

## 可能存在的冲突

- `wiki/概念/` 目录下的文件移动到 `wiki/{领域}/概念/` 时，目标目录为空，无冲突
- `raw/` 下无投资/视频创作/写作表达目录，无冲突
- 不存在 `raw/理财/` 或 `wiki/理财/` 目录，无需迁移
- 不存在 `raw/笔记/` 或 `wiki/笔记/` 目录，无需迁移

## 不会执行的危险操作

- ❌ 不删除任何现有文件
- ❌ 不覆盖已有正文
- ❌ 不修改 `.obsidian/` 配置
- ❌ 不执行 Git 提交
- ❌ 不修改附件/图片/PDF
- ❌ 不批量修改已有笔记正文
- ❌ 不将 AI 生成内容标记为 evergreen
- ❌ 不为建立双链而创建空笔记
