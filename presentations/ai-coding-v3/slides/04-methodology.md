---
layout: Default
---

# 方法论演进：从 Prompt 到 Harness

<div class="evolution-flow">

<div class="evo-card">
<div class="evo-header">
<div class="evo-badge">1</div>
<div class="evo-title">
<div class="evo-name">Prompt Engineering</div>
<div class="evo-label">提示词工程</div>
</div>
</div>
<div class="evo-body">
<div class="evo-focus">如何写更好的指令</div>
<div class="evo-problem">问题：上下文不足仍会失败</div>
</div>
</div>

<div class="evo-arrow">→</div>

<div class="evo-card">
<div class="evo-header">
<div class="evo-badge">2</div>
<div class="evo-title">
<div class="evo-name">Context Engineering</div>
<div class="evo-label">上下文工程</div>
</div>
</div>
<div class="evo-body">
<div class="evo-focus">如何筛选精准上下文</div>
<div class="evo-problem">问题：管理依赖人工，难以复用</div>
</div>
</div>

<div class="evo-arrow">→</div>

<div class="evo-card current">
<div class="evo-header">
<div class="evo-badge">3</div>
<div class="evo-title">
<div class="evo-name" style="color:#10b981">Harness Engineering</div>
<div class="evo-label highlight">编排工程</div>
</div>
</div>
<div class="evo-body">
<div class="evo-focus">如何工程化约束 AI</div>
<div class="evo-success">结果：模板+规则+工作流可复用体系</div>
</div>
<div class="current-tag">当前阶段</div>
</div>

</div>

<style>
.evolution-flow {
  display: flex;
  align-items: stretch;
  justify-content: center;
  gap: var(--spacing-lg);
  margin-top: var(--spacing-xl);
  height: calc(100% - 80px);
}

.evo-card {
  flex: 1;
  max-width: 320px;
  background: var(--color-bg-card);
  border: 1px solid var(--color-border);
  border-radius: var(--radius-lg);
  padding: var(--spacing-lg);
  position: relative;
  display: flex;
  flex-direction: column;
}

.evo-card:not(.current) {
  opacity: 0.85;
}

.evo-card.current {
  border-color: var(--color-primary);
  border-width: 2px;
  background: linear-gradient(135deg,
    rgba(var(--color-primary-rgb, 67, 97, 238), 0.12) 0%,
    rgba(var(--color-primary-rgb, 67, 97, 238), 0.05) 100%);
  box-shadow:
    0 4px 12px rgba(var(--color-primary-rgb, 67, 97, 238), 0.15),
    inset 0 1px 0 rgba(255, 255, 255, 0.5);
}

.evo-card.current .evo-name {
  color: var(--color-primary);
  font-weight: 700;
}

.evo-card.current .evo-label {
  color: var(--color-text-primary);
}

.evo-card.current .evo-focus {
  color: var(--color-text-primary);
  font-weight: 500;
}

.evo-header {
  display: flex;
  align-items: center;
  gap: var(--spacing-sm);
  margin-bottom: var(--spacing-md);
}

.evo-badge {
  width: 36px;
  height: 36px;
  border-radius: var(--radius-full);
  background: var(--color-bg-page);
  border: 2px solid var(--color-border);
  display: flex;
  align-items: center;
  justify-content: center;
  font-weight: 600;
  font-size: 16px;
  color: var(--color-text-secondary);
  flex-shrink: 0;
}

.evo-card.current .evo-badge {
  background: #10b981;
  border-color: #10b981;
  color: #ffffff;
  font-weight: 700;
  box-shadow: 0 2px 8px rgba(16, 185, 129, 0.3);
}

.evo-title {
  display: flex;
  flex-direction: column;
  gap: 2px;
}

.evo-name {
  font-weight: 600;
  font-size: var(--font-size-body);
  color: var(--color-text-primary);
}

.evo-label {
  font-size: var(--font-size-caption);
  color: var(--color-text-secondary);
}

.evo-label.highlight {
  color: var(--color-primary);
  font-weight: 500;
}

.evo-body {
  flex: 1;
  display: flex;
  flex-direction: column;
  gap: var(--spacing-sm);
}

.evo-focus {
  font-size: var(--font-size-body-sm);
  color: var(--color-text-secondary);
  line-height: 1.5;
}

.evo-problem {
  font-size: 13px;
  color: #fcd34d;
  background: rgba(245, 158, 11, 0.15);
  padding: var(--spacing-sm);
  border-radius: var(--radius-md);
  border-left: 3px solid #f59e0b;
  font-weight: 500;
}

.evo-success {
  font-size: 13px;
  color: #6ee7b7;
  background: rgba(16, 185, 129, 0.15);
  padding: var(--spacing-sm);
  border-radius: var(--radius-md);
  border-left: 3px solid #10b981;
  font-weight: 500;
}

.current-tag {
  position: absolute;
  top: -12px;
  right: 16px;
  background: #10b981;
  color: #ffffff;
  font-size: 12px;
  font-weight: 700;
  padding: 4px 12px;
  border-radius: var(--radius-full);
  box-shadow: 0 2px 8px rgba(16, 185, 129, 0.3);
  letter-spacing: 0.5px;
}

.evo-arrow {
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 24px;
  color: var(--color-primary);
  font-weight: bold;
}
</style>

<!--
方法论在不断演进。我们把它分成三个阶段：

Level 1: Prompt Engineering（提示词工程）
这是最早的阶段。大家都在研究「怎么写更好的 prompt」。但很快发现问题：指令写得再好，上下文不足还是会失败。AI 不知道你的项目背景，你再怎么问，它也只能瞎猜。

Level 2: Context Engineering（上下文工程）
大家开始意识到上下文的重要性。这个阶段关注「如何为模型筛选最精准的上下文」。但问题是：上下文管理仍依赖人工，每次都要重新筛选，没法沉淀、没法复用。

Level 3: Harness Engineering（编排工程）
这是我们现在的阶段。核心思想：用工程化手段约束 AI 行为。通过模板、规则、工作流形成一个可复用的体系。让 AI 在规范的约束下执行任务，输出变得可预测、可追溯、可验证。

今天分享的核心，就是给你一套完整的 Harness。
-->
