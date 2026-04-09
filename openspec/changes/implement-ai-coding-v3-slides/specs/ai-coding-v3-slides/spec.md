## ADDED Requirements

### Requirement: Slide file structure follows numbering convention

幻灯片文件 SHALL 使用两位数字编号 + 主题描述的命名格式。

#### Scenario: Cover file naming

- **WHEN** 创建封面页文件
- **THEN** 文件名 SHALL 为 `01-cover.md`

#### Scenario: Chapter section file naming

- **WHEN** 创建章节分隔页
- **THEN** 文件名 SHALL 使用 `XX-chapterY-section.md` 格式

#### Scenario: Content file naming

- **WHEN** 创建普通内容页
- **THEN** 文件名 SHALL 使用 `XX-topic.md` 格式，其中 XX 为顺序编号

### Requirement: Slides entry file metadata completeness

slides.md 入口文件 SHALL 包含完整的元数据信息。

#### Scenario: Required metadata fields

- **WHEN** 创建或更新 slides.md
- **THEN** SHALL 包含以下元数据：
  - `id`: 演示文稿唯一标识
  - `title`: 演示标题
  - `created`: 创建日期
  - `updated`: 更新日期
  - `tags`: 标签数组
  - `slidesCount`: 幻灯片总数
  - `estimatedTime`: 预计时长
  - `status`: 状态（draft/published）

#### Scenario: Src references ordering

- **WHEN** slides.md 包含 src 引用
- **THEN** src 引用 SHALL 按幻灯片顺序排列，使用 `---` 分隔

### Requirement: Layout selection matches content type

幻灯片布局 SHALL 根据内容类型选择合适的 layout。

#### Scenario: Cover page layout

- **WHEN** 创建封面页
- **THEN** SHALL 使用 `layout: cover`

#### Scenario: Chapter section layout

- **WHEN** 创建章节分隔页
- **THEN** SHALL 使用 `layout: Section`

#### Scenario: Two-column content layout

- **WHEN** 内容适合双栏展示（如表格+代码）
- **THEN** SHALL 使用 `layout: TwoCols`