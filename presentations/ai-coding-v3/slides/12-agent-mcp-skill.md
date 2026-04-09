---
layout: Default
---

# 2.2 Agent MCP Skill Memory Rule 概念体系

<div class="concept-header">
<strong>一句话理解六者关系：</strong>
Agent 是"人"，MCP 是"大脑+神经"，Memory 是"记忆"，Skills 是"手脚"，Rules 是"规矩"，Commands 是"动作"
</div>

<div class="concept-diagram">
<pre>
                Agent（统筹一切）
                     │
       ┌─────────────┼─────────────┐
       │             │             │
     MCP          Memory       Rules
   （调度/通信）   （信息支撑）  （行为约束）
       │
   ────┴────
   Skills（执行能力）
       │
   Commands（执行指令）
</pre>
</div>

<div class="config-location">
<strong>实际配置位置：</strong>
<pre>
.claude/
├── skills/     ← 团队专属技能
├── memory/     ← 跨会话记忆
└── rules/      ← 行为约束
</pre>
</div>

<style>
.concept-header {
  padding: var(--spacing-md);
  background: #1A365D;
  border-radius: var(--radius-md);
  color: #FFFFFF;
  font-size: var(--font-size-card-body);
  text-align: center;
  margin-bottom: var(--spacing-md);
}
.concept-diagram {
  background: var(--color-bg-subtle);
  padding: var(--spacing-md);
  border-radius: var(--radius-md);
  margin-bottom: var(--spacing-md);
}
.concept-diagram pre {
  font-family: var(--font-family-code);
  font-size: 14px;
  line-height: 1.6;
  color: var(--color-text-primary);
  text-align: center;
}
.config-location {
  padding: var(--spacing-md);
  background: var(--color-accent-teal-light);
  border-radius: var(--radius-md);
  font-size: var(--font-size-card-body);
}
.config-location pre {
  font-family: var(--font-family-code);
  font-size: 13px;
  margin-top: var(--spacing-xs);
  color: var(--color-text-primary);
}
</style>

<!--
这六个概念，我用一个类比来解释：

**Agent 是"人"**——它是整个系统的主体，统筹一切。

**MCP 是"大脑+神经"**——它负责调度和通信，把各个模块连接起来。

**Memory 是"记忆"**——它存储跨会话的信息，让 Agent 能"记住"之前的事情。

**Skills 是"手脚"**——它是执行能力，Agent 用 Skills 来"干活"。

**Rules 是"规矩"**——它约束 Agent 的行为，告诉它什么能做、什么不能做。

**Commands 是"动作"**——它是具体的执行指令，Skills 里的一个个具体操作。

**实际配置位置**

这些配置都放在 `.claude/` 目录下：
- `skills/`：团队专属技能
- `memory/`：跨会话记忆
- `rules/`：行为约束
-->