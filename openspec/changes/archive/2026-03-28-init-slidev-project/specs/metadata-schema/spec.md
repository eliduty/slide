## ADDED Requirements

### Requirement: Presentation metadata in slides.md frontmatter
每个演示的 `slides.md` SHALL 在 YAML frontmatter 中包含演示级元数据。

#### Scenario: Read presentation metadata
- **WHEN** 打开 `presentations/<id>/slides.md`
- **THEN** SHALL 在文件开头的 frontmatter 看到 `id`、`title`、`created`、`updated`、`status` 等元数据字段

### Requirement: Required metadata fields
slides.md frontmatter SHALL 包含以下必需字段：
- `theme`: 共享主题路径
- `title`: 演示标题
- `id`: 演示唯一标识（与目录名一致）
- `created`: 创建日期
- `updated`: 最后更新日期
- `status`: 状态（draft / reviewing / ready / published）

#### Scenario: Validate required fields
- **WHEN** 创建新的 slides.md
- **THEN** SHALL 包含所有必需元数据字段

### Requirement: Optional metadata fields
slides.md frontmatter MAY 包含以下可选字段：
- `author`: 作者名称
- `aspectRatio`: 宽高比（默认 16/9）
- `colorSchema`: 颜色模式（auto / light / dark）
- `tags`: 标签列表
- `slidesCount`: 总页数
- `estimatedTime`: 预计时长

#### Scenario: Add optional metadata
- **WHEN** 需要更详细的演示信息
- **THEN** MAY 在 frontmatter 添加可选字段

### Requirement: Slide-level metadata in split files
`slides/` 目录下的每个拆分文件 MAY 在 frontmatter 包含页级元数据。

#### Scenario: Add slide metadata
- **WHEN** 为某页幻灯片添加元数据
- **THEN** MAY 在文件开头添加 `title`、`order`、`duration`、`keyPoints` 等字段

### Requirement: Slide content split using src
slides.md SHALL 使用 `src: ./slides/<filename>.md` 引用拆分的内容文件。

#### Scenario: Split slides into multiple files
- **WHEN** 演示内容较多需要拆分
- **THEN** slides.md SHALL 使用 `---` 分隔，每个分隔块使用 `src:` 引用外部文件