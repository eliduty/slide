## Why

当前项目需要创建一套基于 `ui-design-spec` 设计规范的 Slidev 主题，用于内部技术分享演示。现有 `theme-shared` 目录仅包含基础布局，未与设计规范对齐，且缺乏可扩展性设计。需要一个可发布为 npm 包的主题，支持 Token 覆盖机制，便于不同项目复用和定制。

## What Changes

- **创建新目录结构**：`packages/slidev-theme-skill-ui` 作为独立 npm 包
- **定义 Token 系统**：基于 ui-design-spec 的色彩、字号、间距、圆角、阴影 Token，支持 CSS 变量覆盖
- **实现双主题支持**：亮色/暗色主题自动切换
- **创建 10 个布局组件**：Cover、Default、Section、TopTitle、SideTitle、TwoCols、TopTitleTwoCols、Full、Quote、Credits
- **创建 4 个基础组件**：CodeBlock、Admonition、Badge、QRCode
- **实现代码高亮主题**：亮色/暗色双主题 Prism 样式
- **迁移现有内容**：将 `theme-shared` 内容迁移到新包结构
- **更新演示项目**：修改 `_template` 的主题引用路径

## Capabilities

### New Capabilities

- `theme-tokens`: 可覆盖的设计 Token 系统（色彩、字号、间距、圆角、阴影），支持亮色/暗色双主题
- `theme-layouts`: 10 个布局组件（Cover、Default、Section、TopTitle、SideTitle、TwoCols、TopTitleTwoCols、Full、Quote、Credits），响应 Token 定义
- `theme-components`: 4 个基础组件（CodeBlock、Admonition、Badge、QRCode），响应 Token 定义
- `code-highlighting`: 亮色/暗色双主题代码高亮，基于品牌色系

### Modified Capabilities

- `shared-theme`: 需要修改现有 spec，将 `theme-shared/` 目录迁移至 `packages/slidev-theme-skill-ui/`，并调整为可发布的 npm 包结构

## Impact

- **项目结构变更**：新增 `packages/` 目录，迁移 `theme-shared/` 内容
- **演示项目更新**：`presentations/_template/slides.md` 的 theme 引用路径变更
- **Token 覆盖机制**：项目可通过本地 CSS 文件覆盖主题 Token
- **布局/组件覆盖**：项目可通过本地同名文件覆盖主题布局和组件（Slidev 原生支持）
- **潜在 npm 发布**：包结构支持未来发布为 `slidev-theme-skill-ui`