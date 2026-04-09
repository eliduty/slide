---
layout: TwoCols
---

::left::

# 方法论演进：从 Prompt 到 Harness

<div class="evolution-container">

<div class="evo-step">
<div class="step-header">
<div class="step-badge">1</div>
<div class="step-titles">
<div class="step-name">Prompt Engineering</div>
<div class="step-label">提示词工程</div>
</div>
</div>
<div class="step-content">
<div class="step-focus">关注「如何写更好的指令」</div>
<div class="step-problem">
<strong>问题：</strong>上下文不足仍会失败
</div>
</div>
</div>

<div class="step-connector">
<div class="connector-line"></div>
<div class="connector-arrow">↓</div>
</div>

<div class="evo-step">
<div class="step-header">
<div class="step-badge">2</div>
<div class="step-titles">
<div class="step-name">Context Engineering</div>
<div class="step-label">上下文工程</div>
</div>
</div>
<div class="step-content">
<div class="step-focus">关注「如何筛选精准上下文」</div>
<div class="step-problem">
<strong>问题：</strong>管理依赖人工，难以复用
</div>
</div>
</div>

<div class="step-connector">
<div class="connector-line"></div>
<div class="connector-arrow">↓</div>
</div>

<div class="evo-step current">
<div class="step-header">
<div class="step-badge">3</div>
<div class="step-titles">
<div class="step-name">Harness Engineering</div>
<div class="step-label highlight">编排工程</div>
</div>
</div>
<div class="step-content">
<div class="step-focus">关注「如何工程化约束 AI」</div>
<div class="step-success">
<strong>结果：</strong>模板+规则+工作流可复用体系
</div>
</div>
<div class="current-tag">当前阶段</div>
</div>

</div>

::right::

<div class="goal-section">

<div class="goal-card">
<div class="goal-icon">🎯</div>
<h3 class="goal-title">本次分享的核心</h3>
<p class="goal-desc">
      给你一套完整的 <strong>Harness</strong>——让 AI 在规范约束下执行任务，输出<strong>可预测、可追溯、可验证</strong>
</p>
</div>

<div class="harness-detail">
<h4 class="detail-title">Harness 包含</h4>
<div class="detail-grid">
<div class="detail-item">
<div class="item-icon" style="--item-color: #4361EE;">📋</div>
<div class="item-text">
<div class="item-name">模板</div>
<div class="item-desc">PRD、design、tasks 等标准化文档</div>
</div>
</div>
<div class="detail-item">
<div class="item-icon" style="--item-color: #22C55E;">📜</div>
<div class="item-text">
<div class="item-name">规则</div>
<div class="item-desc">CLAUDE.md + rules 约束文件</div>
</div>
</div>
<div class="detail-item">
<div class="item-icon" style="--item-color: #F59E0B;">⚙️</div>
<div class="item-text">
<div class="item-name">工作流</div>
<div class="item-desc">propose → explore → apply → archive</div>
</div>
</div>
</div>
</div>

</div>

<style>
/* 左侧演进流程 */
.evolution-container {
  margin-top: var(--spacing-sm);
}

.evo-step {
  background: var(--color-bg-card);
  border: 1px solid var(--color-border);
  border-radius: var(--radius-md);
  padding: var(--spacing-sm);
  position: relative;
  transition: all var(--transition-normal);
}

.evo-step:not(.current) {
  opacity: 0.85;
}

.evo-step.current {
  border-color: var(--color-primary);
  background: linear-gradient(135deg, var(--color-primary-light) 0%, var(--color-bg-card) 100%);
  box-shadow: var(--shadow-md);
}

.step-header {
  display: flex;
  align-items: center;
  gap: var(--spacing-sm);
  margin-bottom: var(--spacing-xs);
}

.step-badge {
  width: 28px;
  height: 28px;
  border-radius: var(--radius-full);
  background: var(--color-bg-page);
  border: 2px solid var(--color-border);
  display: flex;
  align-items: center;
  justify-content: center;
  font-weight: 600;
  font-size: 14px;
  color: var(--color-text-secondary);
}

.evo-step.current .step-badge {
  background: var(--color-primary);
  border-color: var(--color-primary);
  color: white;
}

.step-titles {
  display: flex;
  flex-direction: column;
  gap: 2px;
}

.step-name {
  font-weight: 600;
  font-size: var(--font-size-body-sm);
  color: var(--color-text-primary);
}

.step-label {
  font-size: var(--font-size-caption);
  color: var(--color-text-secondary);
}

.step-label.highlight {
  color: var(--color-primary);
  font-weight: 500;
}

.step-content {
  margin-left: 40px;
}

.step-focus {
  font-size: 14px;
  color: var(--color-text-secondary);
  margin-bottom: 4px;
}

