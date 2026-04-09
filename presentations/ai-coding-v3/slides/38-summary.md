---
layout: Default
---

# 总结

<div class="summary-grid">

<div class="summary-item">
<div class="num">01</div>
<div class="content">
<strong>AI 不是万能的</strong>
<p>擅长代码生成，不擅长业务理解</p>
<p class="key">决策在人，执行在AI</p>
</div>
</div>

<div class="summary-item">
<div class="num">02</div>
<div class="content">
<strong>工作流要标准化</strong>
<p>需求、设计、实现三阶段</p>
<p class="key">明确进入条件和产出物</p>
</div>
</div>

<div class="summary-item">
<div class="num">03</div>
<div class="content">
<strong>角色在转变</strong>
<p>从执行者到把关者</p>
<p class="key">建立对AI输出的校准直觉</p>
</div>
</div>

<div class="summary-item">
<div class="num">04</div>
<div class="content">
<strong>场景要灵活应对</strong>
<p>遗留项目和新项目不同策略</p>
<p class="key">核心是处理好上下文</p>
</div>
</div>

</div>

<style>
.summary-grid {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: var(--spacing-md);
  margin-top: var(--spacing-md);
}
.summary-item {
  padding: var(--spacing-md);
  border-radius: var(--radius-md);
  display: flex;
  gap: var(--spacing-md);
  border: 1px solid;
}
.summary-item:nth-child(1) { background: var(--color-info-light); border-color: var(--color-info); }
.summary-item:nth-child(2) { background: var(--color-success-light); border-color: var(--color-success); }
.summary-item:nth-child(3) { background: var(--color-warning-light); border-color: var(--color-warning); }
.summary-item:nth-child(4) { background: var(--color-accent-teal-light); border-color: var(--color-accent-teal); }
.num {
  font-family: var(--font-family-display);
  width: 32px;
  height: 32px;
  border-radius: var(--radius-sm);
  display: flex;
  align-items: center;
  justify-content: center;
  font-weight: var(--font-weight-semibold);
  font-size: var(--font-size-card-meta);
}
.summary-item:nth-child(1) .num { background: var(--color-info); color: var(--color-bg-card); }
.summary-item:nth-child(2) .num { background: var(--color-success); color: var(--color-bg-card); }
.summary-item:nth-child(3) .num { background: var(--color-warning); color: var(--color-bg-card); }
.summary-item:nth-child(4) .num { background: var(--color-accent-teal); color: var(--color-bg-card); }
.content strong {
  font-family: var(--font-family-display);
  font-size: var(--font-size-card-title);
  color: var(--color-text-primary);
}
.content p { font-size: var(--font-size-card-body); color: var(--color-text-secondary); margin: var(--spacing-xs) 0; }
.content .key { color: var(--color-primary); font-weight: var(--font-weight-medium); }
</style>

<!--
好，今天的培训就到这里。我来做最后总结：

**1. AI 不是万能的**——它擅长代码生成，不擅长业务理解。决策在人，执行在AI。

**2. 工作流要标准化**——需求、设计、环境规范、实现四阶段，每个阶段有明确的进入条件和产出物。

**3. 角色在转变**——从执行者到把关者，需要建立对 AI 输出的校准直觉。

**4. 场景要灵活应对**——遗留项目和新项目有不同的策略，核心是处理好上下文。

培训资料我已经整理好了，放在 workspace/ai-coding/ 目录下。有问题随时找我交流。

谢谢大家！
-->