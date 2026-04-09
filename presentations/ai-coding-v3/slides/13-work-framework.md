---
layout: Default
---

# 2.3 工作开展框架

<div class="workflow-chain">

<div class="chain-stage">
<div class="stage-num">需求阶段</div>
<div class="stage-tool">Superpowers brainstorm</div>
<div class="stage-action">精炼需求，避免理解偏差</div>
</div>

<div class="chain-arrow">↓</div>

<div class="chain-stage">
<div class="stage-num">设计阶段</div>
<div class="stage-tool">OpenSpec explore → propose</div>
<div class="stage-action">生成规范文档，可评审</div>
</div>

<div class="chain-arrow">↓</div>

<div class="chain-stage">
<div class="stage-num">环境规范阶段</div>
<div class="stage-tool">CLAUDE.md + .claude/</div>
<div class="stage-action">配置上下文，让 AI 理解项目</div>
</div>

<div class="chain-arrow">↓</div>

<div class="chain-stage">
<div class="stage-num">实现阶段</div>
<div class="stage-tool">OpenSpec apply + Superpowers TDD</div>
<div class="stage-action">按规范执行，强制测试</div>
</div>

<div class="chain-arrow">↓</div>

<div class="chain-stage">
<div class="stage-num">收尾阶段</div>
<div class="stage-tool">OpenSpec archive</div>
<div class="stage-action">归档沉淀，可追溯</div>
</div>

</div>

<style>
.workflow-chain {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: var(--spacing-xs);
  margin-top: var(--spacing-md);
}
.chain-stage {
  padding: var(--spacing-sm) var(--spacing-md);
  border-radius: var(--radius-md);
  border: 1px solid var(--color-border);
  text-align: center;
  min-width: 400px;
}
.chain-stage:nth-child(1) { background: var(--color-success-light); border-color: var(--color-success); }
.chain-stage:nth-child(3) { background: var(--color-info-light); border-color: var(--color-info); }
.chain-stage:nth-child(5) { background: var(--color-accent-teal-light); border-color: var(--color-accent-teal); }
.chain-stage:nth-child(7) { background: var(--color-warning-light); border-color: var(--color-warning); }
.chain-stage:nth-child(9) { background: var(--color-accent-orange-light); border-color: var(--color-accent-orange); }
.stage-num {
  font-family: var(--font-family-display);
  font-weight: var(--font-weight-medium);
  font-size: var(--font-size-card-title);
  color: var(--color-text-primary);
}
.stage-tool {
  font-size: var(--font-size-card-body);
  color: var(--color-primary);
  font-weight: var(--font-weight-medium);
}
.stage-action {
  font-size: var(--font-size-card-meta);
  color: var(--color-text-secondary);
}
.chain-arrow {
  color: var(--color-text-muted);
  font-size: var(--font-size-heading);
}
</style>

<!--
这是从需求到交付的完整工具链路：

**需求阶段**

工具：Superpowers brainstorm
作用：精炼需求，避免理解偏差
产出：结构化需求描述

**设计阶段**

工具：OpenSpec explore → propose
作用：生成规范文档，可评审
产出：proposal + design + tasks + specs

**环境规范阶段**

工具：CLAUDE.md + .claude/ 配置
作用：让 AI 理解项目上下文
产出：规则文件、上下文配置

**实现阶段**

工具：OpenSpec apply + Superpowers TDD
作用：按规范执行，强制测试
产出：代码 + 测试 + 文档

**收尾阶段**

工具：OpenSpec archive
作用：归档沉淀，可追溯
产出：归档的变更记录

这个框架就是" Harness"的具体体现——每一步都有明确的工具和产出。
-->