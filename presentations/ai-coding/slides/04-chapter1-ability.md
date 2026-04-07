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
  gap: 0.75rem;
  margin-top: 0.75rem;
}
.ability-item {
  background: var(--color-primary-light);
  padding: 0.75rem;
  border-radius: var(--radius-md);
  text-align: center;
}
.level {
  font-weight: 600;
  margin-bottom: 0.25rem;
  padding: 0.2rem 0.5rem;
  border-radius: var(--radius-sm);
  font-size: 0.8rem;
}
.strong .level { background: var(--color-success); color: white; }
.guided .level { background: var(--color-primary); color: white; }
.risky .level { background: var(--color-warning); color: white; }
.dependent .level { background: #6b7280; color: white; }
.title { font-weight: 600; font-size: 0.9rem; color: var(--color-text-primary); }
.desc { font-size: 0.8rem; color: var(--color-text-secondary); }
.condition { font-size: 0.7rem; color: var(--color-text-secondary); margin-top: 0.3rem; }
.key-point {
  margin-top: 1rem;
  padding: 0.75rem;
  background: var(--color-info-light);
  border-radius: var(--radius-md);
  border-left: 4px solid var(--color-primary);
  font-size: 0.9rem;
  color: var(--color-text-primary);
}
</style>