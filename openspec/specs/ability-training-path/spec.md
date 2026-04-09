## ADDED Requirements

### Requirement: Ability training path defined for audience

演示文稿 SHALL 定义听众能力培养路线图，包含初级、中级、高级三个阶段。

#### Scenario: Three-level training path

- **WHEN** 演示文稿包含角色影响章节
- **THEN** SHALL 在章节结尾定义能力培养路线：
  - **初级**：理解工作流、会用工具完成单个任务
  - **中级**：能判断 AI 输出质量、能写出合格的 spec 文档
  - **高级**：能设计上下文策略、能开发团队专属 Skill

#### Scenario: Self-study guidance alignment

- **WHEN** 定义能力培养路线图
- **THEN** SHALL 与附录的自学指引内容对应，每个级别指向具体学习资源

### Requirement: Role transition summary after application

角色影响章节 SHALL 在工具应用章节之后，作为"方法落地后的影响总结"。

#### Scenario: Role chapter position

- **WHEN** 章节包含角色影响内容（PM/SDE/QA 影响）
- **THEN** SHALL 放置在工具应用章节之后，而非工作流章节之后

#### Scenario: Role chapter framing

- **WHEN** 角色影响章节开头
- **THEN** SHALL 明确说明"前面讲了各阶段怎么用，现在来看对你的影响"

### Requirement: Key ability highlighted for each role

每个角色 SHALL 有明确的能力培养重点。

#### Scenario: PM ability focus

- **WHEN** 定义 PM 能力培养
- **THEN** SHALL 强调：需求结构化能力、AI 推演结果审核能力

#### Scenario: SDE ability focus

- **WHEN** 定义 SDE 能力培养
- **THEN** SHALL 强调：上下文工程能力、AI 输出校准直觉、测试思维

#### Scenario: QA ability focus

- **WHEN** 定义 QA 能力培养
- **THEN** SHALL 强调：测试用例业务意义验证能力、边界情况识别能力