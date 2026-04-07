---
layout: Default
---

# 4.1 需求阶段

<div class="stage-title">AI 可以做的事情</div>

<div class="task-list">

<div class="task">
<span class="num">01</span>
<span class="name">需求推演完善</span>
<span class="desc">基于一句话需求，推演细节场景</span>
</div>

<div class="task">
<span class="num">02</span>
<span class="name">结构化描述</span>
<span class="desc">将零散想法整理成 PRD 文档</span>
</div>

<div class="task">
<span class="num">03</span>
<span class="name">界面原型生成</span>
<span class="desc">配合 Pencil 工具快速出原型</span>
</div>

</div>

<div class="case-box">
📁 模板路径：<code>docs/requirements/prd-admin-web.md</code>
</div>

<style>
.stage-title {
  font-weight: 600;
  font-size: 0.85rem;
  color: var(--color-primary);
  margin-bottom: 0.5rem;
}
.task-list {
  display: flex;
  flex-direction: column;
  gap: 0.4rem;
}
.task {
  display: flex;
  align-items: center;
  gap: 0.5rem;
  padding: 0.5rem 0.75rem;
  background: var(--color-primary-light);
  border-radius: var(--radius-sm);
}
.num {
  background: var(--color-primary);
  color: white;
  width: 26px;
  height: 26px;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  font-weight: 600;
  font-size: 0.75rem;
}
.name { font-weight: 600; font-size: 0.85rem; color: var(--color-text-primary); }
.desc { font-size: 0.75rem; color: var(--color-text-secondary); }
.case-box {
  margin-top: 0.75rem;
  padding: 0.5rem 0.75rem;
  background: var(--color-bg-hover);
  border-radius: var(--radius-sm);
  font-size: 0.8rem;
  color: var(--color-text-primary);
}
</style>