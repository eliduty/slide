---
layout: TwoCols
---

::left::

# 3.6 阶段总结

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

<style>
.phase-summary {
  display: flex;
  flex-direction: column;
  gap: var(--spacing-sm);
}
.summary-item {
  display: flex;
  gap: var(--spacing-md);
  padding: var(--spacing-sm);
  border-radius: var(--radius-sm);
  background: var(--color-bg-subtle);
}
.summary-phase {
  font-family: var(--font-family-display);
  font-weight: var(--font-weight-medium);
  min-width: 80px;
  color: var(--color-primary);
}
.summary-key {
  color: var(--color-text-primary);
}
.key-reminders {
  background: var(--color-error-light);
  padding: var(--spacing-md);
  border-radius: var(--radius-md);
}
.key-reminders strong {
  font-family: var(--font-family-display);
  font-size: var(--font-size-card-title);
  color: var(--color-text-primary);
  margin-bottom: var(--spacing-sm);
  display: block;
}
.reminder-item {
  display: flex;
  gap: var(--spacing-md);
  margin-top: var(--spacing-xs);
}
.reminder-num {
  font-family: var(--font-family-display);
  font-weight: var(--font-weight-semibold);
  color: var(--color-error);
  min-width: 30px;
}
.reminder-text {
  color: var(--color-text-primary);
}
</style>

<!--
阶段总结：

**核心规律**：
- 需求：人定目标，AI 推演
- 设计：人做决策，AI 生成方案
- 环境规范：人定规范，AI 执行生成
- 实现：人把控质量，AI 辅助测试

**关键提醒**：

1. 顺序不能乱——跳过环境规范阶段是最常见错误
2. 每个阶段都有进入条件——不满足就不能进入下一阶段
3. 决策在人，执行在AI——这个边界不能模糊

记住这三点，四阶段工作流才能真正落地。
-->