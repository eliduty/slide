# 研发 AI Coding 培训大纲分析报告

> 基于 skill 项目实践的培训大纲优化建议

---

## 一、大纲整体评价

这是一份**结构完整、层次清晰**的 AI Coding 培训大纲，从工作流理念到具体实操场景都有覆盖。大纲的三个核心章节形成了递进关系：

```
第1章：建立认知框架（为什么这样工作）
    ↓
第2章：工具应用方法（如何使用工具）
    ↓
第3章：场景化实操（遇到问题怎么办）
```

---

## 二、与 skill 项目的结合点

skill 项目已经建立了**成熟的 AI Coding 工作流实践**，可以作为培训的**最佳实践案例**。以下是具体对应关系：

### 2.1 大纲 1.2 "基于 AI Coding 工具能力推导的工作流" → 项目中的 OpenSpec + Superpowers 工作流

| 大纲要求 | 项目实践 |
|---------|---------|
| 需求阶段 5W1H | `/opsx:explore` 探索需求 |
| 技术设计阶段 | `/opsx:propose` 生成 proposal + design + tasks |
| 规范 AI 工作环境 | `CLAUDE.md` + `.claude/rules/` + Skills 体系 |

**建议**：将 `docs/guides/openspec-superpowers-workflow.md` 作为培训的**标准工作流模板**，这正是大纲要求的"像素级模仿"范本。

### 2.2 大纲 1.4 "人的工作调整" → 项目中的 Skills 体系

大纲提到的能力转变，在项目中已有对应实现：

| 大纲要求 | 项目实现 |
|---------|---------|
| "建立规则和标准" | `.claude/rules/` 目录下的 12+ 规范文件 |
| "上下文工程" | `writing-plans` skill 的渐进式上下文披露 |
| "问题分拆：架构能力" | `brainstorming` skill + `writing-plans` skill |
| "对 AI 输出的校准直觉" | `systematic-debugging` skill 的防御性思维 |

### 2.3 大纲 2.2 "设计阶段" → 项目中的 spec-driven 开发

项目的 `openspec/specs/` 目录已有 **40+ 个技术规范**，涵盖：
- 实体设计（`base-entity`、`soft-deletable-entity`）
- 组件设计（`role-card-component`、`base-dialog`）
- 架构决策（`multi-tenant-development`、`api-security`）

这正是大纲要求的"接口契约设计"、"架构设计与项目结构治理"的落地实践。

### 2.4 大纲 3.2 "新项目启动" → 项目的脚手架体系

项目已建立的标准化资产：

| 大纲场景 | 项目资产 |
|---------|---------|
| 项目脚手架生成 | Monorepo 架构 + pnpm workspace |
| 上下文工程初始化 | `CLAUDE.md` 层级规则 + Skills 锁定 |
| 测试策略前置 | E2E 测试基础设施 + Playwright 配置 |

---

## 三、大纲可改进之处

### 3.1 缺少"AI Coding 工具链选型"章节

建议在第一章增加：

```markdown
### 1.5 AI Coding 工具链选型

- IDE 集成：Trae / Cursor / Windsurf / Claude Code
- 规则引擎：CLAUDE.md / .cursorrules / .windsurfrules
- 工作流编排：OpenSpec / Superpowers / MCP
- 版本控制联动：分支策略 + AI commit 规范
```

### 3.2 第 2 章缺少"代码评审"的详细操作

大纲 2.4 提到"设计与实现的评价评审"，但没有展开。项目中有 `requesting-code-review` skill 可以作为案例：

```markdown
### 2.5 代码评审阶段

AI 工具应用于：
1. 自动化代码风格检查
2. 安全漏洞扫描
3. 测试覆盖率验证
4. 变更影响分析
```

### 3.3 第 3 章场景可以更具体

当前场景描述偏理论，建议增加**可执行的步骤清单**。例如"场景1：上下文窗口爆炸"可以改为：

```markdown
**场景1：上下文窗口爆炸**

**症状识别**：AI 响应变慢、输出截断、上下文超限错误

**操作步骤**：
1. 执行 `openspec status` 查看当前上下文大小
2. 使用分层摘要策略：
   - 项目级：README.md + CLAUDE.md
   - 模块级：apps/*/CLAUDE.md
   - 文件级：关键文件头注释
3. 建立精简架构描述文档作为"基座上下文"
4. 利用目录树 + 关键文件组合代替全量代码

**验收标准**：上下文控制在合理 tokens 以内，AI 能正确回答模块边界问题
```

