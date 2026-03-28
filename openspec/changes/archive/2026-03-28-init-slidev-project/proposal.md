## Why

需要一个使用 Slidev 构建的个人幻灯片项目库，支持管理多个独立的演示文稿，并能够复用共享的主题、组件和素材。同时，项目结构需要对 AI 友好，便于 AI 理解、编辑和生成幻灯片内容。

## What Changes

- 创建多演示文稿的项目结构（presentations/ 目录）
- 创建共享主题包（theme-shared/）提供统一的布局、组件和样式
- 创建全局共享素材池（assets-shared/）管理图标、品牌资源等
- 为每个演示文稿创建完整的素材工作区（workspace/），包括调研笔记、大纲、演讲脚本、数据源、草稿、反馈记录
- 建立元数据规范，将演示级和页级元数据融入 Markdown frontmatter
- 创建 README.md 作为项目索引
- 创建 docs/ 目录记录设计决策和规范文档

## Capabilities

### New Capabilities

- `project-structure`: 多演示文稿的目录组织结构，包括 presentations/、assets-shared/、theme-shared/、docs/
- `presentation-workspace`: 每个演示的素材工作区，包括 research.md、outline.md、references.md、scripts/、data/、drafts/、feedback.md
- `metadata-schema`: slides.md 演示级元数据和 slides/*.md 页级元数据的规范定义
- `shared-theme`: 共享主题包，提供可复用的布局、组件和样式

### Modified Capabilities

无（这是新项目初始化）

## Impact

- 新项目初始化，无现有代码影响
- 依赖 Slidev 作为演示构建工具
- 项目结构设计为 AI 友好，便于后续使用 AI 协助管理