---
layout: TwoCols
---

::left::

# 3.2 对 SDE/QA 影响

<div class="sde-qa">

<div class="impact-item">
<strong>架构设计前移</strong>
<p>设计必须先行，design.md 在代码之前产出</p>
</div>

<div class="impact-item">
<strong>SDE 补测试技能</strong>
<p>AI可生成测试用例，需验证其业务意义</p>
</div>

<div class="impact-item">
<strong>QA 参与开发</strong>
<p>基于 tasks.md 任务分配，任务已拆得很细</p>
</div>

</div>

::right::

<div class="key-skills">
<strong>需要学习的能力</strong>
<ul>
<li>测试思维：什么是有效测试</li>
<li>任务拆分：如何写出 tasks.md</li>
<li>设计文档：design.md 写什么</li>
</ul>
</div>

<style>
.sde-qa {
  display: flex;
  flex-direction: column;
  gap: 0.5rem;
}
.impact-item {
  padding: 0.5rem;
  background: var(--color-primary-light);
  border-radius: var(--radius-sm);
}
.impact-item p {
  font-size: 0.8rem;
  color: var(--color-text-secondary);
  margin: 0.2rem 0 0 0;
}
.key-skills {
  background: var(--color-primary);
  color: white;
  padding: 1rem;
  border-radius: var(--radius-lg);
}
.key-skills ul {
  margin-top: 0.5rem;
  padding-left: 1rem;
}
.key-skills li { margin-bottom: 0.3rem; font-size: 0.85rem; }
</style>