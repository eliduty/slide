---
layout: TwoCols
---

::left::

# 上下文工程

<div class="ce-core">

<div class="ce-title">什么是上下文工程？</div>
<div class="ce-def">管理"在什么时机、给 AI 什么信息"的能力</div>

</div>

<div class="ce-layers">

<div class="layer-item">
<div class="layer-name">项目层</div>
<div class="layer-desc">架构概述 + 技术栈 + 命名规范</div>
<div class="layer-file">CLAUDE.md</div>
</div>

<div class="layer-item">
<div class="layer-name">模块层</div>
<div class="layer-desc">模块职责 + 接口契约 + 数据模型</div>
<div class="layer-file">docs/modules/*.md</div>
</div>

<div class="layer-item">
<div class="layer-name">任务层</div>
<div class="layer-desc">当前任务的目标 + 约束 + 期望输出</div>
<div class="layer-file">design.md / tasks.md</div>
</div>

</div>

::right::

<div class="harness-panel">

<div class="harness-title">Harness Engineering</div>
<div class="harness-subtitle">渐进式披露原则</div>

<div class="harness-flow">

<div class="flow-step">
<div class="step-when">需求阶段</div>
<div class="step-what">业务背景 + 用户角色</div>
</div>

<div class="flow-step">
<div class="step-when">设计阶段</div>
<div class="step-what">技术规范 + 架构约束</div>
</div>

<div class="flow-step">
<div class="step-when">实现阶段</div>
<div class="step-what">具体模块 + 边界情况</div>
</div>

</div>

<div class="harness-rule">
<strong>规则：</strong>不要一次性把所有信息扔给 AI，按阶段逐步喂入
</div>

</div>

<style>
.ce-core {
  padding: var(--spacing-md);
  border-radius: var(--radius-md);
  background: var(--color-primary-light);
  border: 1px solid var(--color-primary);
  margin-bottom: var(--spacing-md);
}
.ce-title {
  font-family: var(--font-family-display);
  font-weight: var(--font-weight-semibold);
  font-size: var(--font-size-card-title);
  color: var(--color-text-primary);
}
.ce-def {
  font-size: var(--font-size-card-body);
  color: var(--color-text-secondary);
  margin-top: var(--spacing-xs);
}
.ce-layers {
  display: flex;
  flex-direction: column;
  gap: var(--spacing-sm);
}
.layer-item {
  padding: var(--spacing-sm) var(--spacing-md);
  border-radius: var(--radius-md);
  border: 1px solid;
  display: flex;
  align-items: center;
  gap: var(--spacing-md);
}
.layer-item:nth-child(1) { background: var(--color-success-light); border-color: var(--color-success); }
.layer-item:nth-child(2) { background: var(--color-info-light); border-color: var(--color-info); }
.layer-item:nth-child(3) { background: var(--color-warning-light); border-color: var(--color-warning); }
.layer-name {
  font-family: var(--font-family-display);
  font-weight: var(--font-weight-medium);
  font-size: var(--font-size-card-body);
  color: var(--color-text-primary);
  min-width: 60px;
}
.layer-desc {
  font-size: var(--font-size-card-meta);
  color: var(--color-text-secondary);
  flex: 1;
}
.layer-file {
  font-size: var(--font-size-card-meta);
  color: var(--color-primary);
  font-style: italic;
}
.harness-panel {
  background: #1A365D;
  padding: var(--spacing-lg);
  border-radius: var(--radius-lg);
  color: #FFFFFF;
  height: 100%;
}
.harness-title {
  font-family: var(--font-family-display);
  font-weight: var(--font-weight-semibold);
  font-size: var(--font-size-heading);
  text-align: center;
  margin-bottom: var(--spacing-xs);
}
.harness-subtitle {
  font-size: var(--font-size-card-body);
  text-align: center;
  opacity: 0.9;
  margin-bottom: var(--spacing-md);
}
.harness-flow {
  display: flex;
  flex-direction: column;
  gap: var(--spacing-sm);
}
.flow-step {
  display: flex;
  align-items: center;
  gap: var(--spacing-sm);
  padding: var(--spacing-sm);
  border-radius: var(--radius-md);
  background: rgba(255,255,255,0.1);
}
.step-when {
  font-weight: var(--font-weight-medium);
  font-size: var(--font-size-card-body);
  min-width: 80px;
}
.step-what {
  font-size: var(--font-size-card-meta);
  opacity: 0.9;
}
.harness-rule {
  margin-top: var(--spacing-md);
  padding: var(--spacing-md);
  border-radius: var(--radius-md);
  background: rgba(237,137,54,0.3);
  border: 1px solid rgba(237,137,54,0.6);
  font-size: var(--font-size-card-body);
  text-align: center;
}
</style>

<!--
现在我们来讲一个关键能力：**上下文工程**。

什么是上下文工程？简单说，就是管理"在什么时机、给 AI 什么信息"的能力。

很多人用 AI 不顺手，不是因为 AI 不行，是因为上下文没给好。上下文给太多，AI 信息过载，抓不住重点；上下文给太少，AI 缺乏背景，瞎猜乱编。

**上下文要分层管理：**

**第一层：项目层**

放在 CLAUDE.md 里。包括：架构概述、技术栈选择、命名规范。这是每次对话的"基座上下文"，AI 每次都会自动读取。

**第二层：模块层**

放在 docs/modules/*.md 里。包括：模块职责、接口契约、数据模型。当你让 AI 做某个模块的开发时，就把对应模块文档喂给它。

**第三层：任务层**

放在 design.md 和 tasks.md 里。包括：当前任务的目标、约束、期望输出。这是最细粒度的上下文，告诉 AI 这一次对话具体要做什么。

**Harness Engineering：渐进式披露**

这是一个专业术语，翻译过来就是"渐进式披露"。什么意思？不要一次性把所有信息扔给 AI，要按阶段逐步喂入。

**需求阶段**：只给业务背景和用户角色。让 AI 理解"我们在做什么"，不要给技术细节，否则 AI 会过早陷入技术实现。

**设计阶段**：给技术规范和架构约束。让 AI 知道"我们用什么技术、有什么限制"，开始生成技术方案。

**实现阶段**：给具体模块和边界情况。让 AI 知道"这个模块的边界在哪、特殊情况怎么处理"，生成高质量代码。

**记住一个规则：上下文要分层，披露要渐进。**

一次性喂太多，AI 会迷失；喂太少，AI 会瞎猜。把握好节奏，才能让 AI 发挥最大价值。
-->