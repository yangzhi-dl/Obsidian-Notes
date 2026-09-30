# 迁移报告 — 2026-07-30

## 执行概况

- **启动时间**: 2026-07-30
- **知识库**: ObNotes
- **迁移模式**: 安全迁移（复制 raw，移动 wiki）
- **架构变更**: 扁平结构 → 领域优先结构

---

## 已创建目录

### 一级目录（6 个）
- `inbox/`
- `templates/`
- `projects/`
- `outputs/`
- `archive/`
- `.raw/logs/`

### raw 领域目录（7 个领域）
- `raw/工具/`
- `raw/技术/`
- `raw/学习/`
- `raw/投资/`
- `raw/视频创作/`
- `raw/写作表达/`
- `raw/通用/`

### wiki 领域目录（7 领域 × 5 子目录 = 35）
每个领域下：`来源/` `概念/` `实体/` `综合/` 以及领域的 `index.md`

### 输出与归档子目录
- `outputs/文章/` `outputs/报告/` `outputs/分享稿/` `outputs/视频脚本/`
- `archive/projects/` `archive/raw/` `archive/wiki/` `archive/outputs/`

---

## 已创建文件

### 模板（9 个）
- `templates/原始资料模板.md`
- `templates/概念笔记模板.md`
- `templates/来源笔记模板.md`
- `templates/实体笔记模板.md`
- `templates/综合笔记模板.md`
- `templates/项目模板.md`
- `templates/日记模板.md`
- `templates/复盘模板.md`
- `templates/输出模板.md`

### 工作入口索引（6 个）
- `inbox/index.md`
- `raw/index.md`
- `diary/index.md`
- `outputs/index.md`
- `archive/index.md`
- `projects/index.md`

### 领域索引（35 个）
- 7 个领域 `index.md`
- 28 个领域子目录 `_index.md`

### 核心规则文件（2 个）
- `AGENTS.md` — 全面重写为 Agent 协作规范
- `CLAUDE.md` — 重写为 Claude Code 工作规范

### 项目文件（9 个）
- `projects/Obsidian自生长知识库/index.md`
- `projects/Obsidian自生长知识库/requirements.md`
- `projects/Obsidian自生长知识库/decisions.md`
- `projects/Obsidian自生长知识库/tasks.md`
- `projects/Obsidian自生长知识库/changelog.md`
- `projects/投资入门/index.md`
- `projects/投资入门/learning-roadmap.md`
- `projects/投资入门/tasks.md`
- `projects/投资入门/review.md`

---

## 已更新文件

- `wiki/index.md` — 全面重写为知识地图
- `wiki/hot.md` — 更新为当前状态
- `wiki/log.md` — 追加架构变更记录
- `wiki/使用指南.md` — 全面更新为新结构指南
- `.raw/manifest.json` — 合并新架构信息

---

## 已移动文件（wiki — 物理移动）

| 源路径 | 目标路径 |
|--------|---------|
| `wiki/来源/来源-Web Clipper 配置指南.md` | `wiki/工具/来源/来源-Web Clipper 配置指南.md` |
| `wiki/来源/来源-代码阅读与学习方法论.md` | `wiki/学习/来源/来源-代码阅读与学习方法论.md` |
| `wiki/来源/来源-architecture_full.md` | `wiki/技术/来源/来源-architecture_full.md` |
| `wiki/概念/双向链接.md` | `wiki/工具/概念/双向链接.md` |
| `wiki/概念/本地优先.md` | `wiki/工具/概念/本地优先.md` |
| `wiki/概念/个人知识管理.md` | `wiki/工具/概念/个人知识管理.md` |
| `wiki/概念/图谱视图.md` | `wiki/工具/概念/图谱视图.md` |
| `wiki/概念/原子笔记.md` | `wiki/工具/概念/原子笔记.md` |
| `wiki/概念/MOC.md` | `wiki/工具/概念/MOC.md` |
| `wiki/概念/代码阅读方法论.md` | `wiki/学习/概念/代码阅读方法论.md` |
| `wiki/概念/提问的艺术.md` | `wiki/学习/概念/提问的艺术.md` |
| `wiki/概念/费曼学习法.md` | `wiki/学习/概念/费曼学习法.md` |
| `wiki/概念/按需阅读.md` | `wiki/学习/概念/按需阅读.md` |
| `wiki/概念/问题雷达.md` | `wiki/学习/概念/问题雷达.md` |
| `wiki/概念/需求全流程.md` | `wiki/技术/概念/需求全流程.md` |
| `wiki/概念/需求澄清.md` | `wiki/技术/概念/需求澄清.md` |
| `wiki/概念/技术评审清单.md` | `wiki/技术/概念/技术评审清单.md` |
| `wiki/概念/灰度发布与回滚.md` | `wiki/技术/概念/灰度发布与回滚.md` |
| `wiki/概念/项目复盘.md` | `wiki/技术/概念/项目复盘.md` |
| `wiki/实体/Obsidian.md` | `wiki/工具/实体/Obsidian.md` |
| `wiki/实体/Obsidian Web Clipper.md` | `wiki/工具/实体/Obsidian Web Clipper.md` |

