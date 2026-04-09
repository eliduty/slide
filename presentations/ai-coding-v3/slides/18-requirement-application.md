---
layout: Default
---

# 3.3 需求阶段——工具应用

<div class="app-grid">

<div class="app-item">
<div class="app-num">01</div>
<div class="app-title">需求推演完善</div>
<div class="app-desc">基于少量需求描述，AI 帮你推演补充可能遗漏的场景和边界情况</div>
</div>

<div class="app-item">
<div class="app-num">02</div>
<div class="app-title">结构化描述</div>
<div class="app-desc">把模糊的想法转换成结构化的 Markdown 文档，便于评审和传承</div>
</div>

<div class="app-item">
<div class="app-num">03</div>
<div class="app-title">界面原型生成</div>
<div class="app-desc">快速生成可交互原型，验证产品方向，加速需求确认</div>
</div>

<div class="app-item">
<div class="app-num">04</div>
<div class="app-title">需求文档生成</div>
<div class="app-desc">根据结构化描述自动生成 PRD 文档，确保格式规范</div>
</div>

</div>

<div class="tool-tip">
<strong>配合工具：</strong>Superpowers brainstorm——精炼需求，避免理解偏差
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
.app-num {
  font-family: var(--font-family-display);
  font-weight: var(--font-weight-semibold);
  font-size: var(--font-size-heading);
  color: var(--color-success);
  margin-bottom: var(--spacing-xs);
}
.app-title {
  font-family: var(--font-family-display);
  font-weight: var(--font-weight-medium);
  font-size: var(--font-size-card-title);
  color: var(--color-text-primary);
  margin-bottom: var(--spacing-xs);
}
.app-desc {
  font-size: var(--font-size-card-body);
  color: var(--color-text-secondary);
}
.tool-tip {
  margin-top: var(--spacing-lg);
  padding: var(--spacing-md);
  background: var(--color-success-light);
  border-radius: var(--radius-md);
  font-size: var(--font-size-card-body);
  color: var(--color-text-primary);
}
</style>

<!--
需求阶段具体怎么用 AI 工具？

**01. 需求推演完善**

你给 AI 一个简单的需求描述，它会帮你推演补充可能遗漏的场景。比如你说"做一个用户登录功能"，AI 会帮你想到：忘记密码怎么办？账号被锁定怎么办？多设备登录怎么处理？

**02. 结构化描述**

把模糊的想法转换成结构化的 Markdown 文档。这样便于评审，也便于传承——后续接手的人能看清楚需求背景。

**03. 界面原型生成**

快速生成可交互原型，加速需求确认。产品经理可以用这个快速验证产品方向。

**04. 需求文档生成**

根据结构化描述自动生成 PRD 文档，确保格式规范。

**配合工具**：Superpowers brainstorm——精炼需求，避免理解偏差。

需求阶段完成后，进入设计阶段。这是 AI 发挥作用最大的阶段。
-->