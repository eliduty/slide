# UI 设计规范

> 版本：v1.0.0 | 更新日期：2026-03-06
>
> 本文档适用于所有前端应用：admin-web、institution-web、assessee-web、assessee-h5、portal-web。
> 所有 UI 相关的开发决策应以此文档为基准，后续组件库选型完成后在本文档基础上扩展。

---

## 1. 设计原则

| 原则 | 说明 |
|------|------|
| **简洁（Less is More）** | 减少视觉噪音，充分利用留白，只呈现当前任务所需的信息 |
| **一致（Consistency）** | 跨五个应用保持视觉语言统一，相同语义的元素使用相同的样式 |
| **高效（Efficiency）** | 信息密度合理，核心操作路径不超过三步，减少用户认知负担 |
| **可信（Trustworthiness）** | 专业、克制的视觉风格，适合 B 端机构用户与测评场景 |

---

## 2. 色彩系统

### 2.1 品牌色

| Token | 色值 | 用途 |
|-------|------|------|
| `color-primary` | `#4361EE` | 主按钮、链接、激活态、进度条 |
| `color-primary-light` | `#EEF1FD` | 选中背景、标签背景、浅色填充 |
| `color-primary-dark` | `#2D4BC7` | Hover 态、按下态 |

### 2.2 语义色

| Token | 色值 | 用途 |
|-------|------|------|
| `color-success` | `#22C55E` | 通过、完成、正常状态 |
| `color-success-light` | `#DCFCE7` | 成功状态背景 |
| `color-warning` | `#F59E0B` | 待处理、注意、提醒 |
| `color-warning-light` | `#FEF3C7` | 警告状态背景 |
| `color-error` | `#EF4444` | 失败、错误、必填校验 |
| `color-error-light` | `#FEE2E2` | 错误状态背景 |
| `color-info` | `#3B82F6` | 提示信息、说明 |
| `color-info-light` | `#DBEAFE` | 信息状态背景 |

### 2.3 中性色

| Token | 色值 | 用途 |
|-------|------|------|
| `color-text-primary` | `#1A1A2E` | 正文、标题 |
| `color-text-secondary` | `#6B7280` | 描述、辅助文字、占位符 |
| `color-text-disabled` | `#C4C4C4` | 禁用态文字 |
| `color-border` | `#E5E7EB` | 输入框边框、分割线、表格边框 |
| `color-bg-page` | `#F5F7FA` | 页面背景 |
| `color-bg-card` | `#FFFFFF` | 卡片、弹窗、表单背景 |
| `color-bg-hover` | `#F9FAFB` | 列表项 Hover 背景 |

### 2.4 使用规范

- **禁止**使用上表之外的自定义色值，如需扩展请在本文档中追加 Token
- 文字与背景的对比度须满足 WCAG AA 标准（正文 ≥ 4.5:1，大字 ≥ 3:1）
- 语义色仅用于对应的状态场景，不得挪作装饰用途
- **图表扩展色**：institution-web 图表配色基于 `color-primary` 按固定步长（+30° 色相旋转或降低饱和度）派生，不得随意引入无关色彩
- **暗色模式**：当前版本仅定义亮色主题；后续如有暗色需求，另行添加 `[token]-dark` 变体，不覆盖现有 Token

---

## 3. 字体系统

### 3.1 字体族

```css
font-family: -apple-system, BlinkMacSystemFont, "PingFang SC", "Microsoft YaHei",
             "Helvetica Neue", Arial, sans-serif;
```

### 3.2 字号比例

| Token | 字号 | 行高 | 字重 | 用途 |
|-------|------|------|------|------|
| `text-h1` | 32px | 1.3 | 400 | 页面主标题 |
| `text-h2` | 24px | 1.4 | 400 | 区块标题 |
| `text-h3` | 20px | 1.4 | 400 | 卡片标题、弹窗标题 |
| `text-h4` | 18px | 1.5 | 400 | 子区块标题 |
| `text-body-lg` | 16px | 1.6 | 400 | 正文大号 |
| `text-body` | 14px | 1.6 | 400 | 正文（默认） |
| `text-body-sm` | 13px | 1.6 | 400 | 辅助说明 |
| `text-caption` | 12px | 1.5 | 400 | 标注、时间戳、版权信息 |

### 3.3 字重规则

| 字重值 | 用途 |
|--------|------|
| `400` | H1、H2 标题及正文、表单、按钮等绝大多数场景；H1/H2 的轻盈感通过大字号 + 宽行高实现，不依赖字重 300（中文字体通常无此字重） |
| `600` | 强调文字、数值高亮、表头 |

> assessee-h5 移动端：`text-body` 调整为 15px，`text-body-lg` 调整为 17px，保证触屏可读性。

---

## 4. 间距与布局

### 4.1 基础单位

间距基础单位为 **4px**，所有间距值均为 4 的倍数。

### 4.2 间距档位

| Token | 值 | 常用场景 |
|-------|----|---------|
| `spacing-1` | 4px | 图标与文字间距、紧凑标签内边距 |
| `spacing-2` | 8px | 行内元素间距、小组件内边距 |
| `spacing-3` | 12px | 表单项内边距、紧凑卡片内边距 |
| `spacing-4` | 16px | 标准内边距、列表项间距（默认） |
| `spacing-5` | 20px | 表单项间距、中等组件内边距 |
| `spacing-6` | 24px | 卡片内边距、表单分组间距 |
| `spacing-8` | 32px | 区块间距、弹窗内边距 |
| `spacing-12` | 48px | 页面区块间距 |
| `spacing-16` | 64px | 大屏页面顶部留白 |

### 4.3 页面布局

| 场景 | 规范 |
|------|------|
| PC 页面最大宽度 | 1440px |
| PC 内容区宽度 | 1200px（居中，左右各留 120px） |
| PC 侧边栏宽度 | 240px（收起态 64px） |
| 移动端（H5）内容区 | 100vw，内边距 16px |
| PC 栅格 | 12 列，列间距 24px |
| 移动端栅格 | 4 列，列间距 16px |

---

## 5. 圆角与阴影

### 5.1 圆角档位

| Token | 值 | 用途 |
|-------|----|------|
| `radius-sm` | 4px | 标签（Tag）、徽标（Badge）、小按钮 |
| `radius-md` | 8px | 输入框、普通按钮、卡片（默认） |
| `radius-lg` | 12px | 大卡片、面板、侧边栏 |
| `radius-xl` | 16px | 弹窗、底部抽屉（H5） |
| `radius-full` | 9999px | 圆形头像、开关（Switch）、胶囊按钮 |

### 5.2 阴影档位

| Token | 值 | 用途 |
|-------|----|------|
| `shadow-xs` | `0 1px 3px rgba(0,0,0,0.06)` | 卡片默认状态、悬浮工具条 |
| `shadow-sm` | `0 4px 12px rgba(0,0,0,0.08)` | 下拉菜单、Tooltip、悬浮卡片 |
| `shadow-md` | `0 8px 24px rgba(0,0,0,0.10)` | 模态弹窗、抽屉 |
| `shadow-lg` | `0 16px 48px rgba(0,0,0,0.12)` | 全屏弹窗、页面级遮罩层 |

> 阴影保持极淡，避免厚重感。禁止在同一层级叠加多层阴影。

---

## 6. 组件规范

> 组件库选型已完成，详见 `docs/architecture/component-library-selection.md`。

### 6.0 组件库选型

