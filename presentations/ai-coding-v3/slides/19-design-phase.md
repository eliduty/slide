---
layout: Default
---

# 3.4 设计阶段

<div class="stage-detail">

<div class="stage-header info">
<div class="stage-title">设计阶段</div>
<div class="stage-flow">propose → explore → apply → archive</div>
</div>

<div class="stage-grid">

<div class="stage-row">
<div class="row-label">负责</div>
<div class="row-content">SDE 主导 + PM 参与</div>
</div>

<div class="stage-row">
<div class="row-label">AI 可做</div>
<div class="row-content">技术方案生成、接口契约设计、任务拆分</div>
</div>

<div class="stage-row">
<div class="row-label">人必须做</div>
<div class="row-content">技术选型决策、架构边界定义</div>
</div>

<div class="stage-row">
<div class="row-label">产出</div>
<div class="row-content">proposal + design + tasks + specs</div>
</div>

<div class="stage-row">
<div class="row-label">进入条件</div>
<div class="row-content">技术评审通过</div>
</div>

<div class="stage-row">
<div class="row-label">模板文件</div>
<div class="row-content">openspec/changes/ 目录结构</div>
</div>

</div>

</div>

<style>
.stage-detail {
  margin-top: var(--spacing-md);
}
.stage-header {
  padding: var(--spacing-md);
  border-radius: var(--radius-md);
  margin-bottom: var(--spacing-sm);
}
.stage-header.info {
  background: var(--color-info);
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
设计阶段的详细定义：

**流程**：propose → explore → apply → archive

这是 OpenSpec 的核心工作流：
- propose：提出变更，生成 proposal.md
- explore：探索设计，生成 design.md 和 specs
- apply：执行任务，按 tasks.md 实施
- archive：归档沉淀

**负责**：SDE 主导 + PM 参与

**AI 可做**：
- 技术方案生成
- 接口契约设计
- 任务拆分

**人必须做**：
- 技术选型决策——用什么技术栈
- 架构边界定义——模块如何划分

**产出**：proposal + design + tasks + specs 四件套

**进入下一阶段条件**：技术评审通过

**模板文件**：openspec/changes/ 目录结构

这是设计阶段的定义。具体怎么用 AI 工具？让我们看下一页。
-->