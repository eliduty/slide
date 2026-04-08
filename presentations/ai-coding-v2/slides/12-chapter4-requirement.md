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
  font-family: var(--font-family-display);
  font-weight: var(--font-weight-medium);
  font-size: var(--font-size-card-title);
  color: var(--color-primary);
  margin-bottom: var(--spacing-md);
}
.task-list {
  display: flex;
  flex-direction: column;
  gap: var(--spacing-sm);
}
.task {
  display: flex;
  align-items: center;
  gap: var(--spacing-md);
  padding: var(--spacing-sm) var(--spacing-md);
  border-radius: var(--radius-md);
  border: 1px solid;
}
.task:nth-child(1) { background: var(--color-success-light); border-color: var(--color-success); }
.task:nth-child(2) { background: var(--color-info-light); border-color: var(--color-info); }
.task:nth-child(3) { background: var(--color-accent-teal-light); border-color: var(--color-accent-teal); }
.num {
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
.task:nth-child(1) .num { background: var(--color-success); color: var(--color-bg-card); }
.task:nth-child(2) .num { background: var(--color-info); color: var(--color-bg-card); }
.task:nth-child(3) .num { background: var(--color-accent-teal); color: var(--color-bg-card); }
.name {
  font-family: var(--font-family-display);
  font-weight: var(--font-weight-medium);
  font-size: var(--font-size-card-title);
  color: var(--color-text-primary);
}
.desc { font-size: var(--font-size-card-body); color: var(--color-text-secondary); }
.case-box {
  margin-top: var(--spacing-lg);
  padding: var(--spacing-sm) var(--spacing-md);
  background: var(--color-bg-hover);
  border-radius: var(--radius-md);
  font-size: var(--font-size-card-body);
  color: var(--color-text-primary);
}
</style>

<!--
在需求阶段，AI 主要做三件事：

**第一，需求推演完善**

你可能只给 AI 一句话的需求，比如"我想加一个批量导入功能"。AI 可以帮你推演：批量导入需要什么字段？重复数据怎么处理？失败怎么提示？这些细节你可能没考虑到，AI 可以帮你补充。

**第二，需求的结构化描述**

AI 可以把你零散的想法，整理成结构化的 PRD 文档。我们 skill 项目有一个 PRD 模板，大家可以去看看：`docs/requirements/prd-admin-web.md`。

**第三，界面原型生成**

配合 Pencil 工具，AI 可以快速生成界面原型。
-->