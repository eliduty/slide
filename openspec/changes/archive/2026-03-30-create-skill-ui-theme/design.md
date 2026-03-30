## Context

当前项目使用 Slidev 构建幻灯片，`theme-shared/` 目录包含基础的共享主题。现有主题存在以下问题：
- 未与 `docs/ui-spec/ui-design-spec.md` 设计规范对齐
- Token 系统（色彩、字号、间距）缺失
- 布局数量不足，仅 Cover 和 TwoColumn
- 无代码高亮主题定义
- 目录结构不支持 npm 发布

目标用户：内部技术分享演示，需要展示代码块，支持亮色/暗色双主题。

约束条件：
- 必须基于 ui-design-spec 的色彩系统（品牌色 `#4361EE`）
- Token 必须可被项目级 CSS 覆盖
- 布局/组件可被项目同名文件覆盖（Slidev 原生支持）

## Goals / Non-Goals

**Goals:**
- 创建可发布的 npm 包 `slidev-theme-skill-ui`
- 定义完整 Token 系统（色彩、字号、间距、圆角、阴影）
- 实现 Token 覆盖机制（CSS 变量后置覆盖）
- 支持亮色/暗色双主题自动切换
- 提供 10 个布局组件
- 提供 4 个基础组件
- 定义双主题代码高亮样式

**Non-Goals:**
- 不实现图表/数据可视化组件（后续按需添加）
- 不实现复杂动画特效
- 不实现多语言支持
- 不定义 z-index 层级系统（Slidev 内置处理）

## Decisions

### D1: Token 系统实现方式

**选择：CSS 变量方案**

**理由：**
- 与 ui-design-spec 的 TDesign CSS Variables 覆盖模式一致
- Slidev 支持在 `global-top.vue` 或项目 CSS 中后置覆盖
- 无需额外配置系统，降低使用门槛

**备选方案：**
- A) 配置驱动（frontmatter 配置 Token）→ 实现复杂度高，配置过多
- B) SCSS 变量 → 编译时固定，无法动态覆盖

### D2: 目录结构

**选择：`packages/slidev-theme-skill-ui/`**

**理由：**
- 明确区分「可发布包」与「项目资源」
- `packages/` 是 monorepo 常见约定
- 未来可独立发布 npm 包

**备选方案：**
- A) 保持 `theme-shared/` → 名称不具语义，难以识别用途
- B) `@skill/theme-ui-spec` → 不符合 Slidev 主题命名惯例 `slidev-theme-*`

### D3: 布局设计

**选择：参考 Neversink 简化实现**

**理由：**
- Neversink 提供完整的布局类型参考
- 简化参数，只保留必要 frontmatter 选项
- 布局响应 Token，而非硬编码样式

**保留的布局：**
Cover, Default, Section, TopTitle, SideTitle, TwoCols, TopTitleTwoCols, Full, Quote, Credits

**简化原则：**
- 不实现 Neversink 的复杂对齐参数（`align: lt/l-lt-lt`）
- 通过 CSS Flexbox/Grid 自动处理对齐

### D4: 字号放大策略

**选择：单独定义每种用途的字号 Token**

**理由：**
- 幻灯片场景与 B 端应用差异大
- 封面标题（64px）与页面标题（40px）需要不同处理
- 便于项目按需覆盖特定字号

**字号 Token 映射：**
| 用途 | Token | 默认值 |
|------|-------|--------|
| 封面标题 | `--font-size-cover-title` | 64px |
| 封面副标题 | `--font-size-cover-subtitle` | 28px |
| 页面标题 | `--font-size-page-title` | 40px |
| 章节标题 | `--font-size-section-title` | 48px |
| 区块标题 | `--font-size-heading` | 32px |
| 正文 | `--font-size-body` | 24px |
| 辅助文字 | `--font-size-body-sm` | 18px |
| 代码块 | `--font-size-code` | 18px |

### D5: 暗色主题扩展

**选择：基于亮色 Token 推导暗色变体**

**理由：**
- ui-design-spec 未定义暗色主题
- 幻灯片投影环境常需要暗色背景
- 使用 CSS 变量 `html.dark { ... }` 自动切换

**暗色 Token 定义：**
| Token | 亮色值 | 暗色值 |
|-------|--------|--------|
| `--color-text-primary` | #1A1A2E | #F7FAFC |
| `--color-text-secondary` | #6B7280 | #A0AEC0 |
| `--color-bg-page` | #F5F7FA | #1A1A2E |
| `--color-bg-card` | #FFFFFF | #2D3748 |
| `--color-border` | #E5E7EB | #4A5568 |

品牌色在暗色主题保持不变，确保视觉一致性。

## Risks / Trade-offs

**[R1] Token 覆盖可能导致样式冲突**
- **Mitigation**: 覆盖 CSS 必须在主题 CSS 之后加载，使用更高优先级选择器

**[R2] 暗色主题色彩未经 ui-design-spec 定义**
- **Mitigation**: 暗色 Token 基于亮色 Token 对比度推导，保持 WCAG AA 标准

**[R3] 布局覆盖可能导致功能缺失**
- **Mitigation**: 文档说明布局覆盖机制，提供示例

**[R4] 包发布后的版本管理**
- **Mitigation**: 使用 SemVer，变更 Token 名称时升级 major 版本

## Migration Plan

**Phase 1: 结构调整**
1. 创建 `packages/slidev-theme-skill-ui/` 目录
2. 迁移 `theme-shared/layouts/` 内容
3. 迁移 `theme-shared/components/` 内容
4. 删除 `theme-shared/` 目录

**Phase 2: Token 系统**
1. 创建 `styles/variables.css`（亮色 Token）
2. 添加暗色 Token 变体
3. 创建字号/间距/圆角/阴影 Token

**Phase 3: 布局组件**
1. 重构现有布局使用 Token
2. 新增布局组件
3. 创建 `layouts.css` 布局样式

**Phase 4: 基础组件**
1. 重构 CodeBlock 使用 Token
2. 新增 Admonition、Badge、QRCode

**Phase 5: 代码高亮**
1. 创建 `prism-light.css`
2. 创建 `prism-dark.css`

**Phase 6: 演示项目更新**
1. 更新 `_template/slides.md` 主题引用
2. 测试双主题切换

**Rollback**: 可通过 Git 回滚，无破坏性操作。

## Open Questions

- 无待解决问题，设计已明确。