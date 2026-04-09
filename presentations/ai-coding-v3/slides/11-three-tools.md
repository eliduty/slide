---
layout: TwoCols
---

::left::

# 2.1 三大工具概览

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

<div class="collab-diagram">
<strong>协作关系</strong>
<pre>
        Claude Code（执行引擎）
              ↑
    ┌─────────┴─────────┐
    │                   │
OpenSpec            Superpowers
（规格管理）          （能力模块）
</pre>
</div>

<div class="learning-ref">
<strong>学习资源：</strong>
<ul>
<li>Claude Code 官方文档</li>
<li>Superpowers 完全指南（workspace/ai-coding/drafts/）</li>
<li>OpenSpec 完全指南（workspace/ai-coding/drafts/）</li>
</ul>
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
.collab-diagram {
  background: var(--color-bg-subtle);
  padding: var(--spacing-md);
  border-radius: var(--radius-md);
  margin-bottom: var(--spacing-md);
}
.collab-diagram pre {
  font-family: var(--font-family-code);
  font-size: 13px;
  line-height: 1.5;
  color: var(--color-text-primary);
}
.learning-ref {
  padding: var(--spacing-sm);
  background: var(--color-info-light);
  border-radius: var(--radius-md);
  font-size: var(--font-size-card-body);
}
.learning-ref ul {
  margin-top: var(--spacing-xs);
  margin-left: var(--spacing-md);
}
</style>

<!--
三大工具的核心定位：

**Claude Code：执行引擎**

它是"干活的主力"。能读文件、跑命令、写代码、自主验证。所有实际的代码生成、文件操作都由它完成。

**OpenSpec：规格管理**

它提供了一套完整的工作流：propose → explore → apply → archive。每个阶段都有明确的产出物，确保规格驱动开发的落地。

**Superpowers：能力模块**

它是一组由AI skill 组成的集合，专项能力：强制 TDD、brainstorm、系统化调试。这些是"专项技能"，让AI编程在特定场景下表现更好、输出高质量的代码。

**协作关系**

OpenSpec 和 Superpowers 都"挂"在 Claude Code 上。OpenSpec 管流程，Superpowers 管能力，Claude Code 管执行。

这三个工具下来，可能还需要大家花些时间去深入的了解。
-->
