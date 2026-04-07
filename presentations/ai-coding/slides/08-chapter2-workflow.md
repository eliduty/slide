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
  align-items: flex-start;
  gap: 0.25rem;
  margin-top: 0.5rem;
}
.stage {
  flex: 1;
  background: var(--color-primary-light);
  border-radius: var(--radius-md);
  padding: 0.5rem;
}
.stage-header {
  display: flex;
  align-items: center;
  gap: 0.3rem;
  margin-bottom: 0.3rem;
}
.stage-num {
  background: var(--color-primary);
  color: white;
  width: 22px;
  height: 22px;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  font-weight: 600;
  font-size: 0.75rem;
}
.stage-title { font-weight: 600; font-size: 0.85rem; color: var(--color-text-primary); }
.stage-body { font-size: 0.75rem; color: var(--color-text-primary); }
.stage-body div { margin-bottom: 0.1rem; }
.arrow {
  font-size: 1.2rem;
  color: var(--color-primary);
  padding-top: 0.5rem;
}
.highlight {
  margin-top: 1rem;
  padding: 0.75rem;
  background: var(--color-info-light);
  border-radius: var(--radius-md);
  font-size: 0.85rem;
  text-align: center;
  color: var(--color-text-primary);
}
</style>