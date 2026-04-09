---
layout: Default
---

# 2.3 工作开展框架

<div class="workflow-container">

<div class="workflow-flow">

<div class="phase-card phase-requirement">
<div class="phase-badge">01</div>
<div class="phase-content">
<div class="phase-name">需求阶段</div>
<div class="phase-tool">Superpowers brainstorm 精炼需求</div>
</div>
<div class="phase-arrow"></div>
</div>

<div class="phase-card phase-design">
<div class="phase-badge">02</div>
<div class="phase-content">
<div class="phase-name">设计阶段</div>
<div class="phase-tool">OpenSpec explore → propose → 评审</div>
</div>
<div class="phase-arrow"></div>
</div>

<div class="phase-card phase-env">
<div class="phase-badge">03</div>
<div class="phase-content">
<div class="phase-name">环境规范阶段</div>
<div class="phase-tool">CLAUDE.md + .claude/ 配置上下文</div>
</div>
<div class="phase-arrow"></div>
</div>

<div class="phase-card phase-impl">
<div class="phase-badge">04</div>
<div class="phase-content">
<div class="phase-name">实现阶段</div>
<div class="phase-tool">OpenSpec apply + Superpowers TDD</div>
</div>
<div class="phase-arrow"></div>
</div>

<div class="phase-card phase-final">
<div class="phase-badge">05</div>
<div class="phase-content">
<div class="phase-name">收尾阶段</div>
<div class="phase-tool">OpenSpec verify、archive → E2E测试、人工验收</div>
</div>
</div>

</div>

<div class="tools-summary">

<div class="tools-header">
<div class="header-item">阶段</div>
<div class="header-item">核心工具</div>
<div class="header-item header-desc">一句话作用</div>
</div>

<div class="tool-row">
<div class="row-phase"><span class="phase-dot dot-requirement"></span>需求</div>
<div class="row-tool">brainstorm+plan</div>
<div class="row-desc">精炼需求，避免理解偏差</div>
</div>

<div class="tool-row">
<div class="row-phase"><span class="phase-dot dot-design"></span>设计</div>
<div class="row-tool">explore+propose</div>
<div class="row-desc">生成规范文档，可评审</div>
</div>

<div class="tool-row">
<div class="row-phase"><span class="phase-dot dot-env"></span>环境规范</div>
<div class="row-tool">CLAUDE.md</div>
<div class="row-desc">让 AI 理解项目上下文</div>
</div>

<div class="tool-row">
<div class="row-phase"><span class="phase-dot dot-impl"></span>实现</div>
<div class="row-tool">apply + TDD</div>
<div class="row-desc">按规范执行，强制测试</div>
</div>

<div class="tool-row">
<div class="row-phase"><span class="phase-dot dot-final"></span>收尾</div>
<div class="row-tool">verify+archive</div>
<div class="row-desc">归档沉淀，可追溯</div>
</div>

</div>

</div>

<style>
.workflow-container {
  display: flex;
  flex-direction: column;
  gap: var(--spacing-lg);
}

.workflow-flow {
  display: flex;
  justify-content: space-between;
  align-items: stretch;
  gap: var(--spacing-xs);
}

.phase-card {
  flex: 1;
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: var(--spacing-sm) var(--spacing-xs);
  border-radius: var(--radius-md);
  border: 1px solid;
  position: relative;
}

.phase-requirement {
  background: linear-gradient(135deg, var(--color-success-light) 0%, rgba(34, 197, 94, 0.05) 100%);
  border-color: var(--color-success);
}

.phase-design {
  background: linear-gradient(135deg, var(--color-info-light) 0%, rgba(59, 130, 246, 0.05) 100%);
  border-color: var(--color-info);
}

.phase-env {
  background: linear-gradient(135deg, var(--color-accent-teal-light) 0%, rgba(20, 184, 166, 0.05) 100%);
  border-color: var(--color-accent-teal);
}

.phase-impl {
  background: linear-gradient(135deg, var(--color-warning-light) 0%, rgba(245, 158, 11, 0.05) 100%);
  border-color: var(--color-warning);
}

.phase-final {
  background: linear-gradient(135deg, var(--color-accent-orange-light) 0%, rgba(249, 115, 22, 0.05) 100%);
  border-color: var(--color-accent-orange);
}

.phase-badge {
  font-family: var(--font-family-display);
  font-weight: var(--font-weight-bold);
  font-size: 22px;
  color: var(--color-bg-card);
  width: 36px;
  height: 36px;
  border-radius: var(--radius-md);
  display: flex;
  align-items: center;
  justify-content: center;
  margin-bottom: var(--spacing-xs);
}

