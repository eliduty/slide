## ADDED Requirements

### Requirement: Slide numbering consistency

演示文稿结构变更时 SHALL 保持文件编号与引用顺序一致。

#### Scenario: Renumber on reorder

- **WHEN** 调整幻灯片顺序
- **THEN** SHALL 重新编号所有受影响的文件，使编号反映新的顺序位置

#### Scenario: Update slides.md references

- **WHEN** 幻灯片文件重命名
- **THEN** slides.md 入口文件中的 src 引用 SHALL 同步更新为新文件名

### Requirement: Environment stage has dedicated page

四阶段工作流中，每个阶段 SHALL 在应用章节有对应的独立页面。

#### Scenario: Four stages coverage

- **WHEN** 工作流定义为四个阶段（需求、设计、环境规范、实现）
- **THEN** 应用章节 SHALL 包含四个对应的页面，分别讲解每个阶段的具体应用

#### Scenario: Environment stage page content

- **WHEN** 环境规范阶段应用页面
- **THEN** SHALL 包含：
  - 开发环境配置（CLAUDE.md + rules）
  - 测试环境准备（测试策略 + mock 数据）
  - 领域知识文档准备
  - 验证 AI 理解的方法

### Requirement: Summary page includes action call

演示文稿结尾 SHALL 包含明确的行动号召，指导听众下一步做什么。

#### Scenario: Action call in summary

- **WHEN** 演示文稿包含总结页面
- **THEN** SHALL 包含明确的行动建议：
  - "本周内用 AI 完成一个小任务"
  - 或"遇到问题，来看这些资产"

#### Scenario: Timeframe for action

- **WHEN** 定义行动号召
- **THEN** SHALL 包含明确的时间框架（如"本周内"、"两周内")