.step-problem {
  font-size: 13px;
  color: var(--color-warning);
  background: var(--color-warning-light);
  padding: 4px 8px;
  border-radius: var(--radius-sm);
  border-left: 3px solid var(--color-warning);
}

.step-success {
  font-size: 13px;
  color: var(--color-success);
  background: var(--color-success-light);
  padding: 4px 8px;
  border-radius: var(--radius-sm);
  border-left: 3px solid var(--color-success);
}

.current-tag {
  position: absolute;
  top: -10px;
  right: 12px;
  background: var(--color-primary);
  color: white;
  font-size: 12px;
  font-weight: 600;
  padding: 2px 10px;
  border-radius: var(--radius-full);
}

/* 步骤连接器 */
.step-connector {
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: var(--spacing-xs) 0;
}

.connector-line {
  width: 2px;
  height: 16px;
  background: linear-gradient(180deg, var(--color-border) 0%, var(--color-primary) 100%);
}

.connector-arrow {
  color: var(--color-primary);
  font-size: 12px;
  line-height: 1;
}

/* 右侧目标区域 */
.goal-section {
  display: flex;
  flex-direction: column;
  gap: var(--spacing-lg);
}

.goal-card {
  background: linear-gradient(135deg, var(--color-primary-light) 0%, var(--color-bg-card) 100%);
  border: 1px solid var(--color-primary);
  border-radius: var(--radius-lg);
  padding: var(--spacing-md);
  text-align: center;
  box-shadow: var(--shadow-sm);
}

.goal-icon {
  font-size: 36px;
  margin-bottom: var(--spacing-xs);
}

.goal-title {
  font-size: var(--font-size-card-title);
  font-weight: 600;
  color: var(--color-text-primary);
  margin: 0 0 var(--spacing-xs) 0;
}

.goal-desc {
  font-size: 14px;
  color: var(--color-text-secondary);
  line-height: 1.5;
  margin: 0;
}

.goal-desc strong {
  color: var(--color-primary);
}

/* Harness 详情 */
.harness-detail {
  background: var(--color-bg-card);
  border: 1px solid var(--color-border);
  border-radius: var(--radius-lg);
  padding: var(--spacing-md);
}

.detail-title {
  font-size: var(--font-size-card-title);
  font-weight: 600;
  color: var(--color-text-primary);
  margin: 0 0 var(--spacing-sm) 0;
  padding-bottom: var(--spacing-xs);
  border-bottom: 2px solid var(--color-bg-page);
}

.detail-grid {
  display: flex;
  flex-direction: column;
  gap: var(--spacing-sm);
}

.detail-item {
  display: flex;
  align-items: center;
  gap: var(--spacing-sm);
  padding: var(--spacing-xs);
  background: var(--color-bg-page);
  border-radius: var(--radius-md);
}

.detail-item:hover {
  background: var(--color-bg-hover);
  transform: translateX(4px);
}

.item-icon {
  width: 32px;
  height: 32px;
  background: var(--item-color);
  border-radius: var(--radius-md);
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 16px;
  flex-shrink: 0;
}

.item-text {
  display: flex;
  flex-direction: column;
  gap: 2px;
}

.item-name {
  font-weight: 600;
  font-size: 14px;
  color: var(--color-text-primary);
}

.item-desc {
  font-size: 12px;
  color: var(--color-text-secondary);
}
</style>

<!--
方法论也在不断演进。我把它分成三个阶段：

Level 1: Prompt Engineering（提示词工程）

这是最早的阶段。大家都在研究「怎么写更好的 prompt」。但很快发现问题：指令写得再好，上下文不足还是会失败。AI 不知道你的项目背景，你再怎么问，它也只能瞎猜。

Level 2: Context Engineering（上下文工程）

大家开始意识到上下文的重要性。这个阶段关注「如何为模型筛选最精准的上下文」。但问题是：上下文管理仍依赖人工，每次都要重新筛选，没法沉淀、没法复用。

Level 3: Harness Engineering（编排工程）

这是我们现在的阶段。核心思想：用工程化手段约束 AI 行为。通过模板、规则、工作流形成一个可复用的体系。让 AI 在规范的约束下执行任务，输出变得可预测、可追溯、可验证。

今天分享的核心，就是给你一套完整的 Harness。

这套 Harness 包含三部分：
- 模板：PRD、design、tasks 等标准化文档格式
- 规则：CLAUDE.md + rules 约束文件
- 工作流：propose → explore → apply → archive 四步流程

有了这套 Harness，你就不用每次都「祈祷 AI 能猜对」，而是让 AI 在规范约束下执行任务。

接下来，我们正式进入第一部分：AI Coding 的能力边界。
-->
