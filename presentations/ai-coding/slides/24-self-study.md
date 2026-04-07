---
layout: Default
---

# 课后自学指引

<div class="level-path">

<div class="level">
<div class="badge beginner">初级</div>
<div class="content">
阅读工作流指南，理解四阶段流程
<div class="path">docs/guides/openspec-superpowers-workflow.md</div>
</div>
</div>

<div class="level">
<div class="badge intermediate">中级</div>
<div class="content">
参考变更案例，独立完成一个简单变更
<div class="path">openspec/changes/admin-role-authorization/</div>
</div>
</div>

<div class="level">
<div class="badge advanced">高级</div>
<div class="content">
开发团队专属Skill，沉淀最佳实践
<div class="path">.claude/skills/*/SKILL.md</div>
</div>
</div>

</div>

<style>
.level-path {
  display: flex;
  flex-direction: column;
  gap: 0.5rem;
  margin-top: 0.5rem;
}
.level {
  display: flex;
  gap: 0.75rem;
  padding: 0.6rem;
  background: var(--color-primary-light);
  border-radius: var(--radius-sm);
}
.badge {
  width: 50px;
  padding: 0.3rem;
  border-radius: var(--radius-sm);
  text-align: center;
  font-weight: 600;
  font-size: 0.8rem;
}
.beginner { background: var(--color-success); color: white; }
.intermediate { background: var(--color-primary); color: white; }
.advanced { background: #8b5cf6; color: white; }
.content { flex: 1; font-size: 0.85rem; color: var(--color-text-primary); }
.path {
  font-size: 0.75rem;
  color: var(--color-text-secondary);
  margin-top: 0.2rem;
  background: var(--color-bg-hover);
  padding: 0.2rem 0.5rem;
  border-radius: var(--radius-sm);
}
</style>