.phase-requirement .phase-badge { background: var(--color-success); }
.phase-design .phase-badge { background: var(--color-info); }
.phase-env .phase-badge { background: var(--color-accent-teal); }
.phase-impl .phase-badge { background: var(--color-warning); }
.phase-final .phase-badge { background: var(--color-accent-orange); }

.phase-content {
  text-align: center;
  flex: 1;
}

.phase-name {
  font-family: var(--font-family-display);
  font-weight: var(--font-weight-semibold);
  font-size: 14px;
  color: var(--color-text-primary);
  margin-bottom: 4px;
}

.phase-tool {
  font-size: 11px;
  color: var(--color-text-secondary);
  line-height: 1.4;
}

.phase-arrow {
  position: absolute;
  right: -10px;
  top: 50%;
  transform: translateY(-50%);
  width: 0;
  height: 0;
  border-top: 6px solid transparent;
  border-bottom: 6px solid transparent;
  border-left: 8px solid var(--color-border);
  opacity: 0.6;
}

.phase-card:last-child .phase-arrow {
  display: none;
}

.tools-summary {
  background: var(--color-bg-subtle);
  border-radius: var(--radius-md);
  overflow: hidden;
  border: 1px solid var(--color-border);
}

.tools-header {
  display: grid;
  grid-template-columns: 100px 140px 1fr;
  background: transparent;
  color: var(--color-text-primary);
  font-weight: var(--font-weight-semibold);
  font-size: 14px;
  border-bottom: 1px solid var(--color-border);
}

.header-item {
  padding: var(--spacing-xs) var(--spacing-sm);
}

.header-desc {
  padding-left: var(--spacing-md);
}

.tool-row {
  display: grid;
  grid-template-columns: 100px 140px 1fr;
  padding: var(--spacing-xs) var(--spacing-sm);
  border-bottom: 1px solid var(--color-border);
  font-size: 13px;
  align-items: center;
}

.tool-row:last-child {
  border-bottom: none;
}

.tool-row:nth-child(even) {
  background: rgba(0, 0, 0, 0.02);
}

.row-phase {
  display: flex;
  align-items: center;
  gap: 6px;
  font-weight: var(--font-weight-medium);
  color: var(--color-text-primary);
}

.phase-dot {
  width: 8px;
  height: 8px;
  border-radius: 50%;
  flex-shrink: 0;
}

.dot-requirement { background: var(--color-success); }
.dot-design { background: var(--color-info); }
.dot-env { background: var(--color-accent-teal); }
.dot-impl { background: var(--color-warning); }
.dot-final { background: var(--color-accent-orange); }

.row-tool {
  font-family: var(--font-family-code);
  font-size: 12px;
  color: var(--color-primary);
  font-weight: var(--font-weight-medium);
}

.row-desc {
  color: var(--color-text-secondary);
  padding-left: var(--spacing-md);
}
</style>

<!--
那么他们是如何完用他们搭建起整个框架的呢？这是从需求到交付的完整工具链路图。

**需求阶段**
- 使用 Superpowers brainstorm 精炼需求
- 把模糊的想法变成结构化的描述

**设计阶段**
- 可以直接使用Claude Code 的Plan模式设计方案
- 也可以使用 OpenSpec explore 探索方案
- 使用 propose 他会生成3个生成规范的spec文档、proposal.md、design.md、task.md
- 经过评审后再进入下一阶段
- 这一阶段建议将对应的测试任务也设计进去，比如我们项目中采用的就是“金字塔测试”，前端：单元测试、组件测试、E2E（UI自动化），后端：单元测试、集成测试、E2E(接口自动化)

**环境规范阶段**
- 在前面的设计阶段可能会识别出一些规范和规则
- 可以配置到 CLAUDE.md 让 AI 理解项目
- 配置 .claude/ 目录下的规则和技能
- 实际上环境规范是需要贯穿我们整个流程，不断优化调整的，他并不固定在这个阶段。

**实现阶段**
- 使用 OpenSpec apply 更具tasks.md中定义的任务执行，对应认为执行完成会对这项任务做标记，就好比我们平时使用的TODO List
- 另外在执行阶段，会强制触发 Superpowers 采用TDD进行开发
- 这有一个经验分享给大家，如果任务比较大，可以用apply分阶段执行，执行完后清除对话，从新执行下一阶段，这样可以有效避免AI幻觉导致输出的质量不高。

**收尾阶段**
- verify 验证所有任务是否开发完成、是否符合设计。
- 另外可以跑一些 E2E 测试和人工验收
- 最后使用 OpenSpec archive 归档变更
- 最终归档后的内容就可以作为项目的规范和沉淀、并且可追溯
- 后期维护的时候又走整套流程，归档的时候会如果是以前有的需求会自动和以前的需求进行合并。


每个阶段都有对应的工具和明确的产出，最终形成完整的可追溯、可迭代的完整闭环。
-->
