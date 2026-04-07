---
layout: TwoCols
---

::left::

# 2.2 人与AI的边界

<div class="boundary-list">

<div class="boundary-card success">
<div class="stage-badge">01 需求阶段</div>
<div class="card-content">
<div class="role-item">
<span class="tag tag-ai">AI</span>
<span class="text">需求推演完善、结构化描述</span>
</div>
<div class="role-item">
<span class="tag tag-human">人</span>
<span class="text">业务目标定义、验收标准确定</span>
</div>
</div>
</div>

<div class="boundary-card info">
<div class="stage-badge">02 设计阶段</div>
<div class="card-content">
<div class="role-item">
<span class="tag tag-ai">AI</span>
<span class="text">技术方案生成、接口契约设计</span>
</div>
<div class="role-item">
<span class="tag tag-human">人</span>
<span class="text">技术选型决策、架构边界定义</span>
</div>
</div>
</div>

<div class="boundary-card teal">
<div class="stage-badge">03 环境规范</div>
<div class="card-content">
<div class="role-item">
<span class="tag tag-ai">AI</span>
<span class="text">辅助生成规则模板、测试框架</span>
</div>
<div class="role-item">
<span class="tag tag-human">人</span>
<span class="text">定义约束、审核规则、验证理解</span>
</div>
</div>
</div>

<div class="boundary-card warning">
<div class="stage-badge">04 实现阶段</div>
<div class="card-content">
<div class="role-item">
<span class="tag tag-ai">AI</span>
<span class="text">根据规范生成代码、测试</span>
</div>
<div class="role-item">
<span class="tag tag-human">人</span>
<span class="text">验证输出质量、处理边界情况</span>
</div>
</div>
</div>

</div>

::right::

<div class="principle-panel">
<div class="principle-header">核心原则</div>
<div class="principle-main">决策在人<br/>执行在AI</div>
<div class="principle-divider"></div>
<div class="principle-explain">
AI 可以帮你生成方案、生成代码，但决策——做什么、不做什么、怎么做——必须由人来决定。
</div>
<div class="principle-note">
<div class="note-item">环境规范阶段：人定义约束，AI辅助执行</div>
<div class="note-item">验证理解是关键：确保AI真的懂了</div>
</div>
</div>

<style>
.boundary-list {
  display: flex;
  flex-direction: column;
  gap: var(--spacing-sm);
  margin-top: var(--spacing-sm);
}

.boundary-card {
  border-radius: var(--radius-md);
  border: 1px solid;
  display: flex;
  align-items: stretch;
}

.boundary-card.success { background: var(--color-success-light); border-color: var(--color-success); }
.boundary-card.info { background: var(--color-info-light); border-color: var(--color-info); }
.boundary-card.teal { background: var(--color-accent-teal-light); border-color: var(--color-accent-teal); }
.boundary-card.warning { background: var(--color-warning-light); border-color: var(--color-warning); }

.stage-badge {
  font-family: var(--font-family-display);
  font-weight: var(--font-weight-semibold);
  font-size: var(--font-size-card-meta);
  padding: var(--spacing-xs) var(--spacing-sm);
  color: var(--color-bg-card);
  display: flex;
  align-items: center;
  writing-mode: vertical-rl;
  text-orientation: mixed;
  min-width: 32px;
}

.boundary-card.success .stage-badge { background: var(--color-success); }
.boundary-card.info .stage-badge { background: var(--color-info); }
.boundary-card.teal .stage-badge { background: var(--color-accent-teal); }
.boundary-card.warning .stage-badge { background: var(--color-warning); }

.card-content {
  padding: var(--spacing-xs) var(--spacing-sm);
  flex: 1;
}

.role-item {
  display: flex;
  align-items: center;
  gap: var(--spacing-xs);
  padding: 2px 0;
}

.tag {
  font-family: var(--font-family-display);
  font-weight: var(--font-weight-medium);
  font-size: 11px;
  padding: 2px 8px;
  border-radius: var(--radius-sm);
  color: var(--color-bg-card);
}

.tag-ai { background: var(--color-primary); }
.tag-human { background: var(--color-text-primary); }

.text {
  font-size: var(--font-size-card-meta);
  color: var(--color-text-primary);
}

.principle-panel {
  background: linear-gradient(135deg, var(--color-primary) 0%, #2D4BC7 100%);
  border-radius: var(--radius-lg);
  padding: var(--spacing-lg);
  color: var(--color-bg-card);
  height: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}

.principle-header {
  font-family: var(--font-family-display);
  font-size: var(--font-size-card-body);
  opacity: 0.9;
  margin-bottom: var(--spacing-xs);
}

.principle-main {
  font-family: var(--font-family-display);
  font-weight: var(--font-weight-semibold);
  font-size: var(--font-size-heading);
  line-height: var(--line-height-tight);
  text-align: center;
}

.principle-divider {
  width: 60px;
  height: 2px;
  background: rgba(255, 255, 255, 0.3);
  margin: var(--spacing-sm) 0;
}

.principle-explain {
  font-size: var(--font-size-card-body);
  line-height: var(--line-height-relaxed);
  text-align: center;
  opacity: 0.95;
}

.principle-note {
  margin-top: var(--spacing-sm);
  padding: var(--spacing-sm);
  border-radius: var(--radius-md);
  background: rgba(255,255,255,0.1);
}

.note-item {
  font-size: var(--font-size-card-meta);
  opacity: 0.9;
  margin-bottom: 2px;
}
</style>

<!--
我来用一个表格总结"人做什么、AI做什么"，现在我们有四个阶段：

**第一阶段：需求阶段**

AI 负责：需求推演完善、结构化描述。
人负责：业务目标定义、验收标准确定。

AI 可以帮你把模糊的需求变成结构化的文档，但"做什么功能、做到什么程度"，必须你来定。

**第二阶段：设计阶段**

AI 负责：技术方案生成、接口契约设计。
人负责：技术选型决策、架构边界定义。

AI 可以给你几个技术方案选项，但"选哪个方案、架构边界在哪"，必须你来拍板。

**第三阶段：环境规范阶段**

AI 负责：辅助生成规则模板、测试框架。
人负责：定义约束、审核规则、验证理解。

这个阶段，AI 可以帮你生成 CLAUDE.md 的模板、测试框架的代码。但规则内容是什么、测试策略是什么，必须你来定义。

关键是：**验证 AI 真的懂了**。你可以问 AI 一个问题，看它回答是否符合你的预期。如果不符合，说明规则没写清楚，需要补充。

**第四阶段：实现阶段**

AI 负责：根据规范生成代码、测试。
人负责：验证输出质量、处理边界情况。

AI 可以生成代码，但你要验证：代码是否符合规范、边界情况有没有处理、有没有引入安全问题。

**记住一条原则：决策在人，执行在AI。**

AI 可以帮你生成方案、生成代码，但决策——做什么、不做什么、怎么做——必须由人来决定。

**特别提醒：环境规范阶段的"验证理解"是关键。**

很多人写完 CLAUDE.md 就以为 AI 懂了，但其实 AI 可能理解偏差。你要测试一下：让 AI 解释一下某个规则，看它说的跟你想的一致不一致。
-->