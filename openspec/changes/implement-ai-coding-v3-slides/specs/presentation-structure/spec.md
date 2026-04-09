## ADDED Requirements

### Requirement: Part structure extends to eight sections

演示文稿结构 SHALL 支持最多 8 个部分（Part 0-8）的组织方式。

#### Scenario: Part numbering

- **WHEN** 组织演示文稿内容
- **THEN** SHALL 可使用 Part 0 到 Part 8 的编号方式，其中 Part 0 为开场部分

#### Scenario: Part to chapter mapping

- **WHEN** 使用 Part 组织方式
- **THEN** 每个 Part SHALL 对应一个主题章节，包含章节页和内容页

### Requirement: Content reuse between versions

演示文稿版本之间 SHALL 支持内容文件的复用和编号调整。

#### Scenario: Reuse from previous version

- **WHEN** 新版本需要复用旧版本内容
- **THEN** SHALL 可复制旧版本文件并重新编号以衔接新结构

#### Scenario: Numbering adjustment

- **WHEN** 复用文件需要调整编号
- **THEN** SHALL 修改文件名编号和 slides.md 中的 src 引用顺序