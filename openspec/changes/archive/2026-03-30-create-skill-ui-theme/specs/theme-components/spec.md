## ADDED Requirements

### Requirement: CodeBlock component
主题包 SHALL 提供 CodeBlock 组件用于代码展示。

#### Scenario: CodeBlock with title
- **WHEN** 使用 `<CodeBlock title="示例">` 包裹代码
- **THEN** 组件 SHALL 在代码块上方显示标题
- **AND** 代码块使用 `--font-size-code` Token

#### Scenario: CodeBlock styling
- **WHEN** CodeBlock 渲染
- **THEN** 组件 SHALL 应用圆角（`--radius-md`）
- **AND** 支持暗色主题背景切换

### Requirement: Admonition component
主题包 SHALL 提供 Admonition 提示框组件。

#### Scenario: Admonition types
- **WHEN** 使用 `<Admonition type="info|warning|error|success">`
- **THEN** 组件 SHALL 显示对应语义色的提示框
- **AND** 显示对应图标

#### Scenario: Admonition with title
- **WHEN** 使用 `<Admonition type="warning" title="注意">`
- **THEN** 组件 SHALL 显示自定义标题

### Requirement: Badge component
主题包 SHALL 提供 Badge 标签组件。

#### Scenario: Badge with text
- **WHEN** 使用 `<Badge>标签</Badge>`
- **THEN** 组件 SHALL 显示内联标签
- **AND** 使用 `--color-primary-light` 背景
- **AND** 使用 `--color-primary` 文字色

#### Scenario: Badge with custom color
- **WHEN** 使用 `<Badge type="success">`
- **THEN** 组件 SHALL 使用语义色（success/warning/error/info）

### Requirement: QRCode component
主题包 SHALL 提供 QRCode 二维码组件。

#### Scenario: QRCode generation
- **WHEN** 使用 `<QRCode value="https://example.com" />`
- **THEN** 组件 SHALL 显示对应的二维码图片

#### Scenario: QRCode with size
- **WHEN** 使用 `<QRCode value="..." :size="200" />`
- **THEN** 组件 SHALL 按指定尺寸渲染二维码

### Requirement: Components use tokens
所有组件 SHALL 使用 Token 而非硬编码样式。

#### Scenario: Component responds to token override
- **WHEN** 项目覆盖了 Token
- **THEN** 所有组件 SHALL 响应新值

### Requirement: Component override mechanism
项目 SHALL 能够通过本地同名组件文件覆盖主题组件。

#### Scenario: Override component in project
- **WHEN** 项目在本地 `components/` 目录创建同名组件文件
- **THEN** 项目组件 SHALL 覆盖主题组件