---
layout: Default
---

# 4.4 贯穿全局

<div class="global-grid">

<div class="global-item">
<div class="icon">📋</div>
<div class="title">CLAUDE.md</div>
<div class="desc">项目级规则文件</div>
</div>

<div class="global-item">
<div class="icon">📖</div>
<div class="title">上下文披露</div>
<div class="desc">渐进式喂信息</div>
</div>

<div class="global-item">
<div class="icon">🔍</div>
<div class="title">评审</div>
<div class="desc">AI辅助，人决策</div>
</div>

<div class="global-item">
<div class="icon">🔒</div>
<div class="title">安全审计</div>
<div class="desc">扫描漏洞</div>
</div>

<div class="global-item">
<div class="icon">🌳</div>
<div class="title">分支治理</div>
<div class="desc">branch Skill</div>
</div>

<div class="global-item">
<div class="icon">📚</div>
<div class="title">Skills体系</div>
<div class="desc">沉淀实践</div>
</div>

</div>

<style>
.global-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: var(--spacing-md);
  margin-top: var(--spacing-md);
}
.global-item {
  padding: var(--spacing-md);
  border-radius: var(--radius-md);
  text-align: center;
  border: 1px solid;
}
.global-item:nth-child(1) { background: var(--color-primary-light); border-color: var(--color-primary); }
.global-item:nth-child(2) { background: var(--color-accent-teal-light); border-color: var(--color-accent-teal); }
.global-item:nth-child(3) { background: var(--color-warning-light); border-color: var(--color-warning); }
.global-item:nth-child(4) { background: var(--color-error-light); border-color: var(--color-error); }
.global-item:nth-child(5) { background: var(--color-success-light); border-color: var(--color-success); }
.global-item:nth-child(6) { background: var(--color-accent-gold-light); border-color: var(--color-accent-gold); }
.icon { font-size: var(--font-size-heading); margin-bottom: var(--spacing-xs); }
.title {
  font-family: var(--font-family-display);
  font-weight: var(--font-weight-medium);
  font-size: var(--font-size-card-title);
  color: var(--color-text-primary);
}
.desc { font-size: var(--font-size-card-body); color: var(--color-text-secondary); }
</style>