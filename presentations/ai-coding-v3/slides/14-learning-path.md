---
layout: Default
---

# 2.4 学习路径指引

<div class="learning-path">

<div class="level">
<div class="level-header">
<span class="level-num">01</span>
<span class="level-title">初级：会用工具</span>
</div>
<div class="level-body">
<div class="level-check">✓ 了解工作流和安装相关工具</div>
<div class="level-check">✓ 理解四阶段工作流</div>
<div class="level-check">✓ 能用 AI 完成单个任务</div>
</div>
</div>

<div class="level">
<div class="level-header">
<span class="level-num">02</span>
<span class="level-title">中级：能判质量</span>
</div>
<div class="level-body">
<div class="level-check">✓ 参考变更案例，独立完成简单变更</div>
<div class="level-check">✓ 能判断 AI 输出是否符合业务预期</div>
<div class="level-check">✓ 能写出合格的 spec 文档</div>
</div>
</div>

<div class="level">
<div class="level-header">
<span class="level-num">03</span>
<span class="level-title">高级：能设计策略</span>
</div>
<div class="level-body">
<div class="level-check">✓ 开发团队专属 Skill，沉淀最佳实践</div>
<div class="level-check">✓ 能设计上下文策略</div>
<div class="level-check">✓ 能指导他人使用 AI Coding</div>
</div>
</div>

</div>

<div class="resources">
<strong>学习资源指引：</strong>
<ul>
<li>Superpowers 完全指南（workspace/ai-coding/drafts/）</li>
<li>OpenSpec 完全指南（workspace/ai-coding/drafts/）</li>
<li>Claude Code 官方文档</li>
</ul>
</div>

<style>
.learning-path {
  display: flex;
  flex-direction: column;
  gap: var(--spacing-md);
  margin: var(--spacing-md) 0;
}
.level {
  border-radius: var(--radius-md);
  padding: var(--spacing-md);
  border: 1px solid var(--color-border);
}
.level:nth-child(1) { background: var(--color-success-light); border-color: var(--color-success); }
.level:nth-child(2) { background: var(--color-info-light); border-color: var(--color-info); }
.level:nth-child(3) { background: var(--color-accent-teal-light); border-color: var(--color-accent-teal); }
.level-header {
  display: flex;
  align-items: center;
  gap: var(--spacing-sm);
  margin-bottom: var(--spacing-sm);
}
.level-num {
  font-family: var(--font-family-display);
  width: 28px;
  height: 28px;
  border-radius: var(--radius-sm);
  display: flex;
  align-items: center;
  justify-content: center;
  font-weight: var(--font-weight-semibold);
  font-size: 14px;
  background: var(--color-primary);
  color: var(--color-bg-card);
}
.level:nth-child(1) .level-num { background: var(--color-success); }
.level:nth-child(2) .level-num { background: var(--color-info); }
.level:nth-child(3) .level-num { background: var(--color-accent-teal); }
.level-title {
  font-family: var(--font-family-display);
  font-weight: var(--font-weight-semibold);
  font-size: var(--font-size-card-title);
  color: var(--color-text-primary);
}
.level-body {
  display: flex;
  flex-direction: column;
  gap: var(--spacing-xs);
}
.level-check {
  font-size: var(--font-size-card-body);
  color: var(--color-text-primary);
}
.resources {
  margin-top: var(--spacing-lg);
  padding: var(--spacing-md);
  background: var(--color-accent-orange-light);
  border-radius: var(--radius-md);
  border: 1px solid var(--color-accent-orange);
  font-size: var(--font-size-card-body);
}
.resources ul {
  margin-top: var(--spacing-xs);
  margin-left: var(--spacing-md);
}
.resources li {
  margin-bottom: var(--spacing-xs);
}
</style>

<!--
学习 AI Coding 需要一个循序渐进的过程，我把它分为三个阶段。

**初级：会用工具**

这个阶段的目标是入门。你需要：
- 了解工作流和安装相关工具
- 理解四阶段工作流
- 能用 AI 完成单个任务

**中级：能判质量**

这个阶段的目标是独立工作。你需要：
- 参考变更案例，独立完成简单变更
- 能判断 AI 输出是否符合业务预期
- 能写出合格的 spec 文档

**高级：能设计策略**

这个阶段的目标是沉淀和分享。你需要：
- 开发团队专属 Skill，沉淀最佳实践
- 能设计上下文策略
- 能指导他人使用 AI Coding

**学习资源**

- Superpowers 完全指南（workspace/ai-coding/drafts/）
- OpenSpec 完全指南（workspace/ai-coding/drafts/）
- Claude Code 官方文档

根据自己的水平，选择合适的学习路径。
-->
