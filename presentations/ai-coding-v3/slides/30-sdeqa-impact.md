---
layout: TwoCols
---

::left::

# 4.2 对 SDE/QA 影响

<div class="sde-qa">

<div class="impact-item">
<strong>架构设计前移</strong>
<p>设计必须先行，design.md 在代码之前产出</p>
</div>

<div class="impact-item">
<strong>SDE 补测试技能</strong>
<p>AI可生成测试用例，需验证其业务意义</p>
</div>

<div class="impact-item">
<strong>QA 参与开发</strong>
<p>基于 tasks.md 任务分配，任务已拆得很细</p>
</div>

</div>

::right::

<div class="key-skills">
<div class="key-skills-title">需要学习的能力</div>
<ul>
<li>测试思维：什么是有效测试</li>
<li>任务拆分：如何写出 tasks.md</li>
<li>设计文档：design.md 写什么</li>
</ul>
</div>

<style>
.sde-qa {
  display: flex;
  flex-direction: column;
  gap: var(--spacing-md);
}
.impact-item {
  padding: var(--spacing-sm);
  border-radius: var(--radius-md);
  border: 1px solid;
}
.impact-item:nth-child(1) { background: var(--color-info-light); border-color: var(--color-info); }
.impact-item:nth-child(2) { background: var(--color-success-light); border-color: var(--color-success); }
.impact-item:nth-child(3) { background: var(--color-warning-light); border-color: var(--color-warning); }
.impact-item p {
  font-size: var(--font-size-card-body);
  color: var(--color-text-secondary);
  margin: var(--spacing-xs) 0 0 0;
}
.key-skills {
  background: #1A365D;
  padding: var(--spacing-lg);
  border-radius: var(--radius-lg);
}
.key-skills-title {
  color: #FFFFFF;
  font-size: var(--font-size-card-title);
  font-weight: var(--font-weight-medium);
  margin-bottom: var(--spacing-sm);
}
.key-skills ul {
  margin: 0;
  padding-left: var(--spacing-lg);
  list-style-type: none;
}
.key-skills li {
  margin-bottom: var(--spacing-sm);
  font-size: var(--font-size-card-body);
  color: #FFFFFF;
  padding-left: var(--spacing-sm);
  position: relative;
}
.key-skills li::before {
  content: "•";
  position: absolute;
  left: -12px;
  color: #ED8936;
}
</style>

<!--
**架构设计工作的前移与显性化**

以前可能边写代码边设计，现在设计必须先行。design.md 必须在代码之前产出。为什么？因为 AI 需要设计文档作为上下文，没有设计文档，AI 生成的代码就没有约束。

**SDE 如何弥补测试技能的不足**

AI 可以生成测试用例，但你需要验证这些测试用例是否有业务意义。所以 SDE 需要学习测试思维，知道什么样的测试是有效的。

**QA 如何实现开发**

基于 tasks.md 的任务分配，QA 也可以参与开发。因为任务已经拆得很细，每个任务对应一个可独立验证的实现单元。

了解了对 PM、SDE、QA 的影响，我们再看对评审工作的影响。
-->