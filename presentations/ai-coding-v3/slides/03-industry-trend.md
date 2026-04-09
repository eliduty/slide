---
layout: Default
---

# 行业趋势：从"模型崇拜"到"工程落地"

<div class="trend-timeline">

<div class="trend-phase">
<div class="phase-label">2022-2023</div>
<div class="phase-title">模型崇拜时代</div>
<div class="phase-desc">追求更强的模型参数规模</div>
<div class="phase-issue">问题：幻觉与失控无法解决</div>
</div>

<div class="arrow">→</div>

<div class="trend-phase">
<div class="phase-label">2024</div>
<div class="phase-title">上下文工程时代</div>
<div class="phase-desc">关注如何筛选精准上下文</div>
<div class="phase-issue">挑战：上下文管理难以复用</div>
</div>

<div class="arrow">→</div>

<div class="trend-phase current">
<div class="phase-label">2025+</div>
<div class="phase-title">编排工程时代</div>
<div class="phase-desc">工程化手段约束 AI 行为</div>
<div class="phase-issue">关键：规格驱动开发（SDD）</div>
</div>

</div>

<div class="key-insight">
<strong>核心认知：</strong>单纯依靠模型能力已无法解决复杂业务逻辑问题，上下文管理成为 AI 编码的核心挑战
</div>

<style>
.trend-timeline {
  display: flex;
  align-items: stretch;
  gap: var(--spacing-xs);
  margin-top: var(--spacing-md);
}
.trend-phase {
  flex: 1;
  padding: var(--spacing-md);
  border-radius: var(--radius-md);
  border: 1px solid var(--color-border);
}
.trend-phase:nth-child(1) { background: var(--color-bg-subtle); }
.trend-phase:nth-child(3) { background: var(--color-info-light); }
.trend-phase:nth-child(5) { background: var(--color-success-light); border-color: var(--color-success); }
.phase-label {
  font-family: var(--font-family-display);
  font-weight: var(--font-weight-semibold);
  font-size: var(--font-size-card-meta);
  color: var(--color-text-muted);
  margin-bottom: var(--spacing-xs);
}
.phase-title {
  font-family: var(--font-family-display);
  font-weight: var(--font-weight-medium);
  font-size: var(--font-size-card-title);
  color: var(--color-text-primary);
  margin-bottom: var(--spacing-xs);
}
.phase-desc {
  font-size: var(--font-size-card-body);
  color: var(--color-text-secondary);
}
.phase-issue {
  font-size: var(--font-size-card-meta);
  color: var(--color-warning);
  margin-top: var(--spacing-xs);
}
.arrow {
  font-size: var(--font-size-heading);
  color: var(--color-text-muted);
  padding-top: var(--spacing-md);
}
.key-insight {
  margin-top: var(--spacing-lg);
  padding: var(--spacing-md);
  background: var(--color-accent-orange-light);
  border-radius: var(--radius-md);
  border-left: 4px solid var(--color-accent-orange);
  font-size: var(--font-size-card-body);
  color: var(--color-text-primary);
}
</style>

<!--
行业正在经历一个重要的转型。

**2022-2023：模型崇拜时代**

那时候大家都在追求更强的模型——GPT-4、Claude 2，参数越来越大。但很快发现一个问题：**模型再强，幻觉和失控问题依然无法解决**。复杂业务逻辑中，AI 会给出看似合理但完全错误的方案。

**2024：上下文工程时代**

大家开始意识到：问题不在模型，而在上下文。我们开始关注如何给 AI 精选上下文。但这个阶段有个问题：**上下文管理很难复用**——每次都要人工筛选，没有沉淀。

**2025+：编排工程时代**

现在，行业共识正在形成：**用工程化手段约束 AI 行为**。通过模板、规则、工作流形成可复用体系。这就是今天分享的核心——规格驱动开发（SDD）。

**核心认知**：单纯依靠模型能力已无法解决复杂业务问题，上下文管理才是 AI 编码的核心挑战。
-->