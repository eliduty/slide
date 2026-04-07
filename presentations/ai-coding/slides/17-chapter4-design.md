---
layout: Default
---

# 4.2 设计阶段

<div class="design-list">

<div class="design-row">
<div class="item">架构设计</div>
<div class="item">技术选型比较</div>
<div class="item">接口契约设计</div>
</div>

<div class="design-row">
<div class="item">界面交互原型</div>
<div class="item">测试方案制定</div>
<div class="item">CI/CD设计</div>
</div>

</div>

<div class="output-box">
<strong>设计阶段产出物三件套：</strong>
<span>proposal.md</span>
<span>design.md</span>
<span>tasks.md</span>
</div>

<div class="case-ref">
📁 案例路径：<code>openspec/changes/admin-role-authorization/</code>
</div>

<style>
.design-list { margin-top: 0.5rem; }
.design-row {
  display: flex;
  gap: 0.4rem;
  margin-bottom: 0.4rem;
}
.item {
  flex: 1;
  background: var(--color-primary-light);
  padding: 0.6rem;
  border-radius: var(--radius-sm);
  text-align: center;
  font-weight: 500;
  font-size: 0.85rem;
  color: var(--color-text-primary);
}
.output-box {
  margin-top: 1rem;
  padding: 0.75rem;
  background: var(--color-primary);
  color: white;
  border-radius: var(--radius-md);
  display: flex;
  align-items: center;
  gap: 1rem;
}
.output-box span {
  background: rgba(255,255,255,0.2);
  padding: 0.2rem 0.5rem;
  border-radius: var(--radius-sm);
  font-size: 0.8rem;
}
.case-ref {
  margin-top: 0.75rem;
  padding: 0.5rem 0.75rem;
  background: var(--color-bg-hover);
  border-radius: var(--radius-sm);
  font-size: 0.8rem;
  color: var(--color-text-primary);
}
</style>