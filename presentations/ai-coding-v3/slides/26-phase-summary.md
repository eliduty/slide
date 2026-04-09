---
layout: TwoCols
---

::left::

# 3.10 阶段总结

<div class="phase-summary">

<div class="summary-item">
<div class="summary-phase">需求</div>
<div class="summary-key">人定目标，AI 推演</div>
</div>

<div class="summary-item">
<div class="summary-phase">设计</div>
<div class="summary-key">人做决策，AI 生成方案</div>
</div>

<div class="summary-item">
<div class="summary-phase">环境规范</div>
<div class="summary-key">人定规范，AI 执行生成</div>
</div>

<div class="summary-item">
<div class="summary-phase">实现</div>
<div class="summary-key">人把控质量，AI 辅助测试</div>
</div>

</div>

<div class="core-app">
<strong>各阶段核心应用</strong>
<ul>
<li>需求：需求推演、结构化描述</li>
<li>设计：架构设计、技术选型、接口契约、任务分解</li>
<li>实现：代码生成、测试生成</li>
<li>全局：知识规范化、上下文工程、安全审计</li>
</ul>
</div>

::right::

<div class="key-reminders">
<strong>关键提醒</strong>

<div class="reminder-item">
<div class="reminder-num">01</div>
<div class="reminder-text">顺序不能乱——跳过环境规范阶段是最常见错误</div>
</div>

<div class="reminder-item">
<div class="reminder-num">02</div>
<div class="reminder-text">每个阶段都有进入条件——不满足就不能进入下一阶段</div>
</div>

<div class="reminder-item">
<div class="reminder-num">03</div>
<div class="reminder-text">决策在人，执行在AI——这个边界不能模糊</div>
</div>

</div>

<div class="insight-box">
<strong>核心认知</strong>
<p>AI 是"执行者"，不是"决策者"。它擅长生成，不擅长判断。工具的作用是提高效率，不是替代思考。</p>
</div>

<style>
.phase-summary {
  display: flex;
  flex-direction: column;
  gap: 8px;
}
.summary-item {
  display: flex;
  gap: var(--spacing-sm);
  padding: 8px var(--spacing-sm);
  border-radius: var(--radius-sm);
  background: var(--color-bg-subtle);
}
.summary-phase {
  font-family: var(--font-family-display);
  font-weight: var(--font-weight-medium);
  min-width: 80px;
  color: var(--color-primary);
  font-size: 15px;
}
.summary-key {
  color: var(--color-text-primary);
  font-size: 15px;
}
.core-app {
  margin-top: var(--spacing-sm);
  padding: var(--spacing-sm);
  border-radius: var(--radius-md);
  background: var(--color-accent-teal-light);
}
.core-app strong {
  font-size: 15px;
}
.core-app ul {
  margin: 4px 0 0 var(--spacing-md);
  font-size: 13px;
}
.key-reminders {
  background: var(--color-error-light);
  padding: var(--spacing-sm);
  border-radius: var(--radius-md);
}
.key-reminders strong {
  font-family: var(--font-family-display);
  font-size: 16px;
  color: var(--color-text-primary);
  margin-bottom: var(--spacing-xs);
  display: block;
}
.reminder-item {
  display: flex;
  gap: var(--spacing-sm);
  margin-top: 4px;
}
.reminder-num {
  font-family: var(--font-family-display);
  font-weight: var(--font-weight-semibold);
  color: var(--color-error);
  min-width: 24px;
  font-size: 14px;
}
.reminder-text {
  color: var(--color-text-primary);
  font-size: 14px;
}
.insight-box {
  margin-top: var(--spacing-sm);
  padding: var(--spacing-sm);
  background: #1A365D;
  border-radius: var(--radius-md);
  color: #FFFFFF;
}
.insight-box strong {
  font-family: var(--font-family-display);
  font-size: 16px;
  margin-bottom: 4px;
  display: block;
}
.insight-box p {
  font-size: 14px;
  margin: 0;
}
</style>

<!--
好，四阶段工作流我们就讲完了。来做个总结：

**各阶段的核心规律**：

- 需求：人定目标，AI 推演
- 设计：人做决策，AI 生成方案
- 环境规范：人定规范，AI 执行生成
- 实现：人把控质量，AI 辅助测试

**各阶段的核心应用**：

- 需求：需求推演、结构化描述
- 设计：架构设计、技术选型、接口契约、任务分解
- 实现：代码生成、测试生成
- 全局：知识规范化、上下文工程、安全审计

**三个关键提醒**：

1. 顺序不能乱——跳过环境规范阶段是最常见错误
2. 每个阶段都有进入条件——不满足就不能进入下一阶段
3. 决策在人，执行在AI——这个边界不能模糊

**核心认知**：

AI 是"执行者"，不是"决策者"。它擅长生成，不擅长判断。工具的作用是提高效率，不是替代思考。

记住这三点，四阶段工作流才能真正落地。

理解了四阶段工作流程，我们来看这套流程对现有工作的影响。
-->