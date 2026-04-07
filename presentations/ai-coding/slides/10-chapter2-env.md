---
layout: Default
---

# 2.3 规范 AI 工作环境

<div class="env-flow">

<div class="env-stage">
<div class="stage-num">01</div>
<div class="stage-title">开发环境</div>
<div class="stage-detail">
<div><strong>谁：</strong>SDE</div>
<div><strong>做：</strong>配置 CLAUDE.md + rules</div>
<div><strong>标准：</strong>AI 能正确理解项目约束</div>
<div><strong>产出：</strong>项目规则文件</div>
</div>
</div>

<div class="env-stage">
<div class="stage-num">02</div>
<div class="stage-title">测试环境</div>
<div class="stage-detail">
<div><strong>谁：</strong>SDE + QA</div>
<div><strong>做：</strong>测试策略 + mock 数据</div>
<div><strong>标准：</strong>覆盖核心业务场景</div>
<div><strong>产出：</strong>测试用例 + mock</div>
</div>
</div>

<div class="env-stage">
<div class="stage-num">03</div>
<div class="stage-title">联动调试</div>
<div class="stage-detail">
<div><strong>谁：</strong>SDE</div>
<div><strong>做：</strong>前后端/模块间联调</div>
<div><strong>标准：</strong>接口契约一致</div>
<div><strong>产出：</strong>集成验证记录</div>
</div>
</div>

<div class="env-stage">
<div class="stage-num">04</div>
<div class="stage-title">领域知识</div>
<div class="stage-detail">
<div><strong>谁：</strong>SDE + PM</div>
<div><strong>做：</strong>业务术语 + 数据流图</div>
<div><strong>标准：</strong>AI 能理解业务语义</div>
<div><strong>产出：</strong>领域知识文档</div>
</div>
</div>

</div>

<div class="highlight">
<strong>关键：</strong>进入实现阶段前，必须完成这四项环境准备工作
</div>

<style>
.env-flow {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: var(--spacing-md);
  margin-top: var(--spacing-md);
}
.env-stage {
  padding: var(--spacing-md);
  border-radius: var(--radius-md);
  border: 1px solid;
}
.env-stage:nth-child(1) { background: var(--color-success-light); border-color: var(--color-success); }
.env-stage:nth-child(2) { background: var(--color-info-light); border-color: var(--color-info); }
.env-stage:nth-child(3) { background: var(--color-warning-light); border-color: var(--color-warning); }
.env-stage:nth-child(4) { background: var(--color-accent-teal-light); border-color: var(--color-accent-teal); }
.stage-num {
  font-family: var(--font-family-display);
  width: 28px;
  height: 28px;
  border-radius: var(--radius-sm);
  display: flex;
  align-items: center;
  justify-content: center;
  font-weight: var(--font-weight-semibold);
  font-size: var(--font-size-card-meta);
  background: var(--color-primary);
  color: var(--color-bg-card);
  margin-bottom: var(--spacing-xs);
}
.stage-title {
  font-family: var(--font-family-display);
  font-weight: var(--font-weight-medium);
  font-size: var(--font-size-card-title);
  color: var(--color-text-primary);
  margin-bottom: var(--spacing-sm);
}
.stage-detail div {
  font-size: var(--font-size-card-body);
  color: var(--color-text-secondary);
  margin-bottom: 2px;
}
.stage-detail strong {
  color: var(--color-primary);
}
.highlight {
  margin-top: var(--spacing-lg);
  padding: var(--spacing-md);
  background: var(--color-accent-orange-light);
  border-radius: var(--radius-md);
  border: 1px solid var(--color-accent-orange);
  font-size: var(--font-size-card-body);
  color: var(--color-text-primary);
}
</style>

<!--
在进入实现阶段之前，还有一件事要做：**规范 AI 工作环境**。

这不是可选的，这是必须的。为什么？因为 AI 需要上下文才能工作。上下文给不好，AI 的输出就会偏离。这个阶段，就是要把上下文准备好。

我们分四个部分来讲：

**第一：开发环境**

谁来做？SDE。

做什么？配置 CLAUDE.md 和 rules 文件。

达到什么标准？AI 能正确理解项目的技术栈约束、命名规范、禁止事项。

产出什么？项目规则文件。

这个阶段，你要告诉 AI：我们用 Vue3 + TypeScript，接口命名用 kebab-case，禁止直接操作 DOM。这些规则写进 CLAUDE.md，每次对话 AI 都会自动遵守。

**第二：测试环境**

谁来做？SDE 和 QA 配合。

做什么？制定测试策略，准备 mock 数据。

达到什么标准？覆盖核心业务场景，每个场景都有明确的输入输出定义。

产出什么？测试用例框架 + mock 数据方案。

这个阶段，你要让 AI 知道：哪些场景必须测试、怎么组织测试数据。否则 AI 生成的测试可能能跑通，但业务意义为零。

**第三：联动调试**

谁来做？SDE。

做什么？前后端联调、模块间联调。

达到什么标准？接口契约一致，数据格式对齐。

产出什么？集成验证记录。

这个阶段，你要把接口契约喂给 AI，让它知道前后端的约定。否则 AI 可能生成前端代码用了 A 字段名，后端却返回了 B 字段名。

**第四：领域知识规范化**

谁来做？SDE 和 PM 配合。

做什么？定义业务术语、绘制数据流图。

达到什么标准？AI 能理解业务语义，知道"订单"和"工单"的区别。

产出什么？领域知识文档。

这个阶段，你要把业务背景写清楚。比如"租户"是什么意思、"多租户隔离"要做到什么程度。这些知识，AI 不懂，你必须教它。

**记住一句话：进入实现阶段前，必须完成这四项环境准备工作。**

没准备好，就开始写代码，AI 就会乱猜。你后面花的时间，会比前期准备多得多。
-->