---
layout: Default
---

# 3.4 人的工作调整

<div class="role-change">

<div class="change-item">
<span class="from">执行者</span>
<span class="arrow">→</span>
<span class="to">把关者</span>
<span class="desc">建立规则、审核输出</span>
</div>

<div class="change-item">
<span class="from">单环节</span>
<span class="arrow">→</span>
<span class="to">全流程</span>
<span class="desc">了解PM/SDE/QA各环节要求</span>
</div>

<div class="change-item">
<span class="from">自己写</span>
<span class="arrow">→</span>
<span class="to">与AI共生</span>
<span class="desc">既指导也采纳建议</span>
</div>

</div>

<div class="key-ability">
<strong>最重要的能力：建立对AI输出的校准直觉</strong>
<p>能识别出"AI正在谄媚"的场景</p>
</div>

<div class="training-path">
<div class="path-title">能力培养路线图</div>

<div class="level-row">
<div class="level-badge beginner">初级</div>
<div class="level-content">
<strong>会用工具</strong>
<p>理解四阶段工作流，能用 AI 完成单个任务</p>
<p class="practice">练习：用 AI 完成一个需求推演</p>
</div>
</div>

<div class="level-row">
<div class="level-badge intermediate">中级</div>
<div class="level-content">
<strong>能判断质量</strong>
<p>能判断 AI 输出是否符合业务预期，能写出合格的 spec 文档</p>
<p class="practice">练习：独立完成一个完整的 OpenSpec 变更</p>
</div>
</div>

<div class="level-row">
<div class="level-badge advanced">高级</div>
<div class="level-content">
<strong>能设计策略</strong>
<p>能设计上下文策略，能开发团队专属 Skill，沉淀最佳实践</p>
<p class="practice">练习：为团队开发一个 Skill</p>
</div>
</div>

</div>

<style>
.role-change {
  display: flex;
  flex-direction: column;
  gap: var(--spacing-md);
  margin-top: var(--spacing-md);
}
.change-item {
  display: flex;
  align-items: center;
  gap: var(--spacing-sm);
  padding: var(--spacing-sm);
  border-radius: var(--radius-md);
  border: 1px solid var(--color-border);
}
.change-item:nth-child(1) { background: var(--color-success-light); }
.change-item:nth-child(2) { background: var(--color-info-light); }
.change-item:nth-child(3) { background: var(--color-accent-teal-light); }
.from, .to {
  font-family: var(--font-family-display);
  font-weight: var(--font-weight-medium);
  padding: 4px 10px;
  border-radius: var(--radius-sm);
  font-size: var(--font-size-card-meta);
}
.from { background: var(--color-border); color: var(--color-text-secondary); }
.to { background: var(--color-primary); color: var(--color-bg-card); }
.arrow { color: var(--color-primary); font-size: var(--font-size-card-title); }
.desc { font-size: var(--font-size-card-body); color: var(--color-text-secondary); margin-left: var(--spacing-sm); }
.key-ability {
  margin-top: var(--spacing-lg);
  margin-bottom: var(--spacing-xl);
  padding: var(--spacing-md);
  background: #1A365D;
  border-radius: var(--radius-lg);
  text-align: center;
}
.key-ability strong { font-size: var(--font-size-card-title); color: #FFFFFF; }
.key-ability p { margin-top: var(--spacing-xs); margin-bottom: 0; font-size: var(--font-size-card-body); color: #FFFFFF; }

.training-path {
  margin-top: var(--spacing-md);
  border-radius: var(--radius-lg);
  overflow: hidden;
}
.path-title {
  background: var(--color-primary);
  color: var(--color-bg-card);
  padding: var(--spacing-sm) var(--spacing-md);
  font-weight: var(--font-weight-medium);
  font-size: var(--font-size-card-title);
}
.level-row {
  display: flex;
  align-items: stretch;
  border-bottom: 1px solid var(--color-border);
}
.level-row:last-child { border-bottom: none; }
.level-badge {
  min-width: 60px;
  padding: var(--spacing-sm);
  display: flex;
  align-items: center;
  justify-content: center;
  font-weight: var(--font-weight-semibold);
  font-size: var(--font-size-card-meta);
  color: var(--color-bg-card);
}
.level-badge.beginner { background: var(--color-success); }
.level-badge.intermediate { background: var(--color-info); }
.level-badge.advanced { background: var(--color-accent-gold); }
.level-content {
  flex: 1;
  padding: var(--spacing-sm) var(--spacing-md);
  background: var(--color-bg-subtle);
}
.level-content strong { color: var(--color-text-primary); font-size: var(--font-size-card-body); }
.level-content p { margin: var(--spacing-xs) 0 0 0; font-size: var(--font-size-card-meta); color: var(--color-text-secondary); }
.level-content .practice { color: var(--color-primary); font-weight: var(--font-weight-medium); }
</style>

<!--
最后，我们来总结一下人的角色转变：

**从执行者到把关者**

以前你是写代码的人，现在你是审核代码的人。你需要建立规则、审核输出，确保 AI 的产出符合预期。

**从单环节到全流程**

你需要了解研发全流程的要求。以前可能只关注自己的环节，现在需要对 PM、SDE、QA 各环节都有所了解。

**与AI共生**

既给予指导，也采纳建议。AI 可能会给你一些你没想到的方案，要有开放的心态去评估。

**建立对AI输出的校准直觉**

这是最重要的能力。你需要能识别出"AI 正在谄媚"的场景。当 AI 给出一个看起来很合理的建议时，要有直觉去判断：这个方向对不对？

**能力培养路线图**

我给大家规划了三个阶段的能力培养路径：

- **初级**：理解四阶段工作流，能用 AI 完成单个任务。练习方式：用 AI 完成一个需求推演。
- **中级**：能判断 AI 输出质量，能写出合格的 spec 文档。练习方式：独立完成一个完整的 OpenSpec 变更。
- **高级**：能设计上下文策略，能开发团队专属 Skill。练习方式：为团队开发一个 Skill。

培训结束后，建议你从初级开始，一步步提升。
-->