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
  gap: var(--spacing-md);
  margin-top: var(--spacing-md);
}
.level {
  display: flex;
  gap: var(--spacing-md);
  padding: var(--spacing-sm);
  border-radius: var(--radius-md);
  border: 1px solid;
}
.level:nth-child(1) { background: var(--color-success-light); border-color: var(--color-success); }
.level:nth-child(2) { background: var(--color-info-light); border-color: var(--color-info); }
.level:nth-child(3) { background: var(--color-accent-gold-light); border-color: var(--color-accent-gold); }
.badge {
  font-family: var(--font-family-display);
  min-width: 50px;
  padding: 4px 10px;
  border-radius: var(--radius-sm);
  text-align: center;
  font-weight: var(--font-weight-medium);
  font-size: var(--font-size-card-meta);
  display: flex;
  align-items: center;
  justify-content: center;
}
.level:nth-child(1) .badge { background: var(--color-success); color: var(--color-bg-card); }
.level:nth-child(2) .badge { background: var(--color-info); color: var(--color-bg-card); }
.level:nth-child(3) .badge { background: var(--color-accent-gold); color: var(--color-bg-card); }
.content { flex: 1; font-size: var(--font-size-card-body); color: var(--color-text-primary); }
.path {
  font-family: var(--font-family-code);
  font-size: var(--font-size-card-meta);
  color: var(--color-text-secondary);
  margin-top: var(--spacing-xs);
  background: var(--color-bg-hover);
  padding: 2px 8px;
  border-radius: var(--radius-sm);
}
</style>

<!--
**课后自学建议**：

- **初级**：阅读 `docs/guides/openspec-superpowers-workflow.md`，理解四阶段流程。
- **中级**：参考 `openspec/changes/admin-role-authorization/` 案例，独立完成一个简单变更。
- **高级**：开发一个团队专属 Skill，沉淀你们的最佳实践。

培训结束后，建议你从初级开始，逐步进阶。

课后自学可以根据这个路径进行。接下来进入问答环节。
-->