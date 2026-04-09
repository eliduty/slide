---
layout: Default
---

# 3.4 设计阶段

<div class="stage-detail">

<div class="stage-header info">
<div class="stage-title">设计阶段</div>
<div class="stage-flow">propose → explore</div>
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
  margin-top: var(--spacing-sm);
}
.stage-header {
  padding: var(--spacing-sm) var(--spacing-md);
  border-radius: var(--radius-md);
  margin-bottom: var(--spacing-sm);
}
.stage-header.info {
  background: #1E3A5F;
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
  background: #1E3A5F;
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
设计阶段的详细定义：

**流程**：propose → explore 

这是 OpenSpec 的核心工作流的一部分：
- explore：探索设计，
- propose：提出变更，生成 design.md 和 specs、proposal.md、tasks.md

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
