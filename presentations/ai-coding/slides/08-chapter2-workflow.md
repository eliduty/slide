---
layout: Default
---

# 2.1 标准工作流四阶段

<div class="workflow-flow">

<div class="stage">
<div class="stage-header">
<span class="stage-num">01</span>
<span class="stage-title">需求阶段</span>
</div>
<div class="stage-body">
<div><strong>参与：</strong>PM + SDE</div>
<div><strong>产出：</strong>PRD 文档</div>
<div><strong>条件：</strong>需求评审通过</div>
</div>
</div>

<div class="arrow">→</div>

<div class="stage">
<div class="stage-header">
<span class="stage-num">02</span>
<span class="stage-title">技术设计</span>
</div>
<div class="stage-body">
<div><strong>参与：</strong>SDE主导 + PM</div>
<div><strong>产出：</strong>proposal + design + tasks</div>
<div><strong>条件：</strong>技术评审通过</div>
</div>
</div>

<div class="arrow">→</div>

<div class="stage">
<div class="stage-header">
<span class="stage-num">03</span>
<span class="stage-title">环境规范</span>
</div>
<div class="stage-body">
<div><strong>参与：</strong>SDE</div>
<div><strong>产出：</strong>规则 + 测试 + 领域知识</div>
<div><strong>条件：</strong>AI能正确理解上下文</div>
</div>
</div>

<div class="arrow">→</div>

<div class="stage">
<div class="stage-header">
<span class="stage-num">04</span>
<span class="stage-title">实现阶段</span>
</div>
<div class="stage-body">
<div><strong>参与：</strong>SDE</div>
<div><strong>产出：</strong>代码 + 测试 + 文档</div>
<div><strong>条件：</strong>lint通过、测试覆盖达标</div>
</div>
</div>

</div>

<div class="highlight">
每个阶段用 5W1H 定义：谁参与、做什么、标准、产出、如何做、用时多少
</div>

<style>
.workflow-flow {
  display: flex;
  align-items: stretch;
  gap: var(--spacing-xs);
  margin-top: var(--spacing-md);
}
.stage {
  flex: 1;
  border-radius: var(--radius-md);
  padding: var(--spacing-sm);
  display: flex;
  flex-direction: column;
}
.stage:nth-child(1) { background: var(--color-success-light); border: 1px solid var(--color-success); }
.stage:nth-child(3) { background: var(--color-info-light); border: 1px solid var(--color-info); }
.stage:nth-child(5) { background: var(--color-accent-teal-light); border: 1px solid var(--color-accent-teal); }
.stage:nth-child(7) { background: var(--color-warning-light); border: 1px solid var(--color-warning); }
.stage-header {
  display: flex;
  align-items: center;
  gap: var(--spacing-xs);
  margin-bottom: var(--spacing-xs);
}
.stage-num {
  font-family: var(--font-family-display);
  width: 24px;
  height: 24px;
  border-radius: var(--radius-sm);
  display: flex;
  align-items: center;
  justify-content: center;
  font-weight: var(--font-weight-semibold);
  font-size: 12px;
}
.stage:nth-child(1) .stage-num { background: var(--color-success); color: var(--color-bg-card); }
.stage:nth-child(3) .stage-num { background: var(--color-info); color: var(--color-bg-card); }
.stage:nth-child(5) .stage-num { background: var(--color-accent-teal); color: var(--color-bg-card); }
.stage:nth-child(7) .stage-num { background: var(--color-warning); color: var(--color-bg-card); }
.stage-title {
  font-family: var(--font-family-display);
  font-weight: var(--font-weight-medium);
  font-size: var(--font-size-card-title);
  color: var(--color-text-primary);
}
.stage-body { font-size: var(--font-size-card-meta); color: var(--color-text-primary); }
.stage-body div { margin-bottom: 2px; }
.stage-body strong { color: var(--color-primary); }
.arrow {
  font-size: var(--font-size-heading);
  color: var(--color-text-muted);
  padding-top: var(--spacing-sm);
}
.highlight {
  margin-top: var(--spacing-lg);
  padding: var(--spacing-md);
  background: var(--color-accent-orange-light);
  border-radius: var(--radius-md);
  border: 1px solid var(--color-accent-orange);
  font-size: var(--font-size-card-body);
  text-align: center;
  color: var(--color-text-primary);
}
</style>

<!--
工作流分为四个大阶段：**需求阶段、技术设计阶段、环境规范阶段、实现阶段**。

每个阶段我们都用 5W1H 来定义：谁参与、做什么事情、达到什么标准、产出哪些东西、如何做、使用多少时间。

**需求阶段**

- **谁参与**：PM + SDE
- **做什么**：结构化需求描述
- **标准**：业务边界明确、验收标准清晰
- **产出物**：PRD 文档
- **进入下一阶段的条件**：需求评审通过

这个阶段，AI 的作用是"需求推演完善"和"结构化描述"。但业务目标定义、验收标准确定，这些必须由人来完成。

**技术设计阶段**

- **谁参与**：SDE 主导，PM 参与
- **做什么**：技术方案、接口契约、测试策略
- **标准**：技术选型确定、架构边界清晰
- **产出物**：proposal.md + design.md + tasks.md 三件套
- **进入下一阶段的条件**：技术评审通过

这个阶段，AI 负责"技术方案生成"、"接口契约设计"。但"技术选型决策"、"架构边界定义"，必须由人来拍板。

**环境规范阶段**

- **谁参与**：SDE
- **做什么**：配置 AI 工作环境、准备测试基础设施、规范化领域知识
- **标准**：AI 能正确理解项目的技术约束和业务语义
- **产出物**：CLAUDE.md + rules + 测试框架 + 领域知识文档
- **进入下一阶段的条件**：AI 能正确理解上下文

这是新增的阶段，很多人会忽略。但我要强调：**没有准备好环境，就开始写代码，AI 就会乱猜。**这个阶段就是把上下文准备好，让 AI 在后续实现阶段有足够的背景。

**实现阶段**

- **谁参与**：SDE
- **做什么**：开发、测试、联动调试
- **标准**：lint 通过、测试覆盖达标
- **产出物**：代码 + 测试 + 文档
- **进入下一阶段的条件**：lint 通过、测试覆盖达标

这个阶段，AI 根据"规范"来生成代码、测试。但验证输出质量、处理边界情况，必须由人来把关。

**记住：四个阶段，顺序不能乱。跳过环境规范阶段，直接进入实现，是最常见的错误。**
-->