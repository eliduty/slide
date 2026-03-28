## 1. 项目根目录初始化

- [x] 1.1 创建项目根目录 `package.json`，包含 Slidev 依赖
- [x] 1.2 创建 `README.md` 项目索引文件，包含目录结构说明占位
- [x] 1.3 创建 `assets-shared/` 目录及子目录（icons/、brand/、templates/、fonts/）
- [x] 1.4 创建 `theme-shared/` 目录及子目录（layouts/、components/、styles/）

## 2. 共享主题包初始化

- [x] 2.1 创建 `theme-shared/package.json`，定义主题包信息
- [x] 2.2 创建 `theme-shared/styles/index.ts` 样式入口文件
- [x] 2.3 创建 `theme-shared/styles/base.css` 基础样式
- [x] 2.4 创建示例布局组件 `theme-shared/layouts/TwoColumn.vue`
- [x] 2.5 创建示例布局组件 `theme-shared/layouts/Cover.vue`
- [x] 2.6 创建示例组件 `theme-shared/components/CodeBlock.vue`

## 3. 演示文稿模板创建

- [x] 3.1 创建 `presentations/` 目录
- [x] 3.2 创建示例演示 `presentations/_template/` 目录（作为新演示模板参考）
- [x] 3.3 创建模板 `slides.md`，包含完整元数据示例
- [x] 3.4 创建模板 `slides/` 目录及示例文件（01-cover.md、02-intro.md、03-summary.md）
- [x] 3.5 创建模板 `workspace/` 目录及所有子文件（research.md、outline.md、references.md、feedback.md）
- [x] 3.6 创建模板 `workspace/scripts/` 目录
- [x] 3.7 创建模板 `workspace/data/` 目录
- [x] 3.8 创建模板 `workspace/drafts/` 目录
- [x] 3.9 创建模板 `public/` 目录及子目录（images/、diagrams/）
- [x] 3.10 创建模板 `archive/` 目录

## 4. 文档完善

- [x] 4.1 更新 `README.md`，填充演示列表和目录结构说明
- [x] 4.2 验证 `docs/project-structure.md` 与实际结构一致
- [x] 4.3 验证 `docs/metadata-spec.md` 与模板 slides.md 一致
- [x] 4.4 验证 `docs/workspace-spec.md` 与模板 workspace 结构一致

## 5. 验证与测试

- [x] 5.1 安装项目依赖（pnpm install）
- [x] 5.2 创建一个测试演示（复制模板目录为 test-demo）
- [x] 5.3 运行测试演示验证 Slidev 是否正常工作
- [x] 5.4 验证共享主题是否正确加载
- [x] 5.5 删除测试演示目录