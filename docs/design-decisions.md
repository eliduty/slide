# 设计决策记录

## 核心决策

| 决策点 | 选择 | 原因 |
|--------|------|------|
| 目录结构 | 扁平多目录 + 共享 Theme | 符合 Slidev 设计、AI易理解、独立性强 |
| 元数据管理 | 融入 Markdown frontmatter | 文件更少、符合 Slidev 理念、git友好 |
| 项目索引 | README.md | 无需额外 JSON 文件 |
| 素材管理 | 素材跟随演示 + 全局共享池 | 关联直观、独立性强、共享有专门位置 |
| 版本归档 | 按日期命名 | 更直观、便于追溯 |
| 变更记录 | 不需要 | git commit 已记录，避免冗余 |

---

## 方案对比记录

### 目录结构方案

**对比了两种方案**：

1. **扁平多目录** - 每个演示独立目录，共享通过 Theme 实现
2. **Monorepo** - 每个演示作为 npm package，通过包依赖共享

**选择**：扁平多目录

**原因**：
- Slidev 官方设计是单项目单演示，Monorepo 需要额外配置
- 扁平结构 AI 更易理解和导航
- 共享 Theme 是 Slidev 原生支持的机制

---

### 元数据方案

**对比了两种方案**：

1. **JSON + Markdown 分离** - meta.json + slides.md
2. **纯 Markdown** - 元数据融入 frontmatter

**选择**：纯 Markdown

**原因**：
- 符合 Slidev "一切在 Markdown" 的设计理念
- AI 读取 slides.md 即可获取完整信息
- 无需维护 JSON 与 Markdown 的一致性
- git diff 更友好

---

### 素材管理方案

**对比了两种方案**：

1. **素材跟随演示** - workspace/ 在每个演示目录内
2. **素材集中管理** - 全局 workspace/ 按演示名分区

**选择**：素材跟随演示 + 全局共享池

**原因**：
- 素材与演示关联直观
- 每个演示完全独立，移动/删除时素材一起处理
- 全局共享素材有专门位置 (assets-shared/)
- AI 能直接理解素材归属

---

### 版本归档命名

**对比了两种方案**：

1. 按版本号：`v1/`, `v2/`
2. 按日期：`2026-03-15/`

**选择**：按日期

**原因**：
- 日期更直观，便于追溯历史
- 避免版本号管理复杂性

---

## 其他讨论结论

### workspace/ 子目录

暂不添加更多子目录，现有结构已满足需求：
- research.md
- outline.md
- references.md
- scripts/
- data/
- drafts/
- feedback.md

### CHANGELOG.md

不需要。git commit 已记录变更历史，避免冗余。

### theme-shared workspace

不需要。共享主题是产出而非创作，不需要素材工作区。