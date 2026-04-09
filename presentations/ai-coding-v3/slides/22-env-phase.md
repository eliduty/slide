---
layout: Default
---

# 3.6 环境规范阶段

<div class="stage-detail">

<div class="stage-header">
<div class="stage-title">环境规范阶段</div>
<div class="stage-flow">配置 CLAUDE.md → 配置 rules → 验证上下文</div>
</div>

<div class="stage-grid">

<div class="stage-row">
<div class="row-label">负责</div>
<div class="row-content">SDE</div>
</div>

<div class="stage-row">
<div class="row-label">AI 可做</div>
<div class="row-content">辅助配置生成</div>
</div>

<div class="stage-row">
<div class="row-label">人必须做</div>
<div class="row-content">编写项目规范、验证上下文有效性</div>
</div>

<div class="stage-row">
<div class="row-label">产出</div>
<div class="row-content">CLAUDE.md + .claude/ 目录</div>
</div>

<div class="stage-row">
<div class="row-label">进入条件</div>
<div class="row-content">AI 能正确理解项目上下文</div>
</div>

<div class="stage-row">
<div class="row-label">模板文件</div>
<div class="row-content">CLAUDE.md、.claude/ 目录</div>
</div>

</div>

<div class="warning-box">
<strong>⚠️ 最常见错误：</strong>跳过此阶段直接进入实现，导致 AI 不理解项目约束，输出偏离预期。
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
  background: #0F4C4C;
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
  background: #0F4C4C;
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
.warning-box {
  margin-top: var(--spacing-sm);
  padding: var(--spacing-sm) var(--spacing-md);
  background: var(--color-warning-light);
  border-radius: var(--radius-md);
  border-left: 4px solid var(--color-warning);
  font-size: var(--font-size-body);
  color: var(--color-text-primary);
}
</style>

<!--
环境规范阶段的详细定义：

**流程**：配置 CLAUDE.md → 配置 rules → 验证上下文

**负责**：SDE

**AI 可做**：辅助配置生成——AI 可以帮你生成配置模板

**人必须做**：
- 编写项目规范——把项目的技术约束、业务规则写清楚
- 验证上下文有效性——确保 AI 能正确理解

**产出**：CLAUDE.md + .claude/ 目录

**进入下一阶段条件**：AI 能正确理解项目上下文

**⚠️ 最常见错误**：跳过此阶段直接进入实现。

很多人拿到任务就让 AI 写代码，但 AI 不理解项目的技术约束和业务规则，输出就会偏离预期。**环境规范阶段就是把上下文准备好，让 AI 在实现阶段有足够的背景。**

环境规范配置好后，就可以进入实现阶段了。
-->
