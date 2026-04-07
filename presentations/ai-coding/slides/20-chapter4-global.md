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

<!--
有一些工作贯穿整个流程：

**项目知识规范化陈述**

我们用 CLAUDE.md 文件来定义项目规则。这个文件是 AI 理解项目的入口，它会告诉 AI：我们用什么技术栈、有什么约定、禁止做什么。

**上下文渐进式披露**

也叫 harness engineering。就是知道在什么时机给 AI 什么信息。开始时给架构背景，设计时给需求细节，实现时给技术规范。

**设计与实现的评价评审**

AI 可以帮你 review 代码、设计方案。但最终决策必须由人来做出。

**安全审计**

AI 可以扫描代码中的安全漏洞，比如 SQL 注入、XSS。但我们有一个规则文件：`rules/api-security.md`，定义了安全规范，AI 会根据这个规范来检查。

**版本控制联动**

分支治理怎么调整？我们有一个 `finishing-a-development-branch` Skill，告诉你分支完成后应该做什么：测试、评审、合并。

**Skills体系**

沉淀最佳实践，形成可复用的知识库。
-->