---
layout: Default
---

# 3.9 贯穿全局——工具应用

<div class="global-grid">

<div class="global-item">
<div class="global-title">知识规范化陈述</div>
<div class="global-desc">合理组织项目知识，让 AI 能理解和复用</div>
</div>

<div class="global-item">
<div class="global-title">上下文渐进式披露</div>
<div class="global-desc">制定规范（spec），控制上下文披露范围</div>
</div>

<div class="global-item">
<div class="global-title">设计与实现评审</div>
<div class="global-desc">AI 辅助评审，发现潜在问题和改进点</div>
</div>

<div class="global-item">
<div class="global-title">安全审计</div>
<div class="global-desc">检查代码中的安全漏洞和风险点</div>
</div>

<div class="global-item">
<div class="global-title">版本控制联动</div>
<div class="global-desc">分支治理策略调整，适配 AI Coding 工作流</div>
</div>

<div class="global-item">
<div class="global-title">上下文工程标准化</div>
<div class="global-desc">上下文组织的标准化实践，形成可复用资产</div>
</div>

</div>

<style>
.global-grid {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: var(--spacing-md);
  margin-top: var(--spacing-md);
}
.global-item {
  padding: var(--spacing-md);
  border-radius: var(--radius-md);
  border: 1px solid var(--color-border);
  background: var(--color-bg-subtle);
}
.global-title {
  font-family: var(--font-family-display);
  font-weight: var(--font-weight-medium);
  font-size: var(--font-size-card-title);
  color: var(--color-text-primary);
  margin-bottom: var(--spacing-xs);
}
.global-desc {
  font-size: var(--font-size-card-body);
  color: var(--color-text-secondary);
}
</style>

<!--
贯穿全局的工具应用：

**知识规范化陈述**

合理组织项目知识，让 AI 能理解和复用。这是上下文工程的基础。

**上下文渐进式披露**

制定规范（spec），控制上下文披露范围。不是所有信息都要给 AI，要根据任务筛选。

**设计与实现评审**

AI 辅助评审，发现潜在问题和改进点。但最终评审权在人。

**安全审计**

检查代码中的安全漏洞和风险点。AI 可以发现常见的安全问题，但不能替代专业安全审计。

**版本控制联动**

分支治理策略调整，适配 AI Coding 工作流。比如 OpenSpec 的变更管理如何与 git 分支策略结合。

**上下文工程标准化**

上下文组织的标准化实践，形成可复用资产。这是 Harness Engineering 的核心。

以上就是四阶段工作流程的全部内容。让我们来做个总结。
-->