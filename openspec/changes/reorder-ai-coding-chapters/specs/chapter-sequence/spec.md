## ADDED Requirements

### Requirement: Chapter sequence defines narrative flow

演示文稿的章节顺序 SHALL 遵循"认知 → 方法 → 应用 → 影响 → 场景"的叙事逻辑链条。

#### Scenario: Standard chapter order

- **WHEN** 创建或调整演示文稿章节顺序
- **THEN** 章节 SHALL 按以下顺序组织：
  1. 能力认知（AI 能做什么、局限是什么）
  2. 标准方法（工作流、边界定义）
  3. 工具应用（各阶段具体怎么用）
  4. 角色影响（对 PM/SDE/QA 的影响、能力培养）
  5. 场景实操（遗留项目、新项目、日常迭代）
  6. 资产交付（标准化资产、自学指引）

#### Scenario: Method to application direct衔接

- **WHEN** 定义工作流相关内容
- **THEN** 工作流方法 SHALL 直接承接应用讲解，中间不插入其他主题章节

### Requirement: Slide file numbering matches sequence

幻灯片文件编号 SHALL 与其在演示顺序中的位置一致。

#### Scenario: Number increases with position

- **WHEN** 幻灯片文件命名为 `XX-topic.md`
- **THEN** `XX` SHALL 反映该幻灯片在 slides.md 引用顺序中的位置（01 为封面，按顺序递增）

#### Scenario: Chapter indicator in filename

- **WHEN** 幻灯片属于特定章节
- **THEN** 文件名 SHALL 包含章节号标识（如 `chapter3-section.md` 表示第3章章节页）

### Requirement: Chapter transitions have explicit statements

章节之间 SHALL 有明确的过渡语句，说明"上一章讲了什么，这章讲什么"。

#### Scenario: Chapter opening transition

- **WHEN** 进入新章节的章节页
- **THEN** speaker notes SHALL 包含过渡语句：
  - "上一章我们讲了 X，这章我们来看 Y"
  - 或"前面讲了 X，现在来看对你的影响"

#### Scenario: Method to application transition

- **WHEN** 工作流章节结束后进入应用章节
- **THEN** 应用章节开头 SHALL 明确承接：
  - "上一章我们讲了四阶段工作流，这章我们来看每个阶段具体怎么用 AI"