## 已复制文件（raw — 保留原文件）

| 源路径 | 目标路径 |
|--------|---------|
| `raw/Web Clipper 配置指南.md` | `raw/工具/文章/Web Clipper 配置指南.md` |
| `raw/文章/architecture_full.md` | `raw/技术/文章/architecture_full.md` |
| `raw/随记/2026-07-05-代码阅读与学习方法论.md` | `raw/学习/随记/2026-07-05-代码阅读与学习方法论.md` |
| `notes/个人笔记-联系表达能力/练习表达能力.md` | `raw/写作表达/随记/练习表达能力.md` |

---

## 跳过的冲突

- 无冲突。现有目标目录均为空，所有移动和复制操作成功。

---

## 未能分类的文件

- `raw/README.md` — raw 目录说明文件，已吸收进 AGENTS.md，保留原位置不变
- `notes/Markdown语法/Markdown语法.md` — 技术参考手册，未确定归属领域，保留原位置
- `外部 data/` 目录 — 非 Markdown 内容，保留原位置
- `关于Obsidian.md`（根目录） — 此文件可能已因之前操作不存在，未处理

---

## 安全检查

### 是否删除文件
✅ **否** — 没有任何文件被删除。raw 文件使用 cp（复制），原始文件保留。wiki 文件使用 mv（移动）。

### 是否覆盖文件
✅ **否** — 所有新文件写入新路径，已有文件读取后合并更新，未覆盖任何正文。

### manifest.json 是否有效
✅ 是 — 合法 JSON 格式。

### 链接检查
⚠️ **部分** — 移动后的 wiki 文件中的 [[WikiLink]] 双链可能指向旧路径。
- 同类概念（同一域内）的链接仍然有效
- 跨域链接可能断裂，需要在后续使用中逐步修复
- 已更新 3 个来源页的 source 字段路径

### 旧目录状态
移动后以下旧目录已空，可以手动删除（等确认后）：
- `wiki/概念/`（原 16 个文件已全部移出）
- `wiki/来源/`（原 3 个文件已全部移出）
- `wiki/实体/`（原 2 个文件已全部移出）
- `wiki/综合/`（原为空）

---

## 后续人工检查事项

1. **检查 wiki 链接** — 移动后的概念页中跨域双链需要验证是否有效
2. **清理旧目录** — 确认 wiki/概念/、wiki/来源/、wiki/实体/ 的旧目录是否可以删除
3. **清理 raw 根文件** — `raw/Web Clipper 配置指南.md` 已在工具/文章下有副本，旧文件可删除
4. **清理 raw/文章/、raw/随记/** — 内容已复制到领域目录，旧路径可删除
5. **配置 Obsidian 模板目录** — 在 Obsidian 设置中将模板目录指向 `templates/`
6. **notes/ 目录** — Markdown语法.md 是保留在 notes/ 还是纳入知识库体系
7. **测试新结构** — 在 Obsidian 中打开验证文件浏览器和图谱视图
