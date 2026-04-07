---
layout: Default
---

# 1.1 能做什么

<div class="ability-grid">

<div class="ability-item strong">
<div class="level">强</div>
<div class="title">代码生成</div>
<div class="desc">Vue组件、接口实现、配置文件</div>
<div class="condition">需清晰规范</div>
</div>

<div class="ability-item guided">
<div class="level">需人引导</div>
<div class="title">架构决策</div>
<div class="desc">Monorepo架构设计</div>
<div class="condition">明确约束</div>
</div>

<div class="ability-item risky">
<div class="level">有风险</div>
<div class="title">跨模块重构</div>
<div class="desc">多租户模块化</div>
<div class="condition">小步验证</div>
</div>

<div class="ability-item dependent">
<div class="level">依赖上下文</div>
<div class="title">业务逻辑理解</div>
<div class="desc">DDD领域模型</div>
<div class="condition">上下文质量</div>
</div>

</div>

<div class="key-point">
<strong>核心结论：</strong> AI 不是万能的，也不是无用的。关键在于用在什么地方。
</div>

<style>
.ability-grid {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: var(--spacing-md);
  margin-top: var(--spacing-md);
}
.ability-item {
  padding: var(--spacing-md);
  border-radius: var(--radius-md);
  border: 1px solid var(--color-border);
  text-align: center;
}
.ability-item:nth-child(1) { background: var(--color-success-light); border-color: var(--color-success); }
.ability-item:nth-child(2) { background: var(--color-info-light); border-color: var(--color-info); }
.ability-item:nth-child(3) { background: var(--color-warning-light); border-color: var(--color-warning); }
.ability-item:nth-child(4) { background: var(--color-bg-subtle); border-color: var(--color-text-muted); }
.level {
  font-family: var(--font-family-display);
  font-weight: var(--font-weight-semibold);
  margin-bottom: var(--spacing-xs);
  padding: 4px 12px;
  border-radius: var(--radius-sm);
  font-size: var(--font-size-card-meta);
}
.strong .level { background: var(--color-success); color: var(--color-bg-card); }
.guided .level { background: var(--color-info); color: var(--color-bg-card); }
.risky .level { background: var(--color-warning); color: var(--color-bg-card); }
.dependent .level { background: var(--color-text-muted); color: var(--color-bg-card); }
.title {
  font-family: var(--font-family-display);
  font-weight: var(--font-weight-medium);
  font-size: var(--font-size-card-title);
  color: var(--color-text-primary);
}
.desc { font-size: var(--font-size-card-body); color: var(--color-text-secondary); }
.condition { font-size: var(--font-size-card-meta); color: var(--color-text-muted); margin-top: var(--spacing-xs); }
.key-point {
  margin-top: var(--spacing-lg);
  padding: var(--spacing-md);
  background: var(--color-accent-orange-light);
  border-radius: var(--radius-md);
  border-left: 4px solid var(--color-accent-orange);
  font-size: var(--font-size-card-body);
  color: var(--color-text-primary);
}
</style>