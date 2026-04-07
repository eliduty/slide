---
layout: TwoCols
---

::left::

# 1.3 局限性是什么

<div class="limitations">

<div class="limit-item">
<div class="icon">🎭</div>
<div>
<strong>AI 会"谄媚"</strong>
<p>给出看起来合理的建议，但方向完全错误</p>
</div>
</div>

<div class="limit-item">
<div class="icon">📦</div>
<div>
<strong>上下文有限</strong>
<p>无法理解百万行代码的隐式依赖</p>
</div>
</div>

<div class="limit-item">
<div class="icon">🎯</div>
<div>
<strong>缺乏业务直觉</strong>
<p>不理解代码背后的业务意图</p>
</div>
</div>

</div>

::right::

<div class="question-box">
<strong>当 AI 做不好时，人应该怎么接管？</strong>

<p class="answer">这是今天培训的核心问题</p>

<p class="hint">接下来的章节将详细讲解"人做什么、AI做什么"的边界</p>
</div>

<style>
.limitations {
  display: flex;
  flex-direction: column;
  gap: var(--spacing-md);
}
.limit-item {
  display: flex;
  gap: var(--spacing-sm);
  padding: var(--spacing-sm);
  border-radius: var(--radius-md);
  border: 1px solid;
}
.limit-item:nth-child(1) { background: var(--color-warning-light); border-color: var(--color-warning); }
.limit-item:nth-child(2) { background: var(--color-error-light); border-color: var(--color-error); }
.limit-item:nth-child(3) { background: var(--color-info-light); border-color: var(--color-info); }
.icon { font-size: var(--font-size-heading); }
.limit-item p {
  font-size: var(--font-size-card-body);
  color: var(--color-text-secondary);
  margin: 0;
}
.question-box {
  background: var(--color-bg-subtle);
  padding: var(--spacing-lg);
  border-radius: var(--radius-lg);
  border: 2px solid var(--color-primary);
}
.answer {
  font-size: var(--font-size-card-title);
  color: var(--color-primary);
  margin-top: var(--spacing-sm);
}
.hint {
  font-size: var(--font-size-card-body);
  color: var(--color-text-secondary);
  margin-top: var(--spacing-sm);
}
</style>