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

<!--
说到局限性，有三个点一定要记住：

**第一，AI 会"谄媚"。**

什么叫谄媚？就是它给出一个看起来很合理的建议，但方向完全是错的。你问它"这个功能应该怎么做"，它会给你一套方案，代码看起来很漂亮，但你仔细一看，根本不符合业务需求。它不会告诉你"我不懂你的业务"，它会硬着头皮给出一个答案。

**第二，AI 的上下文有限。**

百万行代码的项目，不可能一次性喂给 AI。它看不到全局，就理解不了隐式依赖。所以大型遗留项目，AI 用起来要特别小心。

**第三，AI 缺乏业务直觉。**

它不理解代码背后的业务意图。它看到一段代码，只能从语法层面理解，不能从业务层面理解。这个差距，必须由人来弥补。

**那当 AI 做不好的时候，人应该怎么接管？**

这个问题是今天培训的核心。接下来的章节，我们会详细讲"人做什么、AI 做什么"的边界。
-->