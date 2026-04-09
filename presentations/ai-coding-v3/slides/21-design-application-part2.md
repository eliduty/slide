---
layout: Default
---

# 3.5 设计阶段——工具应用（下）

<div class="app-grid">

<div class="app-item">
<div class="app-num">05</div>
<div class="app-title">测试场景与测试方案</div>
<div class="app-desc">生成测试策略、测试场景、测试用例框架</div>
</div>

<div class="app-item">
<div class="app-num">06</div>
<div class="app-title">运维与持续交付方案</div>
<div class="app-desc">生成 CI/CD 配置、部署方案、监控策略</div>
</div>

</div>

<div class="design-summary">
<strong>设计阶段核心产出</strong>
<ul>
<li><strong>架构设计：</strong>目录结构、模块划分、依赖关系</li>
<li><strong>技术选型：</strong>对比分析、推荐理由</li>
<li><strong>接口契约：</strong>API 定义、数据模型、错误码规范</li>
<li><strong>任务分解：</strong>可执行的任务列表（tasks.md）</li>
<li><strong>测试方案：</strong>测试策略、测试场景</li>
<li><strong>运维方案：</strong>CI/CD、部署、监控</li>
</ul>
</div>

<div class="tool-tip">
<strong>配合工具：</strong>OpenSpec propose/explore——生成规范文档，可评审
</div>

<style>
.app-grid {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: var(--spacing-lg);
  margin-top: var(--spacing-xl);
}
.app-item {
  padding: var(--spacing-lg);
  border-radius: var(--radius-md);
  border: 1px solid var(--color-border);
  background: var(--color-bg-subtle);
}
.app-num {
  font-family: var(--font-family-display);
  font-weight: var(--font-weight-semibold);
  font-size: 48px;
  color: var(--color-info);
  margin-bottom: var(--spacing-sm);
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
.design-summary {
  margin-top: var(--spacing-xl);
  padding: var(--spacing-md);
  background: var(--color-info-light);
  border-radius: var(--radius-md);
}
.design-summary strong {
  font-family: var(--font-family-display);
  font-size: var(--font-size-card-title);
  color: var(--color-text-primary);
  display: block;
  margin-bottom: var(--spacing-sm);
}
.design-summary ul {
  margin: 0;
  margin-left: var(--spacing-md);
  font-size: var(--font-size-card-body);
  color: var(--color-text-secondary);
}
.design-summary li {
  margin-bottom: var(--spacing-xs);
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
设计阶段工具应用（下）：

**05. 测试场景与测试方案**

AI 可以生成测试策略、测试场景、测试用例框架。测试策略前置是关键。

**06. 运维与持续交付方案**

AI 可以生成 CI/CD 配置、部署方案、监控策略。

**设计阶段核心产出总结**：

- 架构设计：目录结构、模块划分、依赖关系
- 技术选型：对比分析、推荐理由
- 接口契约：API 定义、数据模型、错误码规范
- 任务分解：可执行的任务列表（tasks.md）
- 测试方案：测试策略、测试场景
- 运维方案：CI/CD、部署、监控

**配合工具**：OpenSpec propose/explore——生成规范文档，可评审。

设计阶段完成后，进入环境规范阶段。
-->
