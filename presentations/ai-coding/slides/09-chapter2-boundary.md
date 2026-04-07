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

<div class="boundary-card warning">
<div class="stage-badge">03 实现阶段</div>
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
</div>

<style>
.boundary-list {
  display: flex;
  flex-direction: column;
  gap: var(--spacing-md);
  margin-top: var(--spacing-md);
}

.boundary-card {
  border-radius: var(--radius-md);
  border: 1px solid;
  display: flex;
  align-items: stretch;
}

.boundary-card.success { background: var(--color-success-light); border-color: var(--color-success); }
.boundary-card.info { background: var(--color-info-light); border-color: var(--color-info); }
.boundary-card.warning { background: var(--color-warning-light); border-color: var(--color-warning); }

.stage-badge {
  font-family: var(--font-family-display);
  font-weight: var(--font-weight-semibold);
  font-size: var(--font-size-card-body);
  padding: var(--spacing-sm) var(--spacing-md);
  color: var(--color-bg-card);
  display: flex;
  align-items: center;
  writing-mode: vertical-rl;
  text-orientation: mixed;
  min-width: 40px;
}

.boundary-card.success .stage-badge { background: var(--color-success); }
.boundary-card.info .stage-badge { background: var(--color-info); }
.boundary-card.warning .stage-badge { background: var(--color-warning); }

.card-content {
  padding: var(--spacing-sm) var(--spacing-md);
  flex: 1;
}

.role-item {
  display: flex;
  align-items: center;
  gap: var(--spacing-sm);
  padding: var(--spacing-xs) 0;
}

.tag {
  font-family: var(--font-family-display);
  font-weight: var(--font-weight-medium);
  font-size: var(--font-size-card-meta);
  padding: 2px 10px;
  border-radius: var(--radius-sm);
  color: var(--color-bg-card);
}

.tag-ai { background: var(--color-primary); }
.tag-human { background: var(--color-text-primary); }

.text {
  font-size: var(--font-size-card-body);
  color: var(--color-text-primary);
}

.principle-panel {
  background: linear-gradient(135deg, var(--color-primary) 0%, #2D4BC7 100%);
  border-radius: var(--radius-lg);
  padding: var(--spacing-xl);
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
  margin-bottom: var(--spacing-sm);
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
  margin: var(--spacing-lg) 0;
}

.principle-explain {
  font-size: var(--font-size-card-body);
  line-height: var(--line-height-relaxed);
  text-align: center;
  opacity: 0.95;
}
</style>

<!--
我来用一个表格总结"人做什么、AI做什么"：

**记住一条原则：决策在人，执行在AI。**

AI 可以帮你生成方案、生成代码，但决策——做什么、不做什么、怎么做——必须由人来决定。
-->