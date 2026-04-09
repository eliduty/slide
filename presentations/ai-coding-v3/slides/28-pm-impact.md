---
layout: Default
---

# 4.1 对 PM 工作的影响

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
  gap: var(--spacing-md);
  margin-top: var(--spacing-md);
}
.impact-card {
  padding: var(--spacing-md);
  border-radius: var(--radius-md);
  border-left: 3px solid;
}
.impact-card:nth-child(1) { background: var(--color-success-light); border-color: var(--color-success); }
.impact-card:nth-child(2) { background: var(--color-info-light); border-color: var(--color-info); }
.impact-card:nth-child(3) { background: var(--color-accent-gold-light); border-color: var(--color-accent-gold); }
.impact-card:nth-child(4) { background: var(--color-warning-light); border-color: var(--color-warning); }
.card-title {
  font-family: var(--font-family-display);
  font-weight: var(--font-weight-medium);
  font-size: var(--font-size-card-title);
  color: var(--color-text-primary);
}
.card-content {
  font-size: var(--font-size-card-body);
  color: var(--color-text-secondary);
  margin-top: var(--spacing-xs);
}
.case-ref {
  margin-top: var(--spacing-lg);
  padding: var(--spacing-sm) var(--spacing-md);
  background: var(--color-bg-hover);
  border-radius: var(--radius-md);
  font-size: var(--font-size-card-body);
  color: var(--color-text-primary);
}
</style>

<!--
AI Coding 对 PM 的影响，主要体现在这几个方面：

**需求陈述的要求变化**

以前需求可能写几句话就完了，现在需要用结构化模板。我们 skill 项目有一套 PRD 模板，包括：背景、目标、用户角色、功能列表、验收标准。这套模板，就是为了让 AI 能理解你的需求。

**一些设计工作可以由工具代劳**

界面原型、数据流图，这些以前需要 PM 画的东西，现在可以交给 AI。我们有一个 Pencil UI 设计工具，AI 可以直接生成界面原型。

**知识文档可以快速生成**

格式更规范，内容范围更标准化。

**需求变更的流程调整**

以前需求变更可能口头说一下，现在需要同步更新 spec 文件。因为 AI 只认文档，文档没更新，AI 就不知道需求变了。

了解了 PM 的变化，我们再看 SDE 和 QA。
-->