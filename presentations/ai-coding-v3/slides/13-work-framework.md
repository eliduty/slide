---
layout: Default
---

# 2.3 工作开展框架

<div class="workflow-diagram">
<pre>
┌─────────────────────────────────────────────────────────────┐
│                                                             │
│   需求阶段                                                   │
│   └── Superpowers brainstorm 精炼需求                       │
│                    ↓                                        │
│   设计阶段                                                   │
│   └── OpenSpec explore → propose → 评审                      │
│                    ↓                                        │
│   环境规范阶段                                               │
│   └── CLAUDE.md + .claude/ 配置上下文                        │
│                    ↓                                        │
│   实现阶段                                                   │
│   └── OpenSpec apply + Superpowers TDD                      │
│                    ↓                                        │
│   收尾阶段                                                   │
│   └── OpenSpec archive → E2E测试、人工验收                    │
│                                                             │
└─────────────────────────────────────────────────────────────┘
</pre>
</div>

<div class="tools-table">

| 阶段 | 核心工具 | 一句话作用 |
|:---:|:---|:---|
| 需求 | brainstorm | 精炼需求，避免理解偏差 |
| 设计 | propose/explore | 生成规范文档，可评审 |
| 环境规范 | CLAUDE.md | 让 AI 理解项目上下文 |
| 实现 | apply + TDD | 按规范执行，强制测试 |
| 收尾 | archive | 归档沉淀，可追溯 |

</div>

<style>
.workflow-diagram {
  background: var(--color-bg-subtle);
  padding: var(--spacing-md);
  border-radius: var(--radius-md);
  margin-bottom: var(--spacing-md);
}
.workflow-diagram pre {
  font-family: var(--font-family-code);
  font-size: 12px;
  line-height: 1.5;
  color: var(--color-text-primary);
  text-align: center;
}
.tools-table {
  font-size: 14px;
}
.tools-table table {
  width: 100%;
  border-collapse: collapse;
}
.tools-table th {
  background: var(--color-primary);
  color: var(--color-bg-card);
  padding: var(--spacing-xs) var(--spacing-sm);
  text-align: left;
  font-weight: var(--font-weight-medium);
}
.tools-table td {
  padding: var(--spacing-xs) var(--spacing-sm);
  border-bottom: 1px solid var(--color-border);
}
.tools-table tr:nth-child(even) {
  background: var(--color-bg-subtle);
}
</style>

<!--
这是从需求到交付的完整工具链路图。

**需求阶段**
- 使用 Superpowers brainstorm 精炼需求
- 把模糊的想法变成结构化的描述

**设计阶段**
- 使用 OpenSpec explore 探索方案
- 使用 propose 生成规范文档
- 经过评审后再进入下一阶段

**环境规范阶段**
- 配置 CLAUDE.md 让 AI 理解项目
- 配置 .claude/ 目录下的规则和技能

**实现阶段**
- 使用 OpenSpec apply 按规范执行
- 配合 Superpowers TDD 强制测试驱动

**收尾阶段**
- 使用 OpenSpec archive 归档变更
- 进行 E2E 测试和人工验收

每个阶段都有对应的工具和明确的产出，形成完整的闭环。
-->
