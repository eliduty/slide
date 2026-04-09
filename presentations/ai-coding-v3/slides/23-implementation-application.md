---
layout: Default
---

# 3.8 实现阶段——工具应用

<div class="app-grid">

<div class="app-item">
<div class="app-header">
<div class="app-num">01</div>
<div class="app-title">代码生成</div>
</div>
<div class="app-desc">根据 specs 和 tasks 生成代码，确保符合规范</div>
</div>

<div class="app-item">
<div class="app-header">
<div class="app-num">02</div>
<div class="app-title">注释生成</div>
</div>
<div class="app-desc">自动生成函数注释、模块文档</div>
</div>

<div class="app-item">
<div class="app-header">
<div class="app-num">03</div>
<div class="app-title">测试生成与执行</div>
</div>
<div class="app-desc">生成单元测试、集成测试，并执行验证</div>
</div>

<div class="app-item">
<div class="app-header">
<div class="app-num">04</div>
<div class="app-title">多层次测试覆盖</div>
</div>
<div class="app-desc">单元测试、集成测试、系统测试多层次覆盖</div>
</div>

</div>

<div class="bottom-row">
<div class="warning-box">
<strong>⚠️ 重要提醒：</strong>AI 生成的代码必须人工验证其"业务正确性"
</div>
<div class="tool-box">
<strong>配合工具：</strong>OpenSpec apply + Superpowers TDD
</div>
</div>

<style>
.app-grid {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: var(--spacing-md);
  margin-top: var(--spacing-md);
}
.app-item {
  padding: var(--spacing-md);
  border-radius: var(--radius-md);
  border: 1px solid var(--color-border);
  background: var(--color-bg-subtle);
}
.app-header {
  display: flex;
  align-items: center;
  gap: var(--spacing-sm);
  margin-bottom: var(--spacing-xs);
}
.app-num {
  font-family: var(--font-family-display);
  font-weight: var(--font-weight-semibold);
  font-size: 18px;
  color: var(--color-accent-teal);
}
.app-title {
  font-family: var(--font-family-display);
  font-weight: var(--font-weight-medium);
  font-size: 20px;
  color: var(--color-text-primary);
}
.app-desc {
  font-size: 14px;
  color: var(--color-text-secondary);
  line-height: 1.5;
}
.bottom-row {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: var(--spacing-md);
  margin-top: var(--spacing-md);
}
.warning-box {
  padding: var(--spacing-sm) var(--spacing-md);
  background: var(--color-warning-light);
  border-radius: var(--radius-md);
  font-size: 14px;
}
.tool-box {
  padding: var(--spacing-sm) var(--spacing-md);
  background: var(--color-accent-teal-light);
  border-radius: var(--radius-md);
  font-size: 14px;
}
</style>

<!--
AI 工具可以帮我们：

**01. 代码生成**

根据 specs 和 tasks 生成代码，确保符合规范。前面阶段定义得好，这个阶段就顺利。

**02. 注释生成**

自动生成函数注释、模块文档，降低维护成本。

**03. 生成测试用例与执行测试用例**

生成单元测试、集成测试，并执行验证。

**04. 多层次测试覆盖**

单元测试、集成测试、系统测试多层次覆盖。

**⚠️ 重要提醒**：AI 生成的代码必须人工验证其"业务正确性"——能跑通 ≠ 有业务意义。

测试能跑通，不代表它真正验证了业务逻辑。你必须检查：测试用例是否覆盖了关键业务场景？断言是否正确？

**配合工具**：OpenSpec apply + Superpowers TDD——按规范执行，强制测试。

除了各阶段的具体应用，还有一些工作贯穿整个流程。让我们看下一页。
-->
