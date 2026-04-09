---
layout: TwoCols
---

::left::

# 方法论演进：从 Prompt 到 Harness

<div class="evolution-stack">

<div class="evo-item">
<div class="evo-level">Level 1</div>
<div class="evo-name">Prompt Engineering</div>
<div class="evo-desc">提示词工程</div>
<div class="evo-focus">关注"如何写更好的指令"</div>
<div class="evo-issue">问题：上下文不足仍会失败</div>
</div>

<div class="evo-item">
<div class="evo-level">Level 2</div>
<div class="evo-name">Context Engineering</div>
<div class="evo-desc">上下文工程</div>
<div class="evo-focus">关注"如何筛选精准上下文"</div>
<div class="evo-issue">问题：管理依赖人工，难以复用</div>
</div>

<div class="evo-item highlight">
<div class="evo-level">Level 3</div>
<div class="evo-name">Harness Engineering</div>
<div class="evo-desc">编排工程</div>
<div class="evo-focus">关注"如何工程化约束 AI"</div>
<div class="evo-result">结果：模板+规则+工作流可复用体系</div>
</div>

</div>

::right::

<div class="goal-box">
<div class="goal-title">本次分享的核心</div>
<div class="goal-desc">给你一套完整的 Harness——让 AI 在规范约束下执行任务，输出可预测、可追溯、可验证</div>
</div>

<div class="harness-components">
<strong>Harness 包含：</strong>
<ul>
<li>模板：PRD、design、tasks 等标准化文档</li>
<li>规则：CLAUDE.md + rules 约束文件</li>
<li>工作流：propose → explore → apply → archive</li>
</ul>
</div>

<style>
.evolution-stack {
  display: flex;
  flex-direction: column;
  gap: var(--spacing-sm);
}
.evo-item {
  padding: var(--spacing-sm);
  border-radius: var(--radius-md);
  border: 1px solid var(--color-border);
}
.evo-item:nth-child(1) { background: var(--color-bg-subtle); }
.evo-item:nth-child(2) { background: var(--color-info-light); }
.evo-item:nth-child(3) { background: var(--color-success-light); border-color: var(--color-success); }
.evo-level {
  font-family: var(--font-family-display);
  font-weight: var(--font-weight-semibold);
  font-size: var(--font-size-card-meta);
  color: var(--color-text-muted);
}
.evo-name {
  font-family: var(--font-family-display);
  font-weight: var(--font-weight-medium);
  font-size: var(--font-size-card-title);
  color: var(--color-text-primary);
}
.evo-desc {
  font-size: var(--font-size-card-meta);
  color: var(--color-text-secondary);
  margin-bottom: var(--spacing-xs);
}
.evo-focus, .evo-issue, .evo-result {
  font-size: var(--font-size-card-body);
  color: var(--color-text-secondary);
}
.evo-issue { color: var(--color-warning); }
.evo-result { color: var(--color-success); }
.goal-box {
  background: #1A365D;
  padding: var(--spacing-lg);
  border-radius: var(--radius-lg);
  text-align: center;
  margin-bottom: var(--spacing-md);
}
.goal-title {
  font-family: var(--font-family-display);
  font-size: var(--font-size-heading);
  font-weight: var(--font-weight-semibold);
  color: #FFFFFF;
  margin-bottom: var(--spacing-sm);
}
.goal-desc {
  font-size: var(--font-size-card-body);
  color: #F7FAFC;
  line-height: 1.6;
}
.harness-components {
  padding: var(--spacing-md);
  background: var(--color-accent-teal-light);
  border-radius: var(--radius-md);
  font-size: var(--font-size-card-body);
}
.harness-components ul {
  margin-top: var(--spacing-xs);
  margin-left: var(--spacing-md);
}
</style>

<!--
方法论也在演进。我把它分成三个阶段：

**Level 1: Prompt Engineering（提示词工程）**

这是最早的阶段。大家都在研究"怎么写更好的 prompt"。但很快发现问题：**指令写得再好，上下文不足还是会失败**。AI 不知道你的项目背景，你再怎么问，它也只能瞎猜。

**Level 2: Context Engineering（上下文工程）**

大家开始意识到上下文的重要性。这个阶段关注"如何为模型筛选最精准的上下文"。但问题是：**上下文管理仍依赖人工**，每次都要重新筛选，没法沉淀、没法复用。

**Level 3: Harness Engineering（编排工程）**

这是我们现在的阶段。核心思想：**用工程化手段约束 AI 行为**。通过模板、规则、工作流形成一个可复用的体系。让 AI 在规范的约束下执行任务，输出变得可预测、可追溯、可验证。

**今天分享的核心，就是给你一套完整的 Harness。**

这套 Harness 包含三部分：
- 模板：PRD、design、tasks 等标准化文档格式
- 规则：CLAUDE.md + rules 约束文件
- 工作流：propose → explore → apply → archive 四步流程

有了这套 Harness，你就不用每次都"祈祷 AI 能猜对"，而是让 AI 在规范约束下执行任务。
-->