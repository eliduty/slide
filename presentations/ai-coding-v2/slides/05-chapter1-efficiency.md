---
layout: Default
---

# 1.2 哪些地方带来效率

<div class="efficiency-grid">

<div class="efficiency-card">
<div class="efficiency-scene">接口契约设计</div>
<div class="efficiency-times">
<span class="old">2天</span>
<span class="arrow">→</span>
<span class="new">半天</span>
</div>
<div class="efficiency-gain">提升 75%</div>
</div>

<div class="efficiency-card">
<div class="efficiency-scene">UI 原型设计</div>
<div class="efficiency-times">
<span class="old">1天</span>
<span class="arrow">→</span>
<span class="new">2小时</span>
</div>
<div class="efficiency-gain">提升 80%</div>
</div>

<div class="efficiency-card">
<div class="efficiency-scene">测试用例生成</div>
<div class="efficiency-times">
<span class="old">3小时</span>
<span class="arrow">→</span>
<span class="new">30分钟</span>
</div>
<div class="efficiency-gain">提升 83%</div>
</div>

</div>

<div class="warning-box">
<strong>⚠️ 需要额外 review 成本的环节：</strong> 架构决策验证、跨模块影响分析、AI输出质量校验
</div>

<div class="insight">
💡 AI 给出的方案，你不能直接信，得自己推演一遍
</div>

<style>
.efficiency-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: var(--spacing-md);
  margin-top: var(--spacing-md);
}
.efficiency-card {
  background: var(--color-bg-subtle);
  border-radius: var(--radius-lg);
  padding: var(--spacing-md);
  text-align: center;
  border: 1px solid var(--color-border);
}
.efficiency-card:nth-child(1) { background: var(--color-success-light); border-color: var(--color-success); }
.efficiency-card:nth-child(2) { background: var(--color-info-light); border-color: var(--color-info); }
.efficiency-card:nth-child(3) { background: var(--color-accent-gold-light); border-color: var(--color-accent-gold); }
.efficiency-scene {
  font-family: var(--font-family-display);
  font-weight: var(--font-weight-medium);
  font-size: var(--font-size-card-title);
  color: var(--color-text-primary);
  margin-bottom: var(--spacing-sm);
}
.efficiency-times {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: var(--spacing-sm);
  margin-bottom: var(--spacing-sm);
}
.old {
  font-size: var(--font-size-card-body);
  color: var(--color-text-secondary);
  text-decoration: line-through;
}
.arrow {
  color: var(--color-primary);
  font-size: var(--font-size-card-title);
}
.new {
  font-size: var(--font-size-card-body);
  color: var(--color-primary);
  font-weight: var(--font-weight-medium);
}
.efficiency-gain {
  font-family: var(--font-family-display);
  font-weight: var(--font-weight-semibold);
  font-size: var(--font-size-card-title);
  color: var(--color-success);
  background: var(--color-bg-card);
  padding: 4px 12px;
  border-radius: var(--radius-sm);
  display: inline-block;
}
.warning-box {
  margin-top: var(--spacing-lg);
  padding: var(--spacing-md);
  background: var(--color-warning-light);
  border-radius: var(--radius-md);
  border-left: 4px solid var(--color-warning);
  color: var(--color-text-primary);
  font-size: var(--font-size-card-body);
  border: 1px solid var(--color-warning);
}
.insight {
  margin-top: var(--spacing-md);
  padding: var(--spacing-sm) var(--spacing-md);
  background: var(--color-accent-teal-light);
  border-radius: var(--radius-md);
  font-size: var(--font-size-card-body);
  color: var(--color-text-primary);
  border: 1px solid var(--color-accent-teal);
}
</style>

<!--
那 AI 到底带来了多少效率提升呢？我们统计了 skill 项目的一些数据：

接口契约设计，从 2 天缩短到半天，提升 75%；
UI 原型设计，从 1 天缩短到 2 小时，提升 80%；
测试用例生成，从 3 小时缩短到 30 分钟，提升 83%。

这些数据看起来很美好，但我必须告诉大家：**AI 也引入了额外的 review 成本。**

哪些环节需要额外花时间？架构决策验证、跨模块影响分析、AI输出质量校验。AI 给出的方案，你得上手验证。它说"这个方案可行"，你不能直接信，得自己推演一遍。
-->