## 1. 项目结构搭建

- [x] 1.1 创建 `packages/slidev-theme-skill-ui/` 目录结构
- [x] 1.2 创建 `package.json`（name: slidev-theme-skill-ui, slidev.colorSchema: auto）
- [x] 1.3 创建 `index.ts` 入口文件
- [x] 1.4 创建 `layouts/`、`components/`、`styles/` 子目录
- [x] 1.5 迁移现有 `theme-shared/layouts/` 内容到新目录
- [x] 1.6 迁移现有 `theme-shared/components/` 内容到新目录
- [x] 1.7 删除旧 `theme-shared/` 目录

## 2. Token 系统实现

- [x] 2.1 创建 `styles/variables.css` 亮色主题 Token
- [x] 2.2 定义品牌色 Token（--color-primary, --color-primary-light, --color-primary-dark）
- [x] 2.3 定义语义色 Token（--color-success, --color-warning, --color-error, --color-info）
- [x] 2.4 定义中性色 Token（--color-text-*, --color-bg-*, --color-border）
- [x] 2.5 定义字号 Token（cover/page/section/body/code）
- [x] 2.6 定义间距 Token（--spacing-xs 到 --spacing-2xl）
- [x] 2.7 定义圆角 Token（--radius-sm 到 --radius-xl）
- [x] 2.8 定义阴影 Token（--shadow-xs 到 --shadow-md）
- [x] 2.9 添加暗色主题 Token 变体（html.dark 选择器）

## 3. 基础样式文件

- [x] 3.1 创建 `styles/index.ts` 入口
- [x] 3.2 创建 `styles/base.css` 基础样式
- [x] 3.3 创建 `styles/typography.css` 字号系统样式
- [x] 3.4 创建 `styles/layouts.css` 布局通用样式

## 4. 布局组件实现

- [x] 4.1 重构 `layouts/Cover.vue` 使用 Token
- [x] 4.2 创建 `layouts/Default.vue`
- [x] 4.3 创建 `layouts/Section.vue`
- [x] 4.4 创建 `layouts/TopTitle.vue`
- [x] 4.5 创建 `layouts/SideTitle.vue`
- [x] 4.6 重构 `layouts/TwoCols.vue` 使用 Token
- [x] 4.7 创建 `layouts/TopTitleTwoCols.vue`
- [x] 4.8 创建 `layouts/Full.vue`
- [x] 4.9 创建 `layouts/Quote.vue`
- [x] 4.10 创建 `layouts/Credits.vue`

## 5. 基础组件实现

- [x] 5.1 重构 `components/CodeBlock.vue` 使用 Token
- [x] 5.2 创建 `components/Admonition.vue`（支持 info/warning/error/success 类型）
- [x] 5.3 创建 `components/Badge.vue`
- [x] 5.4 创建 `components/QRCode.vue`

## 6. 代码高亮主题

- [x] 6.1 创建 `styles/code.css` 代码块基础样式
- [x] 6.2 创建 `styles/prism-light.css` 亮色代码高亮主题
- [x] 6.3 创建 `styles/prism-dark.css` 暗色代码高亮主题
- [x] 6.4 在 `styles/index.ts` 中引入代码高亮样式

## 7. 演示项目更新

- [x] 7.1 更新 `presentations/_template/slides.md` 主题引用路径
- [x] 7.2 测试亮色主题渲染
- [x] 7.3 测试暗色主题渲染
- [x] 7.4 测试 Token 覆盖机制

## 8. 文档更新

- [x] 8.1 更新 `openspec/specs/shared-theme/spec.md` 为新结构
- [x] 8.2 验证所有 spec 文件与新实现一致