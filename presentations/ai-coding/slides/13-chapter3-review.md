---
layout: Default
---

# 3.3 对评审的影响

<div class="review-grid">

<div class="review-card">
<div class="review-type">需求评审</div>
<div class="review-focus">
<strong>验证AI推演结果的业务准确性</strong>
<p>AI补充的细节是否符合业务预期</p>
</div>
</div>

<div class="review-card">
<div class="review-type">Code Review</div>
<div class="review-focus">
<strong>增加AI输出质量校验环节</strong>
<p>是否符合团队规范？是否有安全隐患？</p>
</div>
</div>

<div class="review-card">
<div class="review-type">测试评审</div>
<div class="review-focus">
<strong>验证测试用例的业务意义</strong>
<p>能跑通 ≠ 有业务意义</p>
</div>
</div>

</div>

<div class="reminder">
⚠️ AI生成的代码、测试、文档都需要人工确认其"业务正确性"
</div>

<style>
.review-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 0.5rem;
  margin-top: 0.5rem;
}
.review-card {
  background: var(--color-primary-light);
  padding: 0.6rem;
  border-radius: var(--radius-sm);
}
.review-type {
  background: var(--color-primary);
  color: white;
  padding: 0.2rem 0.5rem;
  border-radius: var(--radius-sm);
  font-weight: 600;
  font-size: 0.8rem;
  display: inline-block;
}
.review-focus strong { font-size: 0.85rem; color: var(--color-text-primary); }
.review-focus p {
  font-size: 0.75rem;
  color: var(--color-text-secondary);
  margin-top: 0.2rem;
}
.reminder {
  margin-top: 0.75rem;
  padding: 0.6rem;
  background: var(--color-warning-light);
  border-radius: var(--radius-sm);
  font-size: 0.85rem;
  text-align: center;
  color: var(--color-text-primary);
}
</style>