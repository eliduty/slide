---
layout: two-cols-header
---

::title::

# 本次分享的核心：Harness 工程化体系

::left::

<div class="goal-card">
<div class="goal-icon">🎯</div>
<h3 class="goal-title">核心理念</h3>
<p class="goal-desc">
   <strong>Harness</strong>——让 AI 在规范约束下执行任务，输出<strong>可预测、可追溯、可验证</strong>的结果
  </p>
</div>

::right::

<div class="harness-detail">
<h4 class="detail-title">Harness 包含三大要素</h4>
<div class="detail-grid">
<div class="detail-item">
<div class="item-icon" style="--item-color: #4361EE;">📋</div>
<div class="item-content">
<div class="item-name">模板</div>
<div class="item-desc">PRD、design、tasks 等标准化文档</div>
</div>
</div>
<div class="detail-item">
<div class="item-icon" style="--item-color: #22C55E;">📜</div>
<div class="item-content">
<div class="item-name">规则</div>
<div class="item-desc">CLAUDE.md + rules 约束文件</div>
</div>
</div>
<div class="detail-item">
<div class="item-icon" style="--item-color: #F59E0B;">⚙️</div>
<div class="item-content">
<div class="item-name">工作流</div>
<div class="item-desc">explore → propose →  apply → archive</div>
</div>
</div>
</div>
</div>

<style>
/* 左侧目标卡片 - 优化紧凑布局 */
.goal-card {
  background: linear-gradient(135deg, var(--color-primary-light) 0%, var(--color-bg-card) 100%);
  border: 2px solid var(--color-primary);
  border-radius: var(--radius-lg);
  padding: var(--spacing-lg);
  text-align: center;
  height: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  box-shadow: var(--shadow-md);
}

.goal-icon {
  font-size: 40px;
  margin-bottom: var(--spacing-sm);
}

.goal-title {
  font-size: 40px;
  font-weight: 600;
  color: var(--color-text-primary);
  margin: 0 0 var(--spacing-sm) 0;
}

.goal-desc {
  font-size: calc(var(--font-size-body-sm) * 1.05);
  color: var(--color-text-secondary);
  line-height: 1.5;
  margin: 0;
}

.goal-desc strong {
  color: var(--color-primary);
  font-weight: 600;
}

/* 右侧 Harness 详情 - 优化紧凑布局 */
.harness-detail {
  background: var(--color-bg-card);
  border: 1px solid var(--color-border);
  border-radius: var(--radius-lg);
  padding: var(--spacing-sm);
  height: 100%;
  display: flex;
  flex-direction: column;
}

.detail-title {
  font-size: var(--font-size-card-title);
  font-weight: 600;
  color: var(--color-text-primary);
  margin: 0 0 var(--spacing-md) 0;
  padding-bottom: var(--spacing-xs);
  border-bottom: 2px solid var(--color-bg-page);
}

.detail-grid {
  display: flex;
  flex-direction: column;
  gap: var(--spacing-sm);
  flex: 1;
  justify-content: center;
}

.detail-item {
  display: flex;
  align-items: center;
  gap: var(--spacing-sm);
  padding: 10px var(--spacing-sm);
  background: var(--color-bg-page);
  border-radius: var(--radius-md);
  transition: all var(--transition-fast);
}

.detail-item:hover {
  background: var(--color-bg-hover);
  transform: translateX(4px);
}

.item-icon {
  width: 40px;
  height: 40px;
  background: var(--item-color);
  border-radius: var(--radius-md);
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 20px;
  flex-shrink: 0;
}

.item-content {
  display: flex;
  flex-direction: column;
  gap: 2px;
  flex: 1;
}

.item-name {
  font-weight: 600;
  font-size: var(--font-size-body-sm);
  color: var(--color-text-primary);
}

.item-desc {
  font-size: calc(var(--font-size-body-sm) * 0.9);
  color: var(--color-text-secondary);
  line-height: 1.4;
}
</style>

<!--
有了这套 Harness，你就不用每次都「祈祷 AI 能猜对」，而是让 AI 在规范约束下执行任务。

这套 Harness 包含三部分：
- 模板：PRD、design、tasks 等标准化文档格式
- 规则：CLAUDE.md + rules 约束文件
- 工作流：explore →propose →  apply → archive 四步流程

接下来，我们正式进入第一部分：AI Coding 的能力边界。
-->
