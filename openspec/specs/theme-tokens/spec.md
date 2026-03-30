## ADDED Requirements

### Requirement: Color tokens defined
主题包 SHALL 定义完整的色彩 Token 系统，包括品牌色、语义色、中性色。

#### Scenario: Brand colors available
- **WHEN** 主题被加载
- **THEN** CSS 变量 `--color-primary`、`--color-primary-light`、`--color-primary-dark` SHALL 可用
- **AND** 默认值分别为 `#4361EE`、`#EEF1FD`、`#2D4BC7`

#### Scenario: Semantic colors available
- **WHEN** 主题被加载
- **THEN** CSS 变量 `--color-success`、`--color-warning`、`--color-error`、`--color-info` SHALL 可用
- **AND** 默认值符合 ui-design-spec 语义色定义

#### Scenario: Neutral colors available
- **WHEN** 主题被加载
- **THEN** CSS 变量 `--color-text-primary`、`--color-text-secondary`、`--color-bg-page`、`--color-bg-card`、`--color-border` SHALL 可用

### Requirement: Font size tokens defined
主题包 SHALL 定义幻灯片场景的字号 Token 系统。

#### Scenario: Cover font sizes
- **WHEN** 主题被加载
- **THEN** CSS 变量 `--font-size-cover-title`（64px）、`--font-size-cover-subtitle`（28px）、`--font-size-cover-meta`（16px）SHALL 可用

#### Scenario: Page font sizes
- **WHEN** 主题被加载
- **THEN** CSS 变量 `--font-size-page-title`（40px）、`--font-size-section-title`（48px）、`--font-size-heading`（32px）SHALL 可用

#### Scenario: Body font sizes
- **WHEN** 主题被加载
- **THEN** CSS 变量 `--font-size-body`（24px）、`--font-size-body-sm`（18px）、`--font-size-caption`（14px）SHALL 可用

#### Scenario: Code font size
- **WHEN** 主题被加载
- **THEN** CSS 变量 `--font-size-code`（18px）SHALL 可用

### Requirement: Spacing tokens defined
主题包 SHALL 定义基于 4px 基础单位的间距 Token。

#### Scenario: Spacing scale available
- **WHEN** 主题被加载
- **THEN** CSS 变量 `--spacing-xs`（4px）、`--spacing-sm`（8px）、`--spacing-md`（16px）、`--spacing-lg`（24px）、`--spacing-xl`（32px）、`--spacing-2xl`（48px）SHALL 可用

### Requirement: Border radius tokens defined
主题包 SHALL 定义圆角 Token。

#### Scenario: Radius scale available
- **WHEN** 主题被加载
- **THEN** CSS 变量 `--radius-sm`（4px）、`--radius-md`（8px）、`--radius-lg`（12px）、`--radius-xl`（16px）SHALL 可用

### Requirement: Shadow tokens defined
主题包 SHALL 定义阴影 Token。

#### Scenario: Shadow scale available
- **WHEN** 主题被加载
- **THEN** CSS 变量 `--shadow-xs`、`--shadow-sm`、`--shadow-md` SHALL 可用
- **AND** 阴影值符合 ui-design-spec 定义（极淡风格）

### Requirement: Dark theme tokens
主题包 SHALL 提供暗色主题 Token 变体。

#### Scenario: Dark mode color override
- **WHEN** HTML 元素有 `.dark` 类
- **THEN** 中性色 Token SHALL 自动切换为暗色值
- **AND** `--color-text-primary` 变为 `#F7FAFC`
- **AND** `--color-bg-page` 变为 `#1A1A2E`
- **AND** 品牌色 Token 保持不变

### Requirement: Token override mechanism
项目 SHALL 能够通过 CSS 变量覆盖主题 Token。

#### Scenario: Override token in project CSS
- **WHEN** 项目在主题加载后定义 CSS 变量
- **THEN** 项目定义的值 SHALL 覆盖主题默认值
- **AND** 所有使用该 Token 的布局和组件 SHALL 响应新值