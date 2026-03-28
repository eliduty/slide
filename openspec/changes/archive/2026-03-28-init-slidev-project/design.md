## Context

这是一个新项目初始化，目标是构建一个使用 Slidev 的个人幻灯片项目库。项目需要支持多个独立演示文稿的管理，并提供共享的主题、组件和素材复用机制。

**约束条件**：
- 使用 Slidev 作为演示构建工具
- 项目结构需要 AI 友好
- 遵循 Slidev 的设计哲学（单项目单演示、Theme/Addon 共享机制）
- 每个演示文稿需要完全独立，可单独运行、构建、导出

**参考资料**：
- docs/project-structure.md - 目录结构设计
- docs/design-decisions.md - 设计决策记录

## Goals / Non-Goals

**Goals:**

- 创建清晰的多演示文稿目录结构，每个演示完全独立
- 建立共享主题包机制，复用布局、组件和样式
- 为每个演示提供完整的素材工作区，支持从调研到产出的完整工作流
- 将元数据融入 Markdown，避免额外的 JSON 文件
- 项目结构易于 AI 理解和操作

**Non-Goals:**

- 不创建演示内容本身（仅创建结构和示例模板）
- 不实现自动化脚本或 CLI 工具
- 不配置 CI/CD 或自动化构建流程
- 不创建实际的可演示内容

## Decisions

### 1. 目录结构：扁平多目录 + 共享 Theme

**选择**：扁平多目录结构，每个演示独立目录，通过 Theme 包共享组件。

**替代方案**：
- Monorepo 方案：每个演示作为 npm package，更工程化但结构复杂
- 单项目 + 内容拆分：无法同时维护多套演示

**理由**：
- Slidev 设计哲学是单项目单演示，扁平和 Slidev 原生兼容
- AI 更易理解和导航扁平结构
- 共享 Theme 是 Slidev 原生支持的机制
- 每个演示完全独立，耦合最低

### 2. 元数据管理：融入 Markdown frontmatter

**选择**：将演示级和页级元数据直接写入 Markdown 的 YAML frontmatter。

**替代方案**：
- JSON 文件（meta.json、project.json）单独管理元数据

**理由**：
- 符合 Slidev "一切在 Markdown" 的设计理念
- AI 读取 slides.md 即可获取完整信息
- 无需维护 JSON 与 Markdown 的一致性
- git diff 更友好

### 3. 素材管理：素材跟随演示

**选择**：每个演示有自己的 workspace/ 目录，素材与演示紧密关联。

**替代方案**：
- 全局 workspace/ 按演示名分区管理

**理由**：
- 素材与演示关联直观
- 移动/删除演示时素材一起处理
- AI 能直接理解素材归属
- 全局共享素材有专门位置（assets-shared/）

### 4. 项目索引：README.md

**选择**：使用 README.md 作为项目索引，列出所有演示和结构说明。

**替代方案**：
- project.json 作为机器可读索引

**理由**：
- README.md 是项目标配，无需额外文件
- Markdown 格式对人友好，AI 也易理解
- 可包含使用说明和快速开始指南

## Risks / Trade-offs

| Risk | Mitigation |
|------|------------|
| 共享主题路径引用（../theme-shared）在不同层级可能失效 | 统一约定每个演示引用相对路径 `../theme-shared` |
| 素材工作区增加目录深度 | 接受深度换取独立性，AI 已理解结构 |
| 演示增多时 README.md 维护负担 | README.md 记录核心信息，详细元数据在 slides.md |