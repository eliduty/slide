---
layout: Default
---

# 1.3 为什么需要SDD

<div class="reason-grid">

<div class="reason-item">
<div class="reason-num reason-num-1">01</div>
<div class="reason-title">意图清晰化</div>
<div class="reason-desc">规格文档把模糊的想法变成明确的定义，AI 不再猜测</div>
</div>

<div class="reason-item">
<div class="reason-num reason-num-2">02</div>
<div class="reason-title">知识可沉淀</div>
<div class="reason-desc">规格文档可以保存、复用、传承，不再是"一次性对话"</div>
</div>

<div class="reason-item">
<div class="reason-num reason-num-3">03</div>
<div class="reason-title">协作可追溯</div>
<div class="reason-desc">团队成员可以看到 AI 当时的理解，知道为什么这样做</div>
</div>

<div class="reason-item">
<div class="reason-num reason-num-4">04</div>
<div class="reason-title">质量可验证</div>
<div class="reason-desc">有了规格，就有了验收标准，AI 输出可以对照检查</div>
</div>

</div>

<div class="transition-note">
<strong>演进路径：</strong> 对话驱动 → Plan 模式 → Spec 驱动<br/>
<span class="sub-note">对话驱动的问题让大家意识到：需要把对话内容文档化才能有效复用</span>
</div>

<style>
.reason-grid {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: var(--spacing-md);
  margin-top: var(--spacing-md);
}
.reason-item {
  padding: var(--spacing-md);
  border-radius: var(--radius-md);
  border: 1px solid var(--color-border);
  background: var(--color-bg-subtle);
  display: flex;
  gap: var(--spacing-md);
}
.reason-num {
  font-family: var(--font-family-display);
  font-weight: var(--font-weight-semibold);
  font-size: var(--font-size-heading);
  min-width: 40px;
}
.reason-num-1 {
  color: #C05621;
}
.reason-num-2 {
  color: #0D9488;
}
.reason-num-3 {
  color: #E11D48;
}
.reason-num-4 {
  color: #B7791F;
}
.reason-title {
  font-family: var(--font-family-display);
  font-weight: bold;
  font-size: var(--font-size-card-title);
  color: var(--color-text-primary);
  margin-bottom: var(--spacing-xs);
}
.reason-desc {
  font-size: var(--font-size-card-body);
  color: var(--color-text-secondary);
}
.transition-note {
  margin-top: var(--spacing-lg);
  padding: var(--spacing-md);
  background: var(--color-accent-teal-light);
  border-radius: var(--radius-md);
  border: 1px solid var(--color-accent-teal);
  font-size: var(--font-size-card-body);
  color: var(--color-text-primary);
}
.sub-note {
  font-size: var(--font-size-card-meta);
  color: var(--color-text-secondary);
  margin-top: var(--spacing-xs);
  display: block;
}
</style>

<!--
为什么需要规格驱动？四个核心价值：

**01. 意图清晰化**

规格文档把模糊的想法变成明确的定义。你心里想的是"做一个用户管理模块"，但 AI 可能理解成各种样子。规格文档就是把这想法写清楚，AI 不再猜测。

**02. 知识可沉淀**

对话驱动的问题是：聊完了就没了。下次遇到类似问题，又要重新说一遍。规格文档可以保存、复用、传承。

**03. 协作可追溯**

团队成员可以看到 AI 当时的理解，知道为什么这样做。而不是"AI 当时说要这样做，我也不知道为什么"。

**04. 质量可验证**

有了规格，就有了验收标准。AI 输出的东西，可以对照规格检查——是否符合定义、是否满足要求。

**演进路径**：对话驱动 → Plan 模式 → Spec 驱动

对话驱动的问题让大家意识到，需要把对话内容文档化才能有效复用。这就是为什么规格驱动成为主流范式。

明白了规格驱动的价值，接下来我们来看具体的人机协作边界。
-->
