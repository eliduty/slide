---
layout: Default
---

# 3.9 贯穿全局的应用总结

<div class="app-grid">

<div class="app-item">
<div class="app-header"><span class="app-num">01</span> <span class="app-title">知识规范化陈述</span></div>
<div class="app-desc">文档结构标准化，让 AI 能理解和复用</div>
</div>

<div class="app-item">
<div class="app-header"><span class="app-num">02</span> <span class="app-title">上下文渐进式披露</span></div>
<div class="app-desc">按需披露，不是所有信息都一次性给 AI</div>
</div>

<div class="app-item">
<div class="app-header"><span class="app-num">03</span> <span class="app-title">设计与实现评审</span></div>
<div class="app-desc">AI 辅助发现潜在问题，最终评审权在人</div>
</div>

<div class="app-item">
<div class="app-header"><span class="app-num">04</span> <span class="app-title">安全审计</span></div>
<div class="app-desc">AI 发现常见安全问题，审计仍需人工</div>
</div>

<div class="app-item">
<div class="app-header"><span class="app-num">05</span> <span class="app-title">版本控制联动</span></div>
<div class="app-desc">OpenSpec 变更管理与 git 分支策略</div>
</div>

<div class="app-item">
<div class="app-header"><span class="app-num">06</span> <span class="app-title">上下文工程标准化</span></div>
<div class="app-desc">Harness Engineering 核心：可复用资产沉淀</div>
</div>

</div>

<div class="bottom-row">
<div class="output-box">
<strong>核心产出：</strong>CLAUDE.md + rules + 可复用资产
</div>
<div class="tool-box">
<strong>配合工具：</strong>OpenSpec archive + Superpowers
</div>
</div>

<div class="key-point">
<strong>关键原则：</strong>这些实践贯穿整个开发流程，不是某个阶段专属
</div>

<style>
.app-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: var(--spacing-sm);
  margin-top: var(--spacing-sm);
}
.app-item {
  padding: var(--spacing-sm);
  border-radius: var(--radius-md);
  border: 1px solid var(--color-border);
  background: var(--color-bg-subtle);
  text-align: center;
}
.app-header {
  display: flex;
  align-items: center;
  gap: 8px;
  margin-bottom: 10px;
}
.app-num {
  font-family: var(--font-family-display);
  font-weight: var(--font-weight-semibold);
  font-size: 18px;
  color: var(--color-warning);
}
.app-title {
  font-family: var(--font-family-display);
  font-weight: var(--font-weight-medium);
  font-size: 18px;
  color: var(--color-text-primary);
}
.app-desc {
  font-size: 14px;
  color: var(--color-text-secondary);
  line-height: 1.3;
}
.bottom-row {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: var(--spacing-sm);
  margin-top: var(--spacing-sm);
}
.output-box {
  padding: var(--spacing-sm);
  background: var(--color-primary-light);
  border-radius: var(--radius-md);
  font-size: 13px;
}
.tool-box {
  padding: var(--spacing-sm);
  background: var(--color-accent-gold-light);
  border-radius: var(--radius-md);
  font-size: 13px;
}
.key-point {
  margin-top: var(--spacing-md);
  padding: var(--spacing-sm) var(--spacing-md);
  background: var(--color-accent-orange-light);
  border-radius: var(--radius-md);
  border: 1px solid var(--color-accent-orange);
  text-align: center;
  font-size: 14px;
}
</style>

<!--
例如：

**知识规范化陈述**
文档结构标准化、命名规范统一、术语定义清晰，让 AI 能理解和复用项目知识。

**上下文渐进式披露**
不是所有信息都要一次性给 AI，制定规范（spec），按需披露，控制上下文范围。

**设计与实现评审**
AI 辅助评审发现潜在问题，但最终评审权在人——深层次的业务逻辑问题仍需人工判断。

**安全审计**
AI 可以发现常见的安全问题，但不能替代专业安全审计，最终安全责任还是在人。

**版本控制联动**
OpenSpec 变更管理如何与 git 分支策略结合，适配 AI Coding 工作流。

**上下文工程标准化**
Harness Engineering 的核心：上下文组织的标准化实践，形成可复用资产。

**核心原则**：这些实践贯穿整个开发流程，不是某个阶段专属。

好，到这里我们完整介绍了 AI Coding 的四阶段工作流程和贯穿全局的实践方法。四阶段工作流程讲完了，大家可能会问：这套流程对现有的工作方式会有什么改变？接下来我们看第四部分——对 PM、SDE、QA 工作的影响。
-->
