---
layout: TwoCols
---

::left::

# 4.5 阶段总结

<div class="summary-table">

| 阶段 | 核心应用 |
|:---:|:---|
| 需求 | 需求推演、结构化描述 |
| 设计 | 架构设计、技术选型、接口契约、任务分解 |
| 实现 | 代码生成、测试生成 |
| 全局 | 知识规范化、上下文工程、安全审计 |

</div>

::right::

<div class="insight-box">
<strong>核心认知</strong>

<div class="insight-item">
AI 是"执行者"，不是"决策者"。它擅长生成，不擅长判断。
</div>

<div class="insight-item">
每个阶段都有明确的"人必须做"和"AI 可做"边界。
</div>

<div class="insight-item">
工具的作用是提高效率，不是替代思考。
</div>
</div>

<style>
.summary-table {
  margin-top: var(--spacing-md);
}
.summary-table table {
  width: 100%;
  border-collapse: collapse;
}
.summary-table th,
.summary-table td {
  padding: var(--spacing-xs) var(--spacing-sm);
  border: 1px solid var(--color-border);
  font-size: var(--font-size-card-body);
}
.summary-table th {
  background: var(--color-bg-subtle);
  font-family: var(--font-family-display);
  font-weight: var(--font-weight-medium);
}
.summary-table td:first-child {
  text-align: center;
  font-weight: var(--font-weight-medium);
  color: var(--color-primary);
}
.insight-box {
  background: #1A365D;
  padding: var(--spacing-md);
  border-radius: var(--radius-md);
  color: #FFFFFF;
}
.insight-box strong {
  font-family: var(--font-family-display);
  font-size: var(--font-size-card-title);
  margin-bottom: var(--spacing-sm);
  display: block;
}
.insight-item {
  font-size: var(--font-size-card-body);
  color: #F7FAFC;
  margin-bottom: var(--spacing-xs);
  padding-left: var(--spacing-md);
  position: relative;
}
.insight-item::before {
  content: "•";
  position: absolute;
  left: 0;
}
</style>

<!--
阶段总结：

**各阶段核心应用**：

- 需求：需求推演、结构化描述
- 设计：架构设计、技术选型、接口契约、任务分解
- 实现：代码生成、测试生成
- 全局：知识规范化、上下文工程、安全审计

**核心认知**：

1. AI 是"执行者"，不是"决策者"。它擅长生成，不擅长判断。

2. 每个阶段都有明确的"人必须做"和"AI 可做"边界。

3. 工具的作用是提高效率，不是替代思考。

记住这三点，工具才能真正发挥作用。
-->