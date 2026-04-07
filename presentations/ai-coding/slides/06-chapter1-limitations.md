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
  gap: 0.5rem;
}
.limit-item {
  display: flex;
  gap: 0.5rem;
  padding: 0.5rem;
  background: var(--color-primary-light);
  border-radius: var(--radius-sm);
}
.icon { font-size: 1.2rem; }
.limit-item p {
  font-size: 0.8rem;
  color: var(--color-text-secondary);
  margin: 0;
}
.question-box {
  background: var(--color-info-light);
  padding: 1rem;
  border-radius: var(--radius-lg);
  border: 2px solid var(--color-primary);
}
.answer {
  font-size: 0.9rem;
  color: var(--color-primary);
  margin-top: 0.5rem;
}
.hint {
  font-size: 0.8rem;
  color: var(--color-text-secondary);
  margin-top: 0.3rem;
}
</style>