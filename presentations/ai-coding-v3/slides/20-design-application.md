---
layout: Default
---

# 3.4 设计阶段——工具应用（上）

<div class="app-grid">

<div class="app-item">
<div class="app-num">01</div>
<div class="app-title">架构设计与项目结构治理</div>
<div class="app-desc">生成合理的目录结构、模块划分、依赖关系</div>
</div>

<div class="app-item">
<div class="app-num">02</div>
<div class="app-title">技术选型</div>
<div class="app-desc">对比不同技术方案的优劣，给出推荐理由</div>
</div>

<div class="app-item">
<div class="app-num">03</div>
<div class="app-title">接口契约设计</div>
<div class="app-desc">生成 API 接口定义、数据模型、错误码规范</div>
</div>

<div class="app-item">
<div class="app-num">04</div>
<div class="app-title">任务分解</div>
<div class="app-desc">把设计拆分成可执行的任务列表，便于分配和跟踪</div>
</div>

</div>

<div class="tool-tip">
<strong>配合工具：</strong>OpenSpec propose/explore——生成规范文档，可评审
</div>

<div class="continue-hint" style="margin-top: var(--spacing-md); text-align: center; color: var(--color-text-secondary);">
<strong>→</strong> 接下页：测试场景与运维方案
</div>

<style>
.app-grid {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: var(--spacing-md);
  margin-top: var(--spacing-md);
}
.app-item {
  padding: var(--spacing-md);
  border-radius: var(--radius-md);
  border: 1px solid var(--color-border);
  background: var(--color-bg-subtle);
}
.app-num {
  font-family: var(--font-family-display);
  font-weight: var(--font-weight-semibold);
  font-size: var(--font-size-heading);
  color: var(--color-info);
  margin-bottom: var(--spacing-xs);
}
.app-title {
  font-family: var(--font-family-display);
  font-weight: var(--font-weight-medium);
  font-size: var(--font-size-card-title);
  color: var(--color-text-primary);
  margin-bottom: var(--spacing-xs);
}
.app-desc {
  font-size: var(--font-size-card-body);
  color: var(--color-text-secondary);
}
.tool-tip {
  margin-top: var(--spacing-lg);
  padding: var(--spacing-md);
  background: var(--color-info-light);
  border-radius: var(--radius-md);
  font-size: var(--font-size-card-body);
  color: var(--color-text-primary);
}
</style>

<!--
设计阶段具体怎么用 AI 工具？

**01. 架构设计与项目结构治理**

AI 可以生成合理的目录结构、模块划分、依赖关系。但你要给它明确的约束条件。

**02. 技术选型**

AI 可以对比不同技术方案的优劣，给出推荐理由。但最终决策权在你。

**03. 接口契约设计**

AI 可以生成 API 接口定义、数据模型、错误码规范。这是设计阶段最重要的产出之一。

**04. 任务分解**

AI 可以把设计拆分成可执行的任务列表，便于分配和跟踪。这就是 tasks.md。

**05. 测试场景与测试方案**

AI 可以生成测试策略、测试场景、测试用例框架。测试策略前置是关键。

**06. 运维与持续交付方案**

AI 可以生成 CI/CD 配置、部署方案、监控策略。

**配合工具**：OpenSpec propose/explore——生成规范文档，可评审。

设计阶段完成后，进入环境规范阶段。这个阶段最容易被跳过，但非常重要。
-->