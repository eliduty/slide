---
layout: Default
---

# 3.1 四阶段总览

<div class="phases-flow">

<div class="phase-box">
<div class="phase-num">01</div>
<div class="phase-name">需求阶段</div>
<div class="phase-desc">需求推演 → 结构化描述 → PRD</div>
</div>

<div class="flow-arrow">→</div>

<div class="phase-box">
<div class="phase-num">02</div>
<div class="phase-name">设计阶段</div>
<div class="phase-desc">propose → explore → apply → archive</div>
</div>

<div class="flow-arrow">→</div>

<div class="phase-box">
<div class="phase-num">03</div>
<div class="phase-name">环境规范阶段</div>
<div class="phase-desc">CLAUDE.md + rules + 验证上下文</div>
</div>

<div class="flow-arrow">→</div>

<div class="phase-box">
<div class="phase-num">04</div>
<div class="phase-name">实现阶段</div>
<div class="phase-desc">按 tasks 执行 → 生成代码 → 测试验证</div>
</div>

</div>

<div class="phase-note">
<strong>关键原则：</strong>每个阶段用 5W1H 定义——谁参与、做什么、标准、产出、如何做。顺序不能乱，跳过环境规范阶段是最常见错误。
</div>

<style>
.phases-flow {
  display: flex;
  align-items: stretch;
  gap: var(--spacing-xs);
  margin-top: var(--spacing-md);
}
.phase-box {
  flex: 1;
  padding: var(--spacing-md);
  border-radius: var(--radius-md);
  text-align: center;
}
.phase-box:nth-child(1) { background: var(--color-success-light); border: 1px solid var(--color-success); }
.phase-box:nth-child(3) { background: var(--color-info-light); border: 1px solid var(--color-info); }
.phase-box:nth-child(5) { background: var(--color-accent-teal-light); border: 1px solid var(--color-accent-teal); }
.phase-box:nth-child(7) { background: var(--color-warning-light); border: 1px solid var(--color-warning); }
.phase-num {
  font-family: var(--font-family-display);
  font-weight: var(--font-weight-semibold);
  font-size: var(--font-size-heading);
  color: var(--color-primary);
  margin-bottom: var(--spacing-xs);
}
.phase-name {
  font-family: var(--font-family-display);
  font-weight: var(--font-weight-medium);
  font-size: var(--font-size-card-title);
  color: var(--color-text-primary);
  margin-bottom: var(--spacing-xs);
}
.phase-desc {
  font-size: var(--font-size-card-body);
  color: var(--color-text-secondary);
}
.flow-arrow {
  font-size: var(--font-size-heading);
  color: var(--color-text-muted);
  padding-top: var(--spacing-md);
}
.phase-note {
  margin-top: var(--spacing-lg);
  padding: var(--spacing-md);
  background: var(--color-error-light);
  border-radius: var(--radius-md);
  border-left: 4px solid var(--color-error);
  font-size: var(--font-size-card-body);
  color: var(--color-text-primary);
}
</style>

<!--
四阶段工作流程：

**01 需求阶段**
流程：需求推演 → 结构化描述 → PRD 文档
这个阶段把模糊的想法变成明确的需求文档。

**02 设计阶段**
流程：propose → explore → apply → archive
这个阶段生成技术规范，经过评审后执行。

**03 环境规范阶段**
流程：配置 CLAUDE.md → rules → 验证上下文
这个阶段让 AI 理解项目上下文，是最容易被跳过的阶段。

**04 实现阶段**
流程：按 tasks 执行 → 生成代码 → 测试验证
这个阶段按规范执行，生成代码和测试。

**关键原则**：
- 每个阶段用 5W1H 定义
- 顺序不能乱
- 跳过环境规范阶段是最常见错误

接下来，我们逐个阶段详细展开。先看需求阶段。
-->