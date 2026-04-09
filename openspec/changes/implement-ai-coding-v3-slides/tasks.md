## 1. 准备工作

- [x] 1.1 创建 slides/ 目录结构
- [x] 1.2 确认 v2 版本文件列表和内容作为参考

## 2. Part 0 开场（4页）

- [x] 2.1 创建 01-cover.md（封面页，layout: cover）
- [x] 2.2 创建 02-pain-points.md（痛点引入，layout: Default）
- [x] 2.3 创建 03-industry-trend.md（行业趋势，layout: Default）
- [x] 2.4 创建 04-methodology.md（方法论演进，layout: Default 或 TwoCols）

## 3. Part 1 背景铺垫（5页）

- [x] 3.1 创建 05-chapter1-section.md（章节页，layout: Section）
- [x] 3.2 创建 06-ai-ability.md（AI能力等级，复用v2样式）
- [x] 3.3 创建 07-what-is-sdd.md（什么是SDD，layout: Default）
- [x] 3.4 创建 08-why-sdd.md（为什么需要SDD，layout: Default）
- [x] 3.5 创建 09-human-ai-boundary.md（人机协作边界，layout: Default）

## 4. Part 2 工具与协作框架（5页）

- [x] 4.1 创建 10-chapter2-section.md（章节页，layout: Section）
- [x] 4.2 创建 11-three-tools.md（三大工具概览，layout: Default 或 TwoCols）
- [x] 4.3 创建 12-agent-mcp-skill.md（Agent/MCP/Skill概念体系，layout: Default）
- [x] 4.4 创建 13-work-framework.md（工作开展框架，layout: Default）
- [x] 4.5 创建 14-learning-path.md（学习路径指引，layout: Default）

## 5. Part 3 四阶段工作流程（7页）

- [x] 5.1 创建 15-chapter3-section.md（章节页，layout: Section）
- [x] 5.2 创建 16-four-phases-overview.md（四阶段总览，layout: Default）
- [x] 5.3 创建 17-requirement-phase.md（需求阶段，layout: Default）
- [x] 5.4 创建 18-design-phase.md（设计阶段，layout: Default）
- [x] 5.5 创建 19-env-phase.md（环境规范阶段，layout: Default）
- [x] 5.6 创建 20-implementation-phase.md（实现阶段，layout: Default）
- [x] 5.7 创建 21-phase-summary.md（阶段总结，layout: Default）

## 6. Part 4 工具作用于工作流（6页）

- [x] 6.1 创建 22-chapter4-section.md（章节页，layout: Section）
- [x] 6.2 创建 23-requirement-application.md（需求阶段应用，layout: Default）
- [x] 6.3 创建 24-design-application.md（设计阶段应用，layout: Default）
- [x] 6.4 创建 25-implementation-application.md（实现阶段应用，layout: Default）
- [x] 6.5 创建 26-global-application.md（全局应用，layout: Default）
- [x] 6.6 创建 27-application-summary.md（阶段总结，layout: Default）

## 7. Part 5-8 复用v2版本（约15页）

- [x] 7.1 复制 v2 17-chapter3-section.md → 28-chapter5-section.md
- [x] 7.2 复制 v2 18-chapter3-pm.md → 29-pm-impact.md
- [x] 7.3 复制 v2 19-chapter3-sdeqa.md → 30-sdeqa-impact.md
- [x] 7.4 复制 v2 20-chapter3-review.md → 31-review-impact.md
- [x] 7.5 复制 v2 21-chapter3-summary.md → 32-human-work-adjust.md
- [x] 7.6 复制 v2 22-chapter5-section.md → 33-chapter6-section.md
- [x] 7.7 复制 v2 23-chapter5-legacy.md → 34-legacy-project.md
- [x] 7.8 复制 v2 24-chapter5-new.md → 35-new-project.md
- [x] 7.9 复制 v2 25-assets.md → 36-assets-list.md
- [x] 7.10 复制 v2 26-assets-full.md → 37-assets-structure.md
- [x] 7.11 复制 v2 27-self-study.md → 38-self-study.md
- [x] 7.12 复制 v2 28-summary.md → 39-summary.md
- [x] 7.13 复制 v2 29-credits.md → 40-qa.md

## 8. 入口文件更新

- [x] 8.1 更新 slides.md 元数据（slidesCount: 40, estimatedTime: 80min）
- [x] 8.2 添加所有 src 引用（按顺序引用 01-40）
- [x] 8.3 添加章节注释（<!-- Part X -->）

## 9. 验证

- [x] 9.1 运行 `pnpm dev:ai-coding-v3` 验证幻灯片可正常显示
- [x] 9.2 检查所有 src 引用路径有效，无缺失文件
- [x] 9.3 验证页面渲染正确，样式一致