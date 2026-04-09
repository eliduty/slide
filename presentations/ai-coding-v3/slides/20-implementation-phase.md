---
layout: Default
---

# 3.5 实现阶段

<div class="stage-detail">

<div class="stage-header orange">
<div class="stage-title">实现阶段</div>
<div class="stage-flow">按 tasks 执行 → 生成代码 → 运行测试 → 质量验证</div>
</div>

<div class="stage-grid">

<div class="stage-row">
<div class="row-label">负责</div>
<div class="row-content">SDE</div>
</div>

<div class="stage-row">
<div class="row-label">AI 可做</div>
<div class="row-content">代码生成、测试生成、文档生成</div>
</div>

<div class="stage-row">
<div class="row-label">人必须做</div>
<div class="row-content">验证输出质量、处理边界情况</div>
</div>

<div class="stage-row">
<div class="row-label">产出</div>
<div class="row-content">代码 + 测试 + 文档</div>
</div>

<div class="stage-row">
<div class="row-label">进入条件</div>
<div class="row-content">lint 通过、测试覆盖达标</div>
</div>

<div class="stage-row">
<div class="row-label">配合工具</div>
<div class="row-content">OpenSpec apply + Superpowers TDD</div>
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
.stage-header.orange {
  background: var(--color-accent-orange);
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
实现阶段的详细定义：

**流程**：按 tasks 执行 → 生成代码 → 运行测试 → 质量验证

**负责**：SDE

**AI 可做**：
- 代码生成
- 测试生成
- 文档生成

**人必须做**：
- 验证输出质量——检查是否符合规范
- 处理边界情况——处理 AI 没考虑到的特殊情况

**产出**：代码 + 测试 + 文档

**进入下一阶段条件**：lint 通过、测试覆盖达标

**配合工具**：OpenSpec apply + Superpowers TDD

Superpowers TDD 会强制要求先生成测试再生成代码，确保测试覆盖。
-->