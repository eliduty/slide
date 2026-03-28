## ADDED Requirements

### Requirement: Workspace directory exists
每个演示 SHALL 包含 `workspace/` 目录用于管理素材和工作文件，与最终产出分离。

#### Scenario: Locate workspace for presentation
- **WHEN** 查看 `presentations/<presentation-id>/` 目录
- **THEN** SHALL 存在 `workspace/` 子目录

### Requirement: Research notes file
workspace/ 目录 SHALL 包含 `research.md` 文件用于记录调研笔记。

#### Scenario: Document research findings
- **WHEN** 准备演示内容，进行知识搜集
- **THEN** 可在 `workspace/research.md` 记录来源链接和要点

### Requirement: Outline file
workspace/ 目录 SHALL 包含 `outline.md` 文件用于演示结构规划。

#### Scenario: Plan presentation structure
- **WHEN** 规划演示的章节结构
- **THEN** 可在 `workspace/outline.md` 记录大纲，对应 slides/ 文件映射

### Requirement: References file
workspace/ 目录 SHALL 包含 `references.md` 文件用于参考资料列表。

#### Scenario: Track reference materials
- **WHEN** 收集演示所需参考资料
- **THEN** 可在 `workspace/references.md` 记录文章、书籍、视频链接

### Requirement: Scripts directory for speaker notes
workspace/ 目录 SHALL 包含 `scripts/` 目录用于演讲脚本（逐字稿）。

#### Scenario: Create speaker script for slide
- **WHEN** 为某页幻灯片准备演讲脚本
- **THEN** 可在 `workspace/scripts/` 创建对应文件（命名与 slides/ 文件对应）

### Requirement: Data directory for source files
workspace/ 目录 SHALL 包含 `data/` 目录用于数据源文件。

#### Scenario: Store chart data
- **WHEN** 幻灯片需要图表展示
- **THEN** 原始数据文件（CSV、JSON 等）SHALL 存放在 `workspace/data/`

### Requirement: Drafts directory for raw files
workspace/ 目录 SHALL 包含 `drafts/` 目录用于原始草稿文件。

#### Scenario: Store Excalidraw source
- **WHEN** 使用 Excalidraw 创建图表
- **THEN** 源文件 SHALL 存放在 `workspace/drafts/`，处理后导出到 public/

### Requirement: Feedback file
workspace/ 目录 SHALL 包含 `feedback.md` 文件用于观众反馈记录。

#### Scenario: Record audience feedback
- **WHEN** 演示后收到观众反馈
- **THEN** 可在 `workspace/feedback.md` 记录反馈内容和处理状态

### Requirement: Public directory for final assets
每个演示 SHALL 包含 `public/` 目录用于存放最终资源，打包进演示。

#### Scenario: Use processed images in slides
- **WHEN** 幻灯片需要展示图片
- **THEN** 图片 SHALL 存放在 `public/images/`，通过相对路径引用

### Requirement: Archive directory for version history
每个演示 SHALL 包含 `archive/` 目录用于版本归档。

#### Scenario: Archive previous version
- **WHEN** 需要保存演示的旧版本
- **THEN** SHALL 在 `archive/<date>/` 创建按日期命名的归档目录