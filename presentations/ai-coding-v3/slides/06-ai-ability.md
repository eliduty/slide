---
layout: Default
---

# 1.1 AI 能力等级

<div class="ability-grid">

<div class="ability-item strong">
<div class="level">强</div>
<div class="title">代码生成</div>
<div class="desc">Vue组件、接口实现、配置文件</div>
<div class="condition">需清晰规范</div>
</div>

<div class="ability-item guided">
<div class="level">需人引导</div>
<div class="title">架构决策</div>
<div class="desc">技术选型、模块划分</div>
<div class="condition">明确约束</div>
</div>

<div class="ability-item risky">
<div class="level">有风险</div>
<div class="title">跨模块重构</div>
<div class="desc">依赖梳理、影响分析</div>
<div class="condition">小步验证</div>
</div>

<div class="ability-item dependent">
<div class="level">依赖上下文</div>
<div class="title">业务逻辑理解</div>
<div class="desc">领域模型、业务规则</div>
<div class="condition">上下文质量</div>
</div>

</div>

<div class="key-point">
<strong>核心结论：</strong> AI 不是万能的，也不是无用的。关键在于用在什么地方。
</div>

<style>
.ability-grid {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: var(--spacing-md);
  margin-top: var(--spacing-md);
}
.ability-item {
  padding: var(--spacing-md);
  border-radius: var(--radius-md);
  border: 1px solid var(--color-border);
  text-align: center;
}
.ability-item:nth-child(1) { background: var(--color-success-light); border-color: var(--color-success); }
.ability-item:nth-child(2) { background: var(--color-info-light); border-color: var(--color-info); }
.ability-item:nth-child(3) { background: var(--color-warning-light); border-color: var(--color-warning); }
.ability-item:nth-child(4) { background: var(--color-bg-subtle); border-color: var(--color-text-muted); }
.level {
  font-family: var(--font-family-display);
  font-weight: var(--font-weight-semibold);
  margin-bottom: var(--spacing-xs);
  padding: 4px 12px;
  border-radius: var(--radius-sm);
  font-size: var(--font-size-card-meta);
}
.strong .level { background: var(--color-success); color: var(--color-bg-card); }
.guided .level { background: var(--color-info); color: var(--color-bg-card); }
.risky .level { background: var(--color-warning); color: var(--color-bg-card); }
.dependent .level { background: var(--color-text-muted); color: var(--color-bg-card); }
.title {
  font-family: var(--font-family-display);
  font-weight: var(--font-weight-medium);
  font-size: var(--font-size-card-title);
  color: var(--color-text-primary);
}
.desc { font-size: var(--font-size-card-body); color: var(--color-text-secondary); }
.condition { font-size: var(--font-size-card-meta); color: var(--color-text-muted); margin-top: var(--spacing-xs); }
.key-point {
  margin-top: var(--spacing-lg);
  padding: var(--spacing-md);
  background: var(--color-accent-orange-light);
  border-radius: var(--radius-md);
  border-left: 4px solid var(--color-accent-orange);
  font-size: var(--font-size-card-body);
  color: var(--color-text-primary);
}
</style>

<!--
我们根据实践经验，把 AI 的能力分成了四个等级：

**第一类：代码生成——强**

这是 AI 最擅长的领域。比如生成 Vue 组件、写接口实现、配置文件。只要你给的规范清晰，输出质量是非常高的。在项目中，我们大量使用 AI 生成前端组件，效率提升非常明显，实际上我们职业素养的项目的代码是100% AI生成。

**第二类：架构决策——需要人引导**

AI 可以帮你做架构设计，但前提是你得给它明确的约束。比如技术选型、模块划分，你得先告诉它：我们用什么技术栈、有什么约束条件。有了这些约束，AI 才能给出合理的方案。没有约束，它就会按自己的"审美"来，可能完全不符合团队习惯。

**第三类：跨模块重构——有风险**

这个要特别小心。AI 很擅长生成重构后的代码，但它很容易忽略隐式依赖。改了 A 模块，但没有同步更新 B 模块中依赖 A 的地方。所以跨模块重构，必须小步验证，每一步都要人工确认。

**第四类：业务逻辑理解——依赖上下文质量**

这是 AI 最弱的环节。它不理解代码背后的业务意图，只能根据上下文去"猜"。上下文给得好，猜得就准；上下文给得差，输出就会偏离。

**核心结论：用在什么地方决定效果。**

刚刚我们也说到AI在理解业务逻辑是他最弱的环境，那么如何解决呢？现阶段的答案就是“规格驱动开发”。
-->
