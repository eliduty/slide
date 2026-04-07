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
  gap: 0.5rem;
  margin-top: 0.5rem;
}
.global-item {
  background: var(--color-primary-light);
  padding: 0.6rem;
  border-radius: var(--radius-sm);
  text-align: center;
}
.icon { font-size: 1.2rem; margin-bottom: 0.2rem; }
.title { font-weight: 600; font-size: 0.85rem; color: var(--color-text-primary); }
.desc { font-size: 0.7rem; color: var(--color-text-secondary); }
</style>