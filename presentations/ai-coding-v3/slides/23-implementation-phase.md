---
layout: Default
---

# 3.7 实现阶段

<div class="stage-detail">

<div class="stage-header orange">
<div class="stage-title">实现阶段</div>
<div class="stage-flow"> apply → archive</div>
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
  margin-top: var(--spacing-sm);
}
.stage-header {
  padding: var(--spacing-sm) var(--spacing-md);
  border-radius: var(--radius-md);
  margin-bottom: var(--spacing-sm);
}
.stage-header.orange {
  background: #7B3F00;
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
  background: #7B3F00;
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
实现阶段的详细定义：

**流程**：apply 按 tasks 执行 → 生成代码 → 运行测试 → 质量验证，最后归档需求。

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

这是实现阶段的定义。具体 AI 工具可以帮我们完成哪些任务呢？让我们看下一页。
-->