---

## 四、结合项目实践的具体建议

### 4.1 将项目作为"标准化资产清单"的范例

大纲末尾建议的"附录：标准化资产清单"，项目已经具备：

| 资产类型 | 项目文件 | 可复用程度 |
|---------|---------|-----------|
| 需求模板 | `docs/requirements/prd-*.md` | ⭐⭐⭐⭐⭐ |
| 设计文档模板 | `openspec/specs/*/spec.md` | ⭐⭐⭐⭐⭐ |
| AI 规则文件模板 | `CLAUDE.md` 层级结构 | ⭐⭐⭐⭐⭐ |
| Prompt 库 | `docs/prompts/*.md` | ⭐⭐⭐⭐ |
| Review Checklist | `.claude/rules/*` | ⭐⭐⭐⭐⭐ |
| Skills 库 | `.agents/skills/*/SKILL.md` | ⭐⭐⭐⭐⭐ |

### 4.2 增加"Skills 开发"培训模块

项目有完整的 `skill-creator` skill，可以增加：

```markdown
## 4. Skills 开发与团队知识沉淀

### 4.1 什么是 Skill
- Skill 的本质：可复用的 AI 协作模式
- 与传统文档的区别：可执行性 + 上下文感知

### 4.2 Skill 开发流程
1. 捕获意图：从重复工作中提取模式
2. 编写 SKILL.md：YAML frontmatter + Markdown 指令
3. 测试验证：创建测试 prompt 验证效果
4. 迭代优化：基于反馈持续改进

### 4.3 团队知识沉淀
- 将团队最佳实践固化为 Skills
- 建立 Skills 版本控制和评审机制
- Skills 继承与组合模式
```

### 4.3 补充"多 Agent 协作"场景

项目中的 `subagent-driven-development` skill 展示了多 Agent 协作模式，建议增加：

```markdown
### 3.3 复杂任务的分解与并行执行

**场景：多个独立任务并行开发**

**操作要点**：
1. 使用 `/opsx:propose` 生成细粒度任务列表
2. 识别任务间的依赖关系
3. 将独立任务分配给不同的 Agent 并行执行
4. 汇总结果并进行集成测试

**项目案例**：`subagent-driven-development` skill
```

---

## 五、培训产出物建议

基于项目实践，建议培训后每个团队持有的标准化资产：

```
team-ai-coding-toolkit/
├── CLAUDE.md                    # 项目级规则（从模板定制）
├── .claude/
│   ├── rules/                   # 开发规范（从 12+ 规范选择）
│   ├── commands/                # 自定义命令（opsx 工作流）
│   └── skills/                  # 团队专属 Skills
├── docs/
│   ├── templates/
│   │   ├── prd-template.md      # 需求文档模板
│   │   ├── spec-template.md     # 技术规范模板
│   │   └── design-template.md   # 设计文档模板
│   └── prompts/                 # 常用 Prompt 库
└── openspec/
    └── specs/                   # 已沉淀的技术规范
```

---

## 六、总结

这份培训大纲**框架完整、思路清晰**，与 skill 项目实践高度契合。主要建议：

1. **增加工具链选型章节**，帮助团队建立统一的技术栈
2. **细化场景操作步骤**，从"知道做什么"到"知道怎么做"
3. **以项目为案例**，展示"像素级模仿"的标准范本
4. **补充 Skills 开发模块**，实现团队知识的可持续沉淀

项目本身就是 AI Coding 工作流的**最佳实践案例**，建议将项目中的工作流文档、规范文件、Skills 体系作为培训的核心教材。

---

## 附录：项目关键文件索引

### 工作流文档
- `docs/guides/openspec-superpowers-workflow.md` - 标准四阶段工作流
- `.claude/commands/opsx/apply.md` - 任务实现流程
- `.agents/skills/writing-plans/SKILL.md` - 计划编写规范

### 规则文件
- `CLAUDE.md` - 项目级规则入口
- `.claude/rules/` - 开发规范目录（12+ 规范文件）

### Skills 体系
- `.agents/skills/skill-creator/SKILL.md` - Skill 开发指南
- `.agents/skills/systematic-debugging/SKILL.md` - 系统化调试
- `.agents/skills/writing-plans/SKILL.md` - 计划编写

### 模板文件
- `docs/requirements/prd-*.md` - 需求文档模板
- `openspec/specs/*/spec.md` - 技术规范模板
- `docs/prompts/*.md` - Prompt 模板库
