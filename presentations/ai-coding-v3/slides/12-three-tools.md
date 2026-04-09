---
layout: TwoCols
---

::left::

# 2.2 三大工具概览

<div class="tools-grid">

<div class="tool-item">
<div class="tool-name">Claude Code</div>
<div class="tool-role">执行引擎</div>
<div class="tool-desc">能读文件、跑命令、写代码、自主验证</div>
</div>

<div class="tool-item">
<div class="tool-name">OpenSpec</div>
<div class="tool-role">规格管理</div>
<div class="tool-desc">propose → explore → apply → archive</div>
</div>

<div class="tool-item">
<div class="tool-name">Superpowers</div>
<div class="tool-role">能力模块</div>
<div class="tool-desc">强制 TDD、brainstorm、系统化调试</div>
</div>

</div>

::right::

<div class="collab-container">
<div class="collab-title">协作关系</div>

<div class="architecture-diagram">
<div class="arch-node engine">
<div class="node-badge">C</div>
<div class="node-info">
<div class="node-name">Claude Code</div>
<div class="node-role">执行引擎</div>
</div>
</div>

<div class="connector">
<div class="arrow-line"></div>
<div class="arrow-head"></div>
</div>

<div class="bottom-nodes">
<div class="arch-node spec">
<div class="node-badge">O</div>
<div class="node-info">
<div class="node-name">OpenSpec</div>
<div class="node-role">规格管理</div>
</div>
</div>

<div class="arch-node powers">
<div class="node-badge">S</div>
<div class="node-info">
<div class="node-name">Superpowers</div>
<div class="node-role">能力模块</div>
</div>
</div>
</div>
</div>

<div class="collab-note">
<div class="note-item">
<span class="dot spec-dot"></span>
<span>OpenSpec 管理需求流程规范</span>
</div>
<div class="note-item">
<span class="dot powers-dot"></span>
<span>Superpowers 提供专项能力管开发流程规范</span>
</div>
<div class="note-item">
<span class="dot engine-dot"></span>
<span>Claude Code 统一执行</span>
</div>
</div>
</div>

<style>
.tools-grid {
  display: flex;
  flex-direction: column;
  gap: var(--spacing-sm);
}
.tool-item {
  padding: var(--spacing-sm);
  border-radius: var(--radius-md);
  border: 1px solid var(--color-border);
}
.tool-item:nth-child(1) { background: var(--color-success-light); border-color: var(--color-success); }
.tool-item:nth-child(2) { background: var(--color-info-light); border-color: var(--color-info); }
.tool-item:nth-child(3) { background: var(--color-accent-teal-light); border-color: var(--color-accent-teal); }
.tool-name {
  font-family: var(--font-family-display);
  font-weight: var(--font-weight-medium);
  font-size: var(--font-size-card-title);
  color: var(--color-text-primary);
}
.tool-role {
  font-size: var(--font-size-card-meta);
  color: var(--color-primary);
  font-weight: var(--font-weight-medium);
}
.tool-desc {
  font-size: var(--font-size-card-body);
  color: var(--color-text-secondary);
  margin-top: var(--spacing-xs);
}

/* 右侧协作关系图 */
.collab-container {
  height: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  padding: var(--spacing-md);
}

.collab-title {
  font-family: var(--font-family-display);
  font-size: var(--font-size-subheading);
  font-weight: var(--font-weight-semibold);
  color: var(--color-text-primary);
  margin-bottom: var(--spacing-lg);
  text-align: center;
}

.architecture-diagram {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: var(--spacing-sm);
  width: 100%;
}

.arch-node {
  display: flex;
  align-items: center;
  gap: var(--spacing-sm);
  padding: var(--spacing-sm) var(--spacing-md);
  border-radius: var(--radius-lg);
  border: 1px solid;
}

.arch-node.engine {
  background: var(--color-success-light);
  border-color: var(--color-success);
  width: 220px;
}

.arch-node.spec {
  background: var(--color-info-light);
  border-color: var(--color-info);
  flex: 1;
}

.arch-node.powers {
  background: var(--color-accent-teal-light);
  border-color: var(--color-accent-teal);
  flex: 1;
}

.node-badge {
  font-family: var(--font-family-display);
  font-weight: var(--font-weight-bold);
  font-size: 18px;
  width: 36px;
  height: 36px;
  display: flex;
  align-items: center;
  justify-content: center;
  border-radius: var(--radius-md);
  color: var(--color-bg-card);
  flex-shrink: 0;
}

.arch-node.engine .node-badge { background: var(--color-success); }
.arch-node.spec .node-badge { background: var(--color-info); }
.arch-node.powers .node-badge { background: var(--color-accent-teal); }

.node-name {
  font-family: var(--font-family-display);
  font-weight: var(--font-weight-semibold);
  font-size: var(--font-size-card-title);
  color: var(--color-text-primary);
}

.node-role {
  font-size: var(--font-size-card-meta);
  color: var(--color-text-secondary);
}

.connector {
  display: flex;
  flex-direction: column;
  align-items: center;
  height: 36px;
}

.arrow-line {
  width: 2px;
  flex: 1;
  background: var(--color-border);
}

.arrow-head {
  width: 0;
  height: 0;
  border-left: 6px solid transparent;
  border-right: 6px solid transparent;
  border-bottom: 8px solid var(--color-border);
}

.bottom-nodes {
  display: flex;
  gap: var(--spacing-md);
  width: 100%;
  justify-content: center;
}

.collab-note {
  margin-top: var(--spacing-lg);
  padding: var(--spacing-md);
  background: var(--color-bg-subtle);
  border-radius: var(--radius-md);
  border: 1px solid var(--color-border);
  width: 100%;
}

.note-item {
  display: flex;
  align-items: center;
  gap: var(--spacing-xs);
  font-size: var(--font-size-card-body);
  color: var(--color-text-secondary);
  margin-bottom: var(--spacing-xs);
}

.note-item:last-child {
  margin-bottom: 0;
}

.dot {
  width: 8px;
  height: 8px;
  border-radius: 50%;
  flex-shrink: 0;
}

.dot.spec-dot { background: var(--color-info); }
.dot.powers-dot { background: var(--color-accent-teal); }
.dot.engine-dot { background: var(--color-success); }
</style>

<!--
接下来介绍我们在职业素养测评项目中用于支撑我们工作流的三大工具，他们分别是Claude Code、OpenSpec、Superpowers。
三大工具的核心定位：

**Claude Code：执行引擎**

它是"干活的主力"。能读文件、跑命令、写代码、自主验证。所有实际的代码生成、文件操作都由它完成。

**OpenSpec：规格管理**

它提供了一套完整的工作流：propose → explore → apply → archive。每个阶段都有明确的产出物，确保规格驱动开发的落地。

同类型的工具还有 Github的Spec Kit-重量级、AWS的 kiro-锁定IDE。

选择OpenSpec的主要原因是：轻量、支持市面上大部分的AI开发工具。

**Superpowers：能力模块**

它是一组由AI skill 组成的集合，专项能力：gitworktree、子代理驱动开发、强制 TDD、brainstorm、系统化调试。这些是"专项技能"，让AI编程在特定场景下表现更好、输出高质量的代码。

**协作关系**

OpenSpec 和 Superpowers 都"挂"在 Claude Code 上。OpenSpec 管流程，Superpowers 管能力，Claude Code 管执行。

这三个就是我们整个开发流程的核心，接下来需要大家花些时间去深入的了解。
-->
