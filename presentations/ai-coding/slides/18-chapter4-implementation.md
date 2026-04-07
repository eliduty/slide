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

<!--
实现阶段，AI 主要做四件事：

1. **代码生成**——根据设计文档生成代码
2. **注释生成**——给代码加注释、写文档
3. **测试生成与执行**——生成测试用例并执行
4. **多层次测试**——单元测试、集成测试、系统测试

这里我要特别强调两个 Skills：

**vue-best-practices**

这是我们积累的 Vue 开发规范。当你用 AI 写 Vue 代码时，这个 Skill 会自动加载，确保输出的代码符合团队规范。它的核心原则是：状态可预测、数据流显式、组件小而专注。

**test-driven-development**

这是测试驱动开发的流程。核心原则是：**没有失败的测试，就不写生产代码**。先写测试，看它失败，再写最小代码让它通过，然后重构。这个流程看起来慢，但长期来看，它比"写完代码再补测试"快得多。
-->