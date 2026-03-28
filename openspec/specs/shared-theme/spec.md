## ADDED Requirements

### Requirement: Shared theme directory
项目 SHALL 包含 `theme-shared/` 目录作为共享主题包。

#### Scenario: Locate shared theme
- **WHEN** 查看项目目录
- **THEN** SHALL 存在 `theme-shared/` 目录

### Requirement: Theme layouts directory
theme-shared/ SHALL 包含 `layouts/` 目录存放可复用的布局组件。

#### Scenario: Use shared layout in presentation
- **WHEN** 演示需要使用共享布局
- **THEN** 可在 slides.md frontmatter 设置 `theme: ../theme-shared`，布局 SHALL 自动可用

### Requirement: Theme components directory
theme-shared/ SHALL 包含 `components/` 目录存放可复用的 Vue 组件。

#### Scenario: Use shared component in slides
- **WHEN** 幻灯片需要使用共享组件（如 CodeBlock、Timeline）
- **THEN** 组件 SHALL 自动全局注册，无需手动 import

### Requirement: Theme styles directory
theme-shared/ SHALL 包含 `styles/` 目录存放全局样式。

#### Scenario: Apply shared styles
- **WHEN** 演示使用共享主题
- **THEN** 全局样式 SHALL 自动注入到所有幻灯片

### Requirement: Theme package.json for npm packaging
theme-shared/ SHALL 包含 `package.json` 定义主题包信息。

#### Scenario: Publish theme as npm package
- **WHEN** 需要将主题发布为 npm 包
- **THEN** package.json SHALL 包含正确的 `name`、`slidev` 配置字段

### Requirement: Presentation references shared theme
每个演示的 slides.md SHALL 在 frontmatter 中引用共享主题。

#### Scenario: Reference theme with relative path
- **WHEN** 创建新演示
- **THEN** slides.md frontmatter SHALL 设置 `theme: ../theme-shared`