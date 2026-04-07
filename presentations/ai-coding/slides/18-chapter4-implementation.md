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
  gap: 0.4rem;
}
.impl-item {
  display: flex;
  justify-content: space-between;
  padding: 0.5rem 0.75rem;
  background: var(--color-primary-light);
  border-radius: var(--radius-sm);
  color: var(--color-text-primary);
}
.impl-item span { font-size: 0.8rem; color: var(--color-text-secondary); }
.skills-box {
  background: var(--color-bg-hover);
  padding: 0.75rem;
  border-radius: var(--radius-lg);
}
.skills-box strong { display: block; margin-bottom: 0.5rem; color: var(--color-text-primary); }
.skill-card {
  background: var(--color-primary-light);
  padding: 0.5rem;
  border-radius: var(--radius-sm);
  margin-bottom: 0.4rem;
}
.skill-name { font-weight: 600; color: var(--color-primary); font-size: 0.85rem; }
.skill-desc { font-size: 0.75rem; color: var(--color-text-secondary); margin-top: 0.1rem; }
</style>