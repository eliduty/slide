## ADDED Requirements

### Requirement: Presentations directory structure
项目 SHALL 包含 `presentations/` 目录用于存放所有演示文稿，每个演示文稿作为独立子目录存在。

#### Scenario: Create presentation directory
- **WHEN** 创建新演示文稿
- **THEN** 在 `presentations/` 下创建独立的子目录，目录名作为演示唯一标识

#### Scenario: Each presentation is independent
- **WHEN** 查看 `presentations/` 目录下的任意演示
- **THEN** 该演示 SHALL 包含完整的 Slidev 项目结构（slides.md、slides/、public/ 等），可独立运行

### Requirement: Shared assets directory
项目 SHALL 包含 `assets-shared/` 目录用于存放全局共享素材。

#### Scenario: Global icons accessible
- **WHEN** 演示需要使用通用图标
- **THEN** 可从 `assets-shared/icons/` 引用

#### Scenario: Brand assets shared
- **WHEN** 多个演示需要使用品牌资源（logo 等）
- **THEN** 资源 SHALL 存放在 `assets-shared/brand/`，所有演示可引用

### Requirement: Docs directory for design records
项目 SHALL 包含 `docs/` 目录用于存放设计决策和规范文档。

#### Scenario: Design decisions documented
- **WHEN** 查看项目设计决策
- **THEN** 可在 `docs/design-decisions.md` 找到完整的决策记录

#### Scenario: Specifications documented
- **WHEN** 查看目录结构规范或元数据规范
- **THEN** 可在 `docs/` 下找到对应的规范文档

### Requirement: Root README as project index
项目根目录 SHALL 包含 `README.md` 作为项目索引，列出所有演示文稿和结构说明。

#### Scenario: View presentation list
- **WHEN** 打开 README.md
- **THEN** SHALL 看到演示列表表格（包含 ID、标题、状态、页数、标签、更新日期）

#### Scenario: Understand directory structure
- **WHEN** 打开 README.md
- **THEN** SHALL 看到目录结构简要说明

### Requirement: Root package.json for dependencies
项目根目录 SHALL 包含 `package.json` 管理项目依赖。

#### Scenario: Install Slidev dependency
- **WHEN** 运行 `pnpm install` 或 `npm install`
- **THEN** Slidev 及相关依赖 SHALL 正确安装