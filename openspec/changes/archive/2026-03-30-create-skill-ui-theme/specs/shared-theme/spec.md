## REMOVED Requirements

### Requirement: Shared theme directory
**Reason**: 目录迁移至 `packages/slidev-theme-skill-ui/`，采用可发布的 npm 包结构。
**Migration**: 使用新的主题包路径 `packages/slidev-theme-skill-ui/`，演示项目需更新 `theme` 引用路径。

## ADDED Requirements

### Requirement: Theme package structure
主题 SHALL 位于 `packages/slidev-theme-skill-ui/` 目录，符合 npm 包结构。

#### Scenario: Package directory exists
- **WHEN** 查看项目目录
- **THEN** SHALL 存在 `packages/slidev-theme-skill-ui/` 目录

#### Scenario: Package.json defined
- **WHEN** 查看主题包目录
- **THEN** SHALL 存在 `package.json` 文件
- **AND** `name` 字段为 `slidev-theme-skill-ui`
- **AND** 包含 `slidev` 配置字段（`colorSchema: "auto"`）

### Requirement: Theme layouts directory
主题包 SHALL 包含 `layouts/` 目录存放布局组件。

#### Scenario: Layouts directory exists
- **WHEN** 查看主题包目录
- **THEN** SHALL 存在 `layouts/` 目录

#### Scenario: Layout files available
- **WHEN** 查看主题包 `layouts/` 目录
- **THEN** SHALL 包含 Cover.vue、Default.vue、Section.vue 等布局文件

### Requirement: Theme components directory
主题包 SHALL 包含 `components/` 目录存放 Vue 组件。

#### Scenario: Components directory exists
- **WHEN** 查看主题包目录
- **THEN** SHALL 存在 `components/` 目录

#### Scenario: Component files available
- **WHEN** 查看主题包 `components/` 目录
- **THEN** SHALL 包含 CodeBlock.vue、Admonition.vue 等组件文件

### Requirement: Theme styles directory
主题包 SHALL 包含 `styles/` 目录存放全局样式。

#### Scenario: Styles directory exists
- **WHEN** 查看主题包目录
- **THEN** SHALL 存在 `styles/` 目录

#### Scenario: Style files available
- **WHEN** 查看主题包 `styles/` 目录
- **THEN** SHALL 包含 `variables.css`（Token 定义）、`base.css`、`layouts.css`、`code.css` 等文件

### Requirement: Presentation references theme package
演示项目 SHALL 在 frontmatter 中引用主题包。

#### Scenario: Reference theme with relative path
- **WHEN** 创建新演示
- **THEN** slides.md frontmatter SHALL 设置 `theme: ../../packages/slidev-theme-skill-ui`