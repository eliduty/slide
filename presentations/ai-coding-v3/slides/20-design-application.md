---
layout: Default
---

# 3.5 设计阶段——工具应用

<div class="app-grid">

<div class="app-item">
<div class="app-num">01</div>
<div class="app-title">架构设计</div>
<div class="app-desc">目录结构、模块划分、依赖关系</div>
</div>

<div class="app-item">
<div class="app-num">02</div>
<div class="app-title">技术选型</div>
<div class="app-desc">对比方案优劣，给出推荐理由</div>
</div>

<div class="app-item">
<div class="app-num">03</div>
<div class="app-title">接口契约</div>
<div class="app-desc">API 定义、数据模型、错误码规范</div>
</div>

<div class="app-item">
<div class="app-num">04</div>
<div class="app-title">任务分解</div>
<div class="app-desc">拆分成可执行的任务列表（tasks.md）</div>
</div>

<div class="app-item">
<div class="app-num">05</div>
<div class="app-title">测试方案</div>
<div class="app-desc">测试策略、测试场景、用例框架</div>
</div>

<div class="app-item">
<div class="app-num">06</div>
<div class="app-title">运维方案</div>
<div class="app-desc">CI/CD 配置、部署、监控策略</div>
</div>

</div>

<div class="bottom-row">
<div class="output-box">
<strong>核心产出：</strong>proposal + design + tasks + specs
</div>
<div class="tool-box">
<strong>配合工具：</strong>OpenSpec propose/explore
</div>
</div>

<style>
.app-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: var(--spacing-sm);
  margin-top: var(--spacing-sm);
}
.app-item {
  padding: var(--spacing-sm);
  border-radius: var(--radius-md);
  border: 1px solid var(--color-border);
  background: var(--color-bg-subtle);
  text-align: center;
}
.app-num {
  font-family: var(--font-family-display);
  font-weight: var(--font-weight-semibold);
  font-size: 20px;
  color: var(--color-info);
  margin-bottom: 2px;
}
.app-title {
  font-family: var(--font-family-display);
  font-weight: var(--font-weight-medium);
  font-size: 14px;
  color: var(--color-text-primary);
  margin-bottom: 2px;
}
.app-desc {
  font-size: 11px;
  color: var(--color-text-secondary);
  line-height: 1.3;
}
.bottom-row {
  display: grid;
  grid-template-columns: 1.2fr 0.8fr;
  gap: var(--spacing-sm);
  margin-top: var(--spacing-sm);
}
.output-box {
  padding: var(--spacing-sm);
  background: var(--color-info-light);
  border-radius: var(--radius-md);
  font-size: 13px;
}
.tool-box {
  padding: var(--spacing-sm);
  background: var(--color-accent-gold-light);
  border-radius: var(--radius-md);
  font-size: 13px;
}
</style>

<!--
设计阶段具体怎么用 AI 工具？6个核心应用：

**01. 架构设计**：目录结构、模块划分、依赖关系

**02. 技术选型**：对比方案优劣，给出推荐理由

**03. 接口契约**：API 定义、数据模型、错误码规范

**04. 任务分解**：拆分成可执行的任务列表（tasks.md）

**05. 测试方案**：测试策略、测试场景、用例框架

**06. 运维方案**：CI/CD 配置、部署、监控策略

**核心产出**：proposal + design + tasks + specs
**配合工具**：OpenSpec propose/explore——生成规范文档，可评审

设计阶段完成后，进入环境规范阶段。这个阶段最容易被跳过，但非常重要。
-->
