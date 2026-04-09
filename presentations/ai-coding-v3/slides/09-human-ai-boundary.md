---
layout: TwoCols
---

::left::

# 1.4 人机协作边界

<div class="boundary-list">

<div class="boundary-card success">
<div class="stage-number">01</div>
<div class="stage-name"><span>需求</span><span>阶段</span></div>
<div class="card-content">
<div class="role-item">
<span class="tag tag-human">人</span>
<span class="text">定目标——业务目标、验收标准</span>
</div>
<div class="role-item">
<span class="tag tag-ai">AI</span>
<span class="text">推演细节——补充场景、完善描述</span>
</div>
</div>
</div>

<div class="boundary-card info">
<div class="stage-number">02</div>
<div class="stage-name"><span>设计</span><span>阶段</span></div>
<div class="card-content">
<div class="role-item">
<span class="tag tag-human">人</span>
<span class="text">做决策——技术选型、架构边界</span>
</div>
<div class="role-item">
<span class="tag tag-ai">AI</span>
<span class="text">生成方案——技术方案、接口契约</span>
</div>
</div>
</div>

<div class="boundary-card teal">
<div class="stage-number">03</div>
<div class="stage-name"><span>实现</span><span>阶段</span></div>
<div class="card-content">
<div class="role-item">
<span class="tag tag-human">人</span>
<span class="text">定规范——编码规范、测试策略</span>
</div>
<div class="role-item">
<span class="tag tag-ai">AI</span>
<span class="text">执行生成——按规范生成代码</span>
</div>
</div>
</div>

<div class="boundary-card warning">
<div class="stage-number">04</div>
<div class="stage-name"><span>验证</span><span>阶段</span></div>
<div class="card-content">
<div class="role-item">
<span class="tag tag-human">人</span>
<span class="text">把控质量——验证是否满足规格</span>
</div>
<div class="role-item">
<span class="tag tag-ai">AI</span>
<span class="text">辅助测试——生成用例、执行测试</span>
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
人定义<strong>"是什么"</strong><br/>
AI 执行<strong>"怎么做"</strong>
</div>
<div class="principle-note">
<div class="note-item">这个边界不能模糊</div>
<div class="note-item">把决策交给 AI，结果就会失控</div>
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
  gap: 0;
  overflow: hidden;
}

.boundary-card.success { background: var(--color-success-light); border-color: var(--color-success); }
.boundary-card.info { background: var(--color-info-light); border-color: var(--color-info); }
.boundary-card.teal { background: var(--color-accent-teal-light); border-color: var(--color-accent-teal); }
.boundary-card.warning { background: var(--color-warning-light); border-color: var(--color-warning); }

.stage-number {
  font-family: var(--font-family-display);
  font-weight: var(--font-weight-semibold);
  font-size: 18px;
  padding: var(--spacing-xs) 6px;
  color: var(--color-bg-card);
  display: flex;
  align-items: center;
  justify-content: center;
  min-width: 32px;
  border-radius: var(--radius-md) 0 0 var(--radius-md);
}

.boundary-card.success .stage-number { background: var(--color-success); }
.boundary-card.info .stage-number { background: var(--color-info); }
.boundary-card.teal .stage-number { background: var(--color-accent-teal); }
.boundary-card.warning .stage-number { background: var(--color-warning); }

.stage-name {
  font-family: var(--font-family-display);
  font-weight: var(--font-weight-semibold);
  font-size: 15px;
  padding: 4px 6px;
  color: var(--color-bg-card);
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  line-height: 1.2;
  gap: 0;
}

.stage-name span {
  display: block;
}

.boundary-card.success .stage-name { background: var(--color-success); }
.boundary-card.info .stage-name { background: var(--color-info); }
.boundary-card.teal .stage-name { background: var(--color-accent-teal); }
.boundary-card.warning .stage-name { background: var(--color-warning); }

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
  min-width: 36px;
  text-align: center;
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
清楚了 AI 的能力边界和规格驱动开发的价值，我们来看人机协作的具体分工。

四个阶段，每个阶段都有明确的分工：

**需求阶段**
- 人：定目标——业务目标是什么、验收标准是什么
- AI：推演细节——补充可能遗漏的场景、完善需求描述

**设计阶段**
- 人：做决策——技术选型、架构边界
- AI：生成方案——根据约束生成技术方案、接口契约

**实现阶段**
- 人：定规范——编码规范、测试策略
- AI：执行生成——按规范生成代码、测试

**验证阶段**
- 人：把控质量——验证输出是否满足规格
- AI：辅助测试——生成测试用例、执行测试

**核心原则：决策在人，执行在AI。**

人定义"是什么"，AI 执行"怎么做"。这个边界不能模糊——如果把决策交给 AI，结果就会失控。

清楚了人机协作的分工，接下来我们看看支撑这套分工的工具体系。
-->
