## ADDED Requirements

### Requirement: Light code highlighting theme
主题包 SHALL 提供亮色代码高亮主题。

#### Scenario: Light theme Prism variables
- **WHEN** HTML 没有 `.dark` 类
- **THEN** 代码块 SHALL 使用亮色高亮主题
- **AND** 高亮色基于品牌色系（蓝绿为主）
- **AND** 背景使用 `--color-bg-card` 或浅灰

### Requirement: Dark code highlighting theme
主题包 SHALL 提供暗色代码高亮主题。

#### Scenario: Dark theme Prism variables
- **WHEN** HTML 有 `.dark` 类
- **THEN** 代码块 SHALL 使用暗色高亮主题
- **AND** 高亮色保持足够对比度
- **AND** 背景使用深色

### Requirement: Code highlighting auto switch
代码高亮主题 SHALL 自动跟随 Slidev 主题切换。

#### Scenario: Theme auto switch
- **WHEN** 用户切换 Slidev 亮色/暗色模式
- **THEN** 代码高亮 SHALL 自动切换到对应主题

### Requirement: Code font family
代码块 SHALL 使用等宽字体。

#### Scenario: Monospace font
- **WHEN** 代码块渲染
- **THEN** 字体 SHALL 使用等宽字体栈
- **AND** 优先使用 JetBrains Mono 或 Fira Code（如可用）