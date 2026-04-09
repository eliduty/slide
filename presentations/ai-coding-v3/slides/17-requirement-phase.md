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
  margin-top: var(--spacing-sm);
}
.stage-header {
  background: #1B4332;
  padding: var(--spacing-sm) var(--spacing-md);
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
  font-size: var(--font-size-body);
  color: #F7FAFC;
  margin-top: 4px;
}
.stage-grid {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: var(--spacing-xs);
}
.stage-row {
  display: flex;
  align-items: flex-start;
  gap: var(--spacing-xs);
  padding: var(--spacing-xs) var(--spacing-sm);
  border-radius: var(--radius-sm);
  background: var(--color-bg-subtle);
}
.row-label {
  flex-shrink: 0;
  padding: 2px 10px;
  border-radius: var(--radius-sm);
  background: #1B4332;
  font-family: var(--font-family-display);
  font-weight: var(--font-weight-semibold);
  font-size: 18px;
  color: #FFFFFF;
}
.row-content {
  flex: 1;
  padding-top: 2px;
  font-size: var(--font-size-body);
  color: var(--color-text-primary);
  line-height: 1.4;
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

这是需求阶段的定义。那么具体怎么用 AI 工具？
-->
