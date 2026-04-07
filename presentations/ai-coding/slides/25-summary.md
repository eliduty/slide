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
  gap: 0.5rem;
  margin-top: 0.5rem;
}
.summary-item {
  background: var(--color-primary-light);
  padding: 0.6rem;
  border-radius: var(--radius-sm);
  display: flex;
  gap: 0.5rem;
}
.num {
  background: var(--color-primary);
  color: white;
  width: 26px;
  height: 26px;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  font-weight: 600;
  font-size: 0.75rem;
}
.content strong { font-size: 0.9rem; color: var(--color-text-primary); }
.content p { font-size: 0.8rem; color: var(--color-text-secondary); margin: 0.1rem 0; }
.content .key { color: var(--color-primary); font-weight: 500; }
</style>