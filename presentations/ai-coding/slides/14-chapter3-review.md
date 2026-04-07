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
  gap: var(--spacing-md);
  margin-top: var(--spacing-md);
}
.review-card {
  padding: var(--spacing-md);
  border-radius: var(--radius-md);
  border: 1px solid;
}
.review-card:nth-child(1) { background: var(--color-info-light); border-color: var(--color-info); }
.review-card:nth-child(2) { background: var(--color-success-light); border-color: var(--color-success); }
.review-card:nth-child(3) { background: var(--color-warning-light); border-color: var(--color-warning); }
.review-type {
  padding: 4px 12px;
  border-radius: var(--radius-sm);
  font-weight: var(--font-weight-medium);
  font-size: var(--font-size-card-meta);
  display: inline-block;
}
.review-card:nth-child(1) .review-type { background: var(--color-info); color: var(--color-bg-card); }
.review-card:nth-child(2) .review-type { background: var(--color-success); color: var(--color-bg-card); }
.review-card:nth-child(3) .review-type { background: var(--color-warning); color: var(--color-bg-card); }
.review-focus strong { font-size: var(--font-size-card-title); color: var(--color-text-primary); }
.review-focus p {
  font-size: var(--font-size-card-body);
  color: var(--color-text-secondary);
  margin-top: var(--spacing-xs);
}
.reminder {
  margin-top: var(--spacing-lg);
  padding: var(--spacing-md);
  background: var(--color-accent-rose-light);
  border-radius: var(--radius-md);
  font-size: var(--font-size-card-body);
  text-align: center;
  color: var(--color-text-primary);
  border: 1px solid var(--color-accent-rose);
}
</style>

<!--
**需求评审**

重点是验证 AI 推演结果的业务准确性。AI 可能帮你补充了一些需求细节，这些细节是否符合业务预期？需要人工确认。

**Code Review**

增加了 AI 输出质量校验环节。AI 生成的代码，是否符合团队规范？是否有安全隐患？这些需要人工检查。

**测试评审**

验证测试用例的业务意义。AI 可以生成很多测试用例，但"能跑通"不等于"有业务意义"。
-->