---
layout: Default
---

# 1.2 Spec-Driven Development（SDD）

<div class="sdd-definition">
<div class="sdd-title">一句话定义：规格驱动开发</div>
<div class="sdd-content">先定义"是什么"，再定义"怎么做"</div>
</div>

<div class="sdd-flow">
<div class="flow-step">规格定义</div>
<div class="arrow">→</div>
<div class="flow-step">规格评审</div>
<div class="arrow">→</div>
<div class="flow-step">规格实现</div>
<div class="arrow">→</div>
<div class="flow-step">规格验证</div>
</div>

<div class="comparison-grid">

<div class="compare-item bad">
<div class="compare-title">对话驱动</div>
<div class="compare-list">
<div class="compare-point">❌ 意图模糊，结果不可预测</div>
<div class="compare-point">❌ 需求只在聊天记录，无法沉淀</div>
<div class="compare-point">❌ 缺乏组织，难以协作</div>
</div>
</div>

<div class="compare-item good">
<div class="compare-title">规格驱动</div>
<div class="compare-list">
<div class="compare-point">✓ 可沉淀、可复用、可追溯</div>
<div class="compare-point">✓ 先定义"是什么"，再定义"怎么做"</div>
<div class="compare-point">✓ 规格文档是人机协作的"契约"</div>
</div>
</div>

</div>

<style>
.sdd-definition {
  background: #1A365D;
  padding: var(--spacing-md);
  border-radius: var(--radius-lg);
  text-align: center;
  margin-bottom: var(--spacing-md);
}
.sdd-title {
  font-family: var(--font-family-display);
  font-size: var(--font-size-card-meta);
  color: #F7FAFC;
  margin-bottom: var(--spacing-xs);
}
.sdd-content {
  font-family: var(--font-family-display);
  font-size: var(--font-size-heading);
  font-weight: var(--font-weight-semibold);
  color: #FFFFFF;
}
.sdd-flow {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: var(--spacing-xs);
  margin-bottom: var(--spacing-md);
}
.flow-step {
  padding: var(--spacing-xs) var(--spacing-md);
  background: var(--color-primary-light);
  border-radius: var(--radius-md);
  font-family: var(--font-family-display);
  font-weight: var(--font-weight-medium);
  font-size: var(--font-size-card-body);
  color: var(--color-primary);
  border: 1px solid var(--color-primary);
}
.arrow {
  color: var(--color-primary);
  font-size: var(--font-size-card-title);
}
.comparison-grid {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: var(--spacing-md);
}
.compare-item {
  padding: var(--spacing-md);
  border-radius: var(--radius-md);
}
.compare-item.bad {
  background: var(--color-warning-light);
  border: 1px solid var(--color-warning);
}
.compare-item.good {
  background: var(--color-success-light);
  border: 1px solid var(--color-success);
}
.compare-title {
  font-family: var(--font-family-display);
  font-weight: var(--font-weight-medium);
  font-size: var(--font-size-card-title);
  color: var(--color-text-primary);
  margin-bottom: var(--spacing-sm);
}
.compare-list {
  display: flex;
  flex-direction: column;
  gap: var(--spacing-xs);
}
.compare-point {
  font-size: var(--font-size-card-body);
  color: var(--color-text-primary);
}
</style>

<!--
什么是规格驱动开发？一句话：**先定义"是什么"，再定义"怎么做"**。

核心流程是：规格定义 → 规格评审 → 规格实现 → 规格验证。

**对话驱动 vs 规格驱动**

对话驱动的问题：
- 意图模糊，结果不可预测——你说了半天，AI 理解的可能完全不一样
- 需求只在聊天记录，无法沉淀——下次遇到类似问题，又要重新说一遍
- 缺乏组织，难以协作——团队成员不知道 AI 当时是怎么理解的

规格驱动的好处：
- 可沉淀、可复用、可追溯——规格文档可以保存，下次直接复用
- 先定义"是什么"，再定义"怎么做"——避免 AI 猜错方向
- 规格文档是人机协作的"契约"——人先让 AI 生成规格，评审后再执行

简单说：**对话驱动是"边说边做"，规格驱动是"先说清楚再做"。**

那么，为什么我们需要规格驱动？它具体解决了什么问题？
-->
