## ADDED Requirements

### Requirement: Cover layout
主题包 SHALL 提供 Cover 布局用于封面页。

#### Scenario: Cover layout structure
- **WHEN** 使用 `layout: cover`
- **THEN** 布局 SHALL 提供标题、副标题、页脚区域
- **AND** 标题使用 `--font-size-cover-title` Token
- **AND** 内容垂直居中

### Requirement: Default layout
主题包 SHALL 提供 Default 布局作为默认正文页。

#### Scenario: Default layout structure
- **WHEN** 未指定布局或使用 `layout: default`
- **THEN** 布局 SHALL 提供页面标题和内容区域
- **AND** 标题使用 `--font-size-page-title` Token
- **AND** 内容区域有适当内边距

### Requirement: Section layout
主题包 SHALL 提供 Section 布局用于章节分隔页。

#### Scenario: Section layout structure
- **WHEN** 使用 `layout: section`
- **THEN** 布局 SHALL 提供居中的大标题
- **AND** 标题使用 `--font-size-section-title` Token
- **AND** 内容垂直水平居中

### Requirement: TopTitle layout
主题包 SHALL 提供 TopTitle 布局，标题在顶部。

#### Scenario: TopTitle layout structure
- **WHEN** 使用 `layout: top-title`
- **THEN** 布局 SHALL 在顶部显示标题
- **AND** 标题下方为内容区域
- **AND** 标题使用 `--font-size-page-title` Token

### Requirement: SideTitle layout
主题包 SHALL 提供 SideTitle 布局，标题在左侧。

#### Scenario: SideTitle layout structure
- **WHEN** 使用 `layout: side-title`
- **THEN** 布局 SHALL 在左侧显示标题
- **AND** 右侧为内容区域
- **AND** 标题使用 `--font-size-heading` Token

### Requirement: TwoCols layout
主题包 SHALL 提供 TwoCols 双列布局。

#### Scenario: TwoCols layout structure
- **WHEN** 使用 `layout: two-cols`
- **THEN** 布局 SHALL 提供左右两个等宽区域
- **AND** 支持 `::left::` 和 `::right::` slot

### Requirement: TopTitleTwoCols layout
主题包 SHALL 提供 TopTitleTwoCols 布局，顶部标题加双列内容。

#### Scenario: TopTitleTwoCols layout structure
- **WHEN** 使用 `layout: top-title-two-cols`
- **THEN** 布局 SHALL 在顶部显示标题
- **AND** 标题下方为左右两个等宽内容区域
- **AND** 支持 `::left::` 和 `::right::` slot

### Requirement: Full layout
主题包 SHALL 提供 Full 布局用于全屏内容。

#### Scenario: Full layout structure
- **WHEN** 使用 `layout: full`
- **THEN** 内容 SHALL 占满整个幻灯片区域
- **AND** 无默认内边距

### Requirement: Quote layout
主题包 SHALL 提供 Quote 布局用于引用页。

#### Scenario: Quote layout structure
- **WHEN** 使用 `layout: quote`
- **THEN** 布局 SHALL 提供引用文字和来源区域
- **AND** 引用文字有特殊样式（如左侧边框、斜体）

### Requirement: Credits layout
主题包 SHALL 提供 Credits 布局用于结束页。

#### Scenario: Credits layout structure
- **WHEN** 使用 `layout: credits`
- **THEN** 布局 SHALL 提供感谢语和联系方式区域
- **AND** 内容垂直居中

### Requirement: Layouts use tokens
所有布局 SHALL 使用 Token 而非硬编码样式。

#### Scenario: Layout responds to token override
- **WHEN** 项目覆盖了 Token（如 `--color-primary`）
- **THEN** 所有布局 SHALL 响应新值
- **AND** 无硬编码的颜色、字号、间距值

### Requirement: Layout override mechanism
项目 SHALL 能够通过本地同名布局文件覆盖主题布局。

#### Scenario: Override layout in project
- **WHEN** 项目在本地 `layouts/` 目录创建同名布局文件（如 `Cover.vue`）
- **THEN** 项目布局 SHALL 覆盖主题布局