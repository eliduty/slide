---
layout: Default
---

# 2.1 标准工作流三阶段

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
  gap: var(--spacing-sm);
  margin-top: var(--spacing-md);
}
.stage {
  flex: 1;
  border-radius: var(--radius-md);
  padding: var(--spacing-md);
  display: flex;
  flex-direction: column;
}
.stage:nth-child(1) { background: var(--color-success-light); border: 1px solid var(--color-success); }
.stage:nth-child(3) { background: var(--color-info-light); border: 1px solid var(--color-info); }
.stage:nth-child(5) { background: var(--color-warning-light); border: 1px solid var(--color-warning); }
.stage-header {
  display: flex;
  align-items: center;
  gap: var(--spacing-xs);
  margin-bottom: var(--spacing-sm);
}
.stage-num {
  font-family: var(--font-family-display);
  width: 28px;
  height: 28px;
  border-radius: var(--radius-sm);
  display: flex;
  align-items: center;
  justify-content: center;
  font-weight: var(--font-weight-semibold);
  font-size: var(--font-size-card-meta);
}
.stage:nth-child(1) .stage-num { background: var(--color-success); color: var(--color-bg-card); }
.stage:nth-child(3) .stage-num { background: var(--color-info); color: var(--color-bg-card); }
.stage:nth-child(5) .stage-num { background: var(--color-warning); color: var(--color-bg-card); }
.stage-title {
  font-family: var(--font-family-display);
  font-weight: var(--font-weight-medium);
  font-size: var(--font-size-card-title);
  color: var(--color-text-primary);
}
.stage-body { font-size: var(--font-size-card-body); color: var(--color-text-primary); }
.stage-body div { margin-bottom: var(--spacing-xs); }
.stage-body strong { color: var(--color-primary); }
.arrow {
  font-size: var(--font-size-heading);
  color: var(--color-text-muted);
  padding-top: var(--spacing-md);
}
.highlight {
  margin-top: var(--spacing-lg);
  padding: var(--spacing-md);
  background: var(--color-accent-teal-light);
  border-radius: var(--radius-md);
  border: 1px solid var(--color-accent-teal);
  font-size: var(--font-size-card-body);
  text-align: center;
  color: var(--color-text-primary);
}
</style>