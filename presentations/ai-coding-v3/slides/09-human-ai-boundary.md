---
layout: Default
---

# 1.4 人机协作边界

<div class="boundary-grid">

<div class="phase-row">
<div class="phase-name">需求阶段</div>
<div class="human-task">人定目标</div>
<div class="ai-task">AI 推演细节</div>
</div>

<div class="phase-row">
<div class="phase-name">设计阶段</div>
<div class="human-task">人做决策</div>
<div class="ai-task">AI 生成方案</div>
</div>

<div class="phase-row">
<div class="phase-name">实现阶段</div>
<div class="human-task">人定规范</div>
<div class="ai-task">AI 执行生成</div>
</div>

<div class="phase-row">
<div class="phase-name">验证阶段</div>
<div class="human-task">人把控质量</div>
<div class="ai-task">AI 辅助测试</div>
</div>

</div>

<div class="boundary-rule">
<strong>核心原则：</strong> 决策在人，执行在AI。人定义"是什么"，AI 执行"怎么做"。
</div>

<style>
.boundary-grid {
  display: flex;
  flex-direction: column;
  gap: var(--spacing-sm);
  margin-top: var(--spacing-md);
}
.phase-row {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  gap: var(--spacing-xs);
  padding: var(--spacing-sm);
  border-radius: var(--radius-md);
  background: var(--color-bg-subtle);
}
.phase-row:nth-child(1) { border-left: 4px solid var(--color-success); }
.phase-row:nth-child(2) { border-left: 4px solid var(--color-info); }
.phase-row:nth-child(3) { border-left: 4px solid var(--color-accent-teal); }
.phase-row:nth-child(4) { border-left: 4px solid var(--color-warning); }
.phase-name {
  font-family: var(--font-family-display);
  font-weight: var(--font-weight-medium);
  font-size: var(--font-size-card-title);
  color: var(--color-text-primary);
}
.human-task {
  background: var(--color-primary-light);
  padding: var(--spacing-xs);
  border-radius: var(--radius-sm);
  font-size: var(--font-size-card-body);
  color: var(--color-primary);
  text-align: center;
}
.ai-task {
  background: var(--color-accent-teal-light);
  padding: var(--spacing-xs);
  border-radius: var(--radius-sm);
  font-size: var(--font-size-card-body);
  color: var(--color-accent-teal);
  text-align: center;
}
.boundary-rule {
  margin-top: var(--spacing-lg);
  padding: var(--spacing-md);
  background: var(--color-accent-orange-light);
  border-radius: var(--radius-md);
  border-left: 4px solid var(--color-accent-orange);
  font-size: var(--font-size-card-body);
  color: var(--color-text-primary);
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

后面我们将围绕这个结论来展开。

接下来，我们进入第二部分：具体的工具和协作框架。
-->