**PC 端选用 [tdesign-vue-next](https://tdesign.tencent.com/vue-next)**（腾讯 TDesign，Vue3 原生实现）。

**选型理由：**
- 企业级 B2B 视觉风格，与本规范的克制、专业定位吻合
- 完善的 CSS Variables 主题体系，可完整覆盖本文档 Token
- Vue3 原生、TypeScript 完善、长期维护

**主题管理：** `packages/ui`（`@skill/ui`）统一存放 TDesign CSS 变量覆盖，各应用按以下顺序引入：

```ts
// apps/[app-name]/src/main.ts
import 'tdesign-vue-next/es/style/index.css' // TDesign 基础样式
import '@skill/ui/src/index.css' // 主题覆盖（后置覆盖变量）
```

**与 UnoCSS 职责划分：**
- TDesign 负责所有 UI 组件
- UnoCSS 负责布局工具类（flex/grid/间距/响应式）
- `@skill/ui` 负责主题变量覆盖

### 6.1 按钮

| 类型 | 样式描述 |
|------|---------|
| Primary | 背景 `color-primary`，白色文字，Hover 变 `color-primary-dark` |
| Secondary | 白色背景，`color-primary` 边框与文字，Hover 背景 `color-primary-light` |
| Text | 无边框无背景，`color-primary` 文字，Hover 背景 `color-bg-hover` |
| Danger | 背景 `color-error`，白色文字 |
| Disabled | 背景 `color-border`，文字 `color-text-disabled`，禁止交互 |

- 标准高度：32px（sm）/ 36px（默认）/ 40px（lg）
- 内边距：水平 16px（默认）
- 圆角：`radius-md`（8px）

### 6.2 输入框与表单

- 输入框高度：36px（默认），H5 场景 44px
- 边框：1px solid `color-border`，圆角 `radius-md`
- Focus 态：边框色 `color-primary`，外发光 `0 0 0 3px rgba(67,97,238,0.15)`
- Error 态：边框色 `color-error`，错误提示文字 `color-error`，字号 12px
- 表单标签（Label）：字号 14px，字重 400，颜色 `color-text-primary`，下间距 6px
- 必填星号（\*）：颜色 `color-error`，位于 Label 之后

### 6.3 表格

- 表头背景：`color-bg-page`，字重 600，字号 14px
- 行高：48px（默认），密集模式 40px
- 行 Hover：背景 `color-bg-hover`
- 边框：仅水平分割线，1px solid `color-border`
- 操作列固定在右侧，超出内容区时出现横向滚动

### 6.4 导航与侧边栏

- 顶部导航高度：60px，背景白色，底部 1px `color-border` 分割
- 侧边栏宽度：240px（展开）/ 64px（收起）
- 激活菜单项：背景 `color-primary-light`，文字与图标 `color-primary`，左侧 3px `color-primary` 竖线
- 非激活菜单项：文字 `color-text-secondary`，Hover 背景 `color-bg-hover`

### 6.5 卡片

- 背景：白色，圆角 `radius-lg`，阴影 `shadow-xs`
- 内边距：24px（标准）/ 16px（紧凑）
- 卡片标题：H3 字号（20px），字重 400，颜色 `color-text-primary`
- 卡片分割线：1px solid `color-border`

---

## 7. 各应用差异说明

| 应用 | 特殊规范 |
|------|---------|
| **admin-web** | 信息密度较高，以表格为主要布局；使用紧凑型表格行高（40px）；侧边栏默认展开，优先显示导航层级 |
| **institution-web** | 数据看板风格，大量卡片+图表组合；数值文字可放大至 28~36px 配合 `color-primary` 高亮；图表配色基于品牌色延伸 |
| **assessee-web（PC）** | 答题区域居中布局，最大宽度 800px；侧边为题目导航；背景使用 `color-bg-page`；营造安静、专注的氛围；避免与答题无关的干扰元素 |
| **assessee-h5（移动）** | 全屏卡片式翻页；底部固定操作区（高度 72px）；正文字号上调至 15px；触摸目标最小尺寸 44×44px；圆角使用 `radius-xl`（16px）营造圆润感 |
| **portal-web** | 偏展示型，留白更多，`spacing-12`（48px）以上的区块间距；图文并茂；标题使用大字号（32px+）配合宽行高营造轻盈感；首屏建议全宽背景图或渐变色块 |

---

## 8. 交互规范

### 8.1 动效时长

| 场景 | 时长 |
|------|------|
| 微交互（按钮 Hover、颜色切换） | 100ms |
| 元素过渡（展开/收起、Tab 切换） | 200ms |
| 弹窗/抽屉出现 | 300ms |
| 页面级路由过渡 | 250ms |

### 8.2 缓动函数

- 进入动画：`ease-out`（快速出现，自然停止）
- 退出动画：`ease-in`（平滑消失）
- 状态切换：`ease-in-out`

### 8.3 反馈状态规范

**加载态**
- 数据请求中：使用骨架屏（Skeleton），保持与真实布局一致的占位结构
- 按钮操作中：按钮内显示 loading 图标，禁用按钮防止重复提交
- 加载超过 3 秒未完成：提示"加载中，请稍候…"

**空状态**
- 使用统一的空状态图示（图标 + 说明文字）
- 说明文字简洁，必要时提供操作引导（如"暂无数据，点击添加"）
- 空状态容器最小高度 200px，内容垂直居中

**错误状态**
- 网络错误/服务异常：展示错误图示 + 错误描述 + "重试"按钮
- 表单校验错误：红色边框 + 错误文字紧贴字段下方，避免弹出 Toast 打断输入流程
- 全局错误（如 403/404/500）：跳转对应错误页，提供返回首页入口

**操作成功**
- 轻量操作（如保存、复制）：顶部 Toast 提示，持续 2 秒自动消失
- 重要操作（如提交测评、删除记录）：弹窗二次确认，成功后 Toast 提示并刷新列表

---

## 9. 层级规范（z-index）

| Token | 值 | 用途 |
|-------|----|------|
| `z-dropdown` | 100 | 下拉菜单、Select 面板 |
| `z-sticky` | 200 | 固定表头、吸顶导航 |
| `z-fixed` | 300 | 固定侧边栏、顶部导航 |
| `z-overlay` | 400 | 弹窗遮罩层 |
| `z-modal` | 500 | 模态弹窗、抽屉 |
| `z-toast` | 600 | Toast 消息提示 |
| `z-tooltip` | 700 | Tooltip、气泡提示 |

- 禁止在业务组件中硬编码 z-index 数值，统一引用 Token
- 同层级组件若出现遮盖需求，在该档位基础上 ±1

---

## 附录：Token 快速索引

```
色彩：color-primary / color-primary-light / color-primary-dark
      color-success / color-warning / color-error / color-info
      color-text-primary / color-text-secondary / color-text-disabled
      color-border / color-bg-page / color-bg-card / color-bg-hover

字体：text-h1 ~ text-h4 / text-body-lg / text-body / text-body-sm / text-caption

间距：spacing-1(4) / spacing-2(8) / spacing-3(12) / spacing-4(16) / spacing-5(20)
      spacing-6(24) / spacing-8(32) / spacing-12(48) / spacing-16(64)

圆角：radius-sm(4) / radius-md(8) / radius-lg(12) / radius-xl(16) / radius-full

阴影：shadow-xs / shadow-sm / shadow-md / shadow-lg

层级：z-dropdown(100) / z-sticky(200) / z-fixed(300) / z-overlay(400)
      z-modal(500) / z-toast(600) / z-tooltip(700)
```
