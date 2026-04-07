---
layout: Default
---

# 3.1 对 PM 工作的影响

<div class="impact-grid">

<div class="impact-card">
<div class="card-title">需求陈述变化</div>
<div class="card-content">需要结构化模板（PRD模板），让AI能理解需求</div>
</div>

<div class="impact-card">
<div class="card-title">设计工作可代劳</div>
<div class="card-content">界面原型、数据流图可交给AI生成</div>
</div>

<div class="impact-card">
<div class="card-title">知识文档快速生成</div>
<div class="card-content">格式规范、内容范围更标准化</div>
</div>

<div class="impact-card">
<div class="card-title">需求变更流程调整</div>
<div class="card-content">必须同步更新 spec 文件，AI只认文档</div>
</div>

</div>

<div class="case-ref">
📁 模板参考：<code>docs/requirements/prd-admin-web.md</code>
</div>

<style>
.impact-grid {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 0.5rem;
  margin-top: 0.5rem;
}
.impact-card {
  background: var(--color-primary-light);
  padding: 0.6rem;
  border-radius: var(--radius-sm);
  border-left: 3px solid var(--color-primary);
}
.card-title { font-weight: 600; font-size: 0.85rem; color: var(--color-text-primary); }
.card-content { font-size: 0.8rem; color: var(--color-text-secondary); margin-top: 0.2rem; }
.case-ref {
  margin-top: 0.75rem;
  padding: 0.5rem 0.75rem;
  background: var(--color-bg-hover);
  border-radius: var(--radius-sm);
  font-size: 0.8rem;
  color: var(--color-text-primary);
}
</style>