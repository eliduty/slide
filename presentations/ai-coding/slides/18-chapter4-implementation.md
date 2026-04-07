---
layout: TwoCols
---

::left::

# 4.3 实现阶段

<div class="impl-list">
<div class="impl-item"><strong>代码生成</strong><span>根据 design.md 规范生成</span></div>
<div class="impl-item"><strong>注释生成</strong><span>添加文档注释</span></div>
<div class="impl-item"><strong>测试生成</strong><span>单测、集成测试</span></div>
<div class="impl-item"><strong>代码重构</strong><span>在tasks.md范围内</span></div>
</div>

::right::

<div class="skills-box">
<strong>关键 Skills</strong>

<div class="skill-card">
<div class="skill-name">vue-best-practices</div>
<div class="skill-desc">Vue开发规范，确保输出符合团队约定</div>
</div>

<div class="skill-card">
<div class="skill-name">test-driven-development</div>
<div class="skill-desc">TDD流程，先写失败的测试，再写代码</div>
</div>
</div>

<style>
.impl-list {
  display: flex;
  flex-direction: column;
  gap: var(--spacing-sm);
}
.impl-item {
  display: flex;
  justify-content: space-between;
  padding: var(--spacing-sm) var(--spacing-md);
  border-radius: var(--radius-md);
  border: 1px solid;
}
.impl-item:nth-child(1) { background: var(--color-info-light); border-color: var(--color-info); }
.impl-item:nth-child(2) { background: var(--color-success-light); border-color: var(--color-success); }
.impl-item:nth-child(3) { background: var(--color-warning-light); border-color: var(--color-warning); }
.impl-item:nth-child(4) { background: var(--color-accent-teal-light); border-color: var(--color-accent-teal); }
.impl-item strong { font-size: var(--font-size-card-title); }
.impl-item span { font-size: var(--font-size-card-body); color: var(--color-text-secondary); }
.skills-box {
  background: var(--color-bg-subtle);
  padding: var(--spacing-md);
  border-radius: var(--radius-lg);
  border: 1px solid var(--color-border);
}
.skills-box strong { display: block; margin-bottom: var(--spacing-sm); color: var(--color-text-primary); font-size: var(--font-size-card-title); }
.skill-card {
  background: var(--color-bg-card);
  padding: var(--spacing-sm);
  border-radius: var(--radius-md);
  margin-bottom: var(--spacing-sm);
  border: 1px solid;
}
.skill-card:nth-child(1) { border-color: var(--color-info); background: var(--color-info-light); }
.skill-card:nth-child(2) { border-color: var(--color-success); background: var(--color-success-light); }
.skill-name { font-family: var(--font-family-display); font-weight: var(--font-weight-medium); color: var(--color-primary); font-size: var(--font-size-card-title); }
.skill-desc { font-size: var(--font-size-card-body); color: var(--color-text-secondary); margin-top: var(--spacing-xs); }
</style>