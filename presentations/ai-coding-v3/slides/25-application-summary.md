---
layout: Default
---

# 3.10 贯穿全局应用总结

<div class="summary-grid">

<div class="summary-card">
<div class="card-title">知识规范化陈述</div>
<div class="card-desc">合理组织项目知识，让 AI 能理解和复用</div>
</div>

<div class="summary-card">
<div class="card-title">上下文渐进式披露</div>
<div class="card-desc">制定规范（spec），控制上下文披露范围</div>
</div>

<div class="summary-card">
<div class="card-title">设计与实现评审</div>
<div class="card-desc">AI 辅助评审，发现潜在问题</div>
</div>

<div class="summary-card">
<div class="card-title">安全审计</div>
<div class="card-desc">检查代码中的安全漏洞和风险点</div>
</div>

<div class="summary-card">
<div class="card-title">版本控制联动</div>
<div class="card-desc">分支治理策略调整</div>
</div>

<div class="summary-card">
<div class="card-title">上下文工程标准化</div>
<div class="card-desc">形成可复用资产</div>
</div>

</div>

<div class="key-point">
<strong>关键原则：</strong>这些实践贯穿整个开发流程，不是某个阶段专属
</div>

<style>
.summary-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: var(--spacing-md);
  margin: var(--spacing-lg) 0;
}
.summary-card {
  background: var(--color-bg-card);
  border: 1px solid var(--color-border);
  border-radius: var(--radius-md);
  padding: var(--spacing-md);
  text-align: center;
}
.card-title {
  font-family: var(--font-family-display);
  font-weight: var(--font-weight-semibold);
  font-size: var(--font-size-card-title);
  color: var(--color-primary);
  margin-bottom: var(--spacing-xs);
}
.card-desc {
  font-size: var(--font-size-card-meta);
  color: var(--color-text-secondary);
  line-height: 1.5;
}
.key-point {
  margin-top: var(--spacing-lg);
  padding: var(--spacing-md);
  background: var(--color-accent-orange-light);
  border-radius: var(--radius-md);
  border: 1px solid var(--color-accent-orange);
  text-align: center;
  font-size: var(--font-size-card-body);
}
</style>

<!--
除了四阶段的工作流程，还有一些实践是贯穿整个开发流程的。

**知识规范化陈述**

合理组织项目知识，让 AI 能理解和复用。这包括：
- 文档结构标准化
- 命名规范统一
- 术语定义清晰

**上下文渐进式披露**

制定规范（spec），控制上下文披露范围。不是所有信息都要一次性给 AI，而是按需披露。

**设计与实现评审**

AI 辅助评审，发现潜在问题。但要注意：AI 发现的只是表面问题，深层次的业务逻辑问题还需要人来判断。

**安全审计**

检查代码中的安全漏洞和风险点。AI 可以帮你扫描常见的安全问题，但最终的安全责任还是在人。

**版本控制联动**

分支治理策略调整。AI Coding 改变了提交频率和提交粒度，需要相应调整分支策略。

**上下文工程标准化**

形成可复用资产。把项目中积累的经验沉淀为标准化的配置和规则。

这些实践不是某个阶段专属的，而是贯穿整个开发流程的。
-->
