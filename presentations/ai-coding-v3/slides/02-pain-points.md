---
layout: Default
---

# 你是否遇到过这些问题？

<div class="pain-grid">

<div class="pain-item">
<div class="pain-icon">❌</div>
<div class="pain-title">代码不符合项目规范</div>
<div class="pain-desc">AI 生成的代码风格、命名、结构与团队习惯不一致</div>
</div>

<div class="pain-item">
<div class="pain-icon">❌</div>
<div class="pain-title">不理解项目架构</div>
<div class="pain-desc">AI 不知道模块边界、依赖关系，改一处忘多处</div>
</div>

<div class="pain-item">
<div class="pain-icon">❌</div>
<div class="pain-title">代码难以维护</div>
<div class="pain-desc">AI 写的代码看似能跑，但缺少抽象、边界处理不当</div>
</div>

</div>

<div class="root-cause">
<strong>问题根源：</strong>缺乏上下文理解 + 没有结构化工作流 + 缺乏规范约束
</div>

<style>
.pain-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: var(--spacing-md);
  margin-top: var(--spacing-md);
}
.pain-item {
  padding: var(--spacing-md);
  border-radius: var(--radius-md);
  border: 1px solid var(--color-border);
  text-align: center;
}
.pain-item:nth-child(1) { background: var(--color-warning-light); border-color: var(--color-warning); }
.pain-item:nth-child(2) { background: var(--color-warning-light); border-color: var(--color-warning); }
.pain-item:nth-child(3) { background: var(--color-warning-light); border-color: var(--color-warning); }
.pain-icon {
  font-size: 32px;
  margin-bottom: var(--spacing-xs);
}
.pain-title {
  font-family: var(--font-family-display);
  font-weight: var(--font-weight-medium);
  font-size: var(--font-size-card-title);
  color: var(--color-text-primary);
  margin-bottom: var(--spacing-xs);
}
.pain-desc {
  font-size: var(--font-size-card-body);
  color: var(--color-text-secondary);
}
.root-cause {
  margin-top: var(--spacing-lg);
  padding: var(--spacing-md);
  background: var(--color-error-light);
  border-radius: var(--radius-md);
  border-left: 4px solid var(--color-error);
  font-size: var(--font-size-card-body);
  color: var(--color-text-primary);
}
</style>

<!--
我相信我们现在已经很多伙伴已经在vibe coding 、vibe design,但是，你是否遇到过这些问题？

**第一个问题：代码不符合项目规范**

你让 AI 帮你写一个组件，它写出来的代码风格、命名习惯、目录结构，跟你们团队的不一样。你还得花时间去调整。

**第二个问题：不理解项目架构**

你让 AI 改一个功能，它改了这个模块，但忘了更新依赖它的其他模块。为什么？因为它不理解你们项目的模块边界和依赖关系。

**第三个问题：代码难以维护**

AI 写的代码看起来能跑，但缺少抽象、边界处理不好，后续维护起来很痛苦。

这三个问题，我相信很多人都遇到过。

**那问题的根源是什么？**

不是 AI 不够聪明，而是三个原因：
1. 缺乏上下文理解——AI 不知道你的项目背景
2. 没有结构化工作流——每次都是"临时起意"式的对话
3. 缺乏规范约束——AI 不知道你们团队的"规矩"

今天分享的核心目的，就是解决这三个问题。

接下来，我们先看看行业正在经历什么样的变化。
-->
