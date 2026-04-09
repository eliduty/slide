---
layout: Default
---

# 3.2 需求阶段

<div class="stage-detail">

<div class="stage-header">
<div class="stage-title">需求阶段</div>
<div class="stage-flow">需求推演 → 结构化描述 → PRD 文档</div>
</div>

<div class="stage-grid">

<div class="stage-row">
<div class="row-label">负责</div>
<div class="row-content">PM 主导 + SDE 参与</div>
</div>

<div class="stage-row">
<div class="row-label">AI 可做</div>
<div class="row-content">需求推演完善、结构化描述、界面原型生成</div>
</div>

<div class="stage-row">
<div class="row-label">人必须做</div>
<div class="row-content">业务目标定义、验收标准确定</div>
</div>

<div class="stage-row">
<div class="row-label">产出</div>
<div class="row-content">PRD 文档</div>
</div>

<div class="stage-row">
<div class="row-label">进入条件</div>
<div class="row-content">需求评审通过</div>
</div>

<div class="stage-row">
<div class="row-label">模板文件</div>
<div class="row-content">docs/requirements/prd-template.md</div>
</div>

</div>

</div>

<style>
.stage-detail {
  margin-top: var(--spacing-md);
}
.stage-header {
  background: var(--color-success);
  padding: var(--spacing-md);
  border-radius: var(--radius-md);
  margin-bottom: var(--spacing-sm);
}
.stage-title {
  font-family: var(--font-family-display);
  font-weight: var(--font-weight-semibold);
  font-size: var(--font-size-heading);
  color: #FFFFFF;
}
.stage-flow {
  font-size: var(--font-size-card-body);
  color: #F7FAFC;
  margin-top: var(--spacing-xs);
}
.stage-grid {
  display: flex;
  flex-direction: column;
  gap: var(--spacing-xs);
}
.stage-row {
  display: grid;
  grid-template-columns: 120px 1fr;
  padding: var(--spacing-sm);
  border-radius: var(--radius-sm);
  background: var(--color-bg-subtle);
}
.row-label {
  font-family: var(--font-family-display);
  font-weight: var(--font-weight-medium);
  color: var(--color-text-secondary);
}
.row-content {
  color: var(--color-text-primary);
}
</style>

<!--
需求阶段的详细定义：

**流程**：需求推演 → 结构化描述 → PRD 文档

**负责**：PM 主导 + SDE 参与

**AI 可做**：
- 需求推演完善——补充可能遗漏的场景
- 结构化描述——把模糊的想法变成结构化文档
- 界面原型生成——生成 UI 原型

**人必须做**：
- 业务目标定义——到底要解决什么问题
- 验收标准确定——什么才算"完成"

**产出**：PRD 文档

**进入下一阶段条件**：需求评审通过

**模板文件**：docs/requirements/prd-template.md

这是需求阶段的定义。那么具体怎么用 AI 工具？让我们看下一页。
-->