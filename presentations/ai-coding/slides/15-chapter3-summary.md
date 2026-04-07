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
-->