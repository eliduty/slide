---
layout: Default
---

# 4.2 设计阶段

<div class="design-list">

<div class="design-row">
<div class="item">架构设计</div>
<div class="item">技术选型比较</div>
<div class="item">接口契约设计</div>
</div>

<div class="design-row">
<div class="item">界面交互原型</div>
<div class="item">测试方案制定</div>
<div class="item">CI/CD设计</div>
</div>

</div>

<div class="output-box">
<strong>设计阶段产出物三件套：</strong>
<span>proposal.md</span>
<span>design.md</span>
<span>tasks.md</span>
</div>

<div class="case-ref">
📁 案例路径：<code>openspec/changes/admin-role-authorization/</code>
</div>

<style>
.design-list { margin-top: var(--spacing-md); }
.design-row {
  display: flex;
  gap: var(--spacing-md);
  margin-bottom: var(--spacing-md);
}
.item {
  flex: 1;
  padding: var(--spacing-md);
  border-radius: var(--radius-md);
  text-align: center;
  font-family: var(--font-family-display);
  font-weight: var(--font-weight-medium);
  font-size: var(--font-size-card-title);
  color: var(--color-text-primary);
  border: 1px solid;
}
.design-row:nth-child(1) .item:nth-child(1) { background: var(--color-info-light); border-color: var(--color-info); }
.design-row:nth-child(1) .item:nth-child(2) { background: var(--color-success-light); border-color: var(--color-success); }
.design-row:nth-child(1) .item:nth-child(3) { background: var(--color-warning-light); border-color: var(--color-warning); }
.design-row:nth-child(2) .item:nth-child(1) { background: var(--color-accent-teal-light); border-color: var(--color-accent-teal); }
.design-row:nth-child(2) .item:nth-child(2) { background: var(--color-accent-gold-light); border-color: var(--color-accent-gold); }
.design-row:nth-child(2) .item:nth-child(3) { background: var(--color-accent-rose-light); border-color: var(--color-accent-rose); }
.output-box {
  margin-top: var(--spacing-lg);
  padding: var(--spacing-md) var(--spacing-lg);
  background: var(--color-primary);
  color: var(--color-bg-card);
  border-radius: var(--radius-md);
  display: flex;
  align-items: center;
  gap: var(--spacing-md);
}
.output-box strong { font-size: var(--font-size-card-body); }
.output-box span {
  background: rgba(255,255,255,0.2);
  padding: 4px 10px;
  border-radius: var(--radius-sm);
  font-size: var(--font-size-card-meta);
}
.case-ref {
  margin-top: var(--spacing-md);
  padding: var(--spacing-sm) var(--spacing-lg);
  background: var(--color-bg-hover);
  border-radius: var(--radius-md);
  font-size: var(--font-size-card-body);
  color: var(--color-text-primary);
}
</style>

<!--
设计阶段是 AI 发挥作用最大的环节。AI 可以帮你做七件事：

1. **架构设计与项目结构治理**——告诉你项目目录怎么组织、模块怎么划分
2. **技术选型**——提供方案比较，帮你分析优劣
3. **接口契约设计**——生成 OpenAPI/Swagger 规范
4. **界面交互原型设计**——我们用 Pencil 工具，AI 可以直接生成原型
5. **界面设计规范与详细设计**——组件怎么设计、交互怎么定义
6. **测试场景与测试方案制定**——告诉你测什么、怎么测
7. **运维与持续交付方案设计**——CI/CD 管道、部署策略

产出物是三件套：proposal.md + design.md + tasks.md。

我们有一个完整的变更案例：`openspec/changes/admin-role-authorization/`。这个案例展示了从 proposal 到 design 到 tasks 的完整过程，大家课后可以去看。
-->