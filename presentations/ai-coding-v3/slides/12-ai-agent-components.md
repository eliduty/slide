---
layout: Default
---

# 2.1 AI Agent 核心组件

<div class="concept-header">
<strong>一句话理解六者关系：</strong>
Agent 是"大脑"，MCP 是"神经"，Memory 是"记忆"，Rules 是"规矩"，Skills 是"手脚"，Commands 是"动作"
</div>

<div class="mt-6 grid grid-cols-3 gap-4">

<div class="p-4 bg-gradient-to-br from-blue-50 to-white dark:from-blue-900/20 dark:to-gray-900/50 rounded-xl border border-blue-100 dark:border-blue-800/30">
<div class="flex items-center gap-3 mb-3">
<div class="w-10 h-10 rounded-lg bg-blue-500 flex items-center justify-center">
<span class="text-white font-bold text-sm">A</span>
</div>
<div>
<div class="font-bold text-blue-700 dark:text-blue-300">Agent</div>
<div class="text-xs text-gray-500 dark:text-gray-400">智能体主体</div>
</div>
</div>
<div class="text-sm text-gray-600 dark:text-gray-300">
统筹决策、规划控制
</div>
</div>

<div class="p-4 bg-gradient-to-br from-purple-50 to-white dark:from-purple-900/20 dark:to-gray-900/50 rounded-xl border border-purple-100 dark:border-purple-800/30">
<div class="flex items-center gap-3 mb-3">
<div class="w-10 h-10 rounded-lg bg-purple-500 flex items-center justify-center">
<span class="text-white font-bold text-sm">M</span>
</div>
<div>
<div class="font-bold text-purple-700 dark:text-purple-300">MCP</div>
<div class="text-xs text-gray-500 dark:text-gray-400">模型上下文协议</div>
</div>
</div>
<div class="text-sm text-gray-600 dark:text-gray-300">
连接外部数据源的开放标准
</div>
</div>

<div class="p-4 bg-gradient-to-br from-pink-50 to-white dark:from-pink-900/20 dark:to-gray-900/50 rounded-xl border border-pink-100 dark:border-pink-800/30">
<div class="flex items-center gap-3 mb-3">
<div class="w-10 h-10 rounded-lg bg-pink-500 flex items-center justify-center">
<span class="text-white font-bold text-sm">M</span>
</div>
<div>
<div class="font-bold text-pink-700 dark:text-pink-300">Memory</div>
<div class="text-xs text-gray-500 dark:text-gray-400">记忆状态</div>
</div>
</div>
<div class="text-sm text-gray-600 dark:text-gray-300">
跨会话持久化存储信息
</div>
</div>

<div class="p-4 bg-gradient-to-br from-amber-50 to-white dark:from-amber-900/20 dark:to-gray-900/50 rounded-xl border border-amber-100 dark:border-amber-800/30">
<div class="flex items-center gap-3 mb-3">
<div class="w-10 h-10 rounded-lg bg-amber-500 flex items-center justify-center">
<span class="text-white font-bold text-sm">R</span>
</div>
<div>
<div class="font-bold text-amber-700 dark:text-amber-300">Rules</div>
<div class="text-xs text-gray-500 dark:text-gray-400">规则约束</div>
</div>
</div>
<div class="text-sm text-gray-600 dark:text-gray-300">
权限边界、安全规范、行为约束
</div>
</div>

<div class="p-4 bg-gradient-to-br from-green-50 to-white dark:from-green-900/20 dark:to-gray-900/50 rounded-xl border border-green-100 dark:border-green-800/30">
<div class="flex items-center gap-3 mb-3">
<div class="w-10 h-10 rounded-lg bg-green-500 flex items-center justify-center">
<span class="text-white font-bold text-sm">S</span>
</div>
<div>
<div class="font-bold text-green-700 dark:text-green-300">Skill</div>
<div class="text-xs text-gray-500 dark:text-gray-400">能力模块</div>
</div>
</div>
<div class="text-sm text-gray-600 dark:text-gray-300">
可复用、可组合的能力单元
</div>
</div>

<div class="p-4 bg-gradient-to-br from-orange-50 to-white dark:from-orange-900/20 dark:to-gray-900/50 rounded-xl border border-orange-100 dark:border-orange-800/30">
<div class="flex items-center gap-3 mb-3">
<div class="w-10 h-10 rounded-lg bg-orange-500 flex items-center justify-center">
<span class="text-white font-bold text-sm">C</span>
</div>
<div>
<div class="font-bold text-orange-700 dark:text-orange-300">Commands</div>
<div class="text-xs text-gray-500 dark:text-gray-400">指令动作</div>
</div>
</div>
<div class="text-sm text-gray-600 dark:text-gray-300">
具体调用工具和操作的指令
</div>
</div>

</div>


<style>
.concept-header {
  padding: var(--spacing-sm) var(--spacing-md);
  background: #1A365D;
  border-radius: var(--radius-md);
  color: #FFFFFF;
  font-size: 15px;
  text-align: center;
  margin-bottom: var(--spacing-sm);
}
.config-location {
  margin-top: var(--spacing-md);
  padding: var(--spacing-sm) var(--spacing-md);
  background: var(--color-accent-teal-light);
  border-radius: var(--radius-md);
  font-size: 14px;
}
.config-location pre {
  font-family: var(--font-family-code);
  font-size: 12px;
  margin-top: var(--spacing-xs);
  color: var(--color-text-primary);
  line-height: 1.6;
}
</style>

<!--
在开始介绍具体的内容前，大家还是有必要先了解一下AI Agent的核心组件。
它们包括：

**Agent（智能体主体）**
Agent 是整个系统的"大脑"，负责统筹决策、规划任务、控制执行流程。它是用户与 AI 系统交互的入口。

**MCP（模型上下文协议）**
MCP 是"神经系统"，负责 Agent 与外部世界的连接。它是一个开放标准协议，让 Agent 能够连接各种数据源、API、工具等外部服务。

**Memory（记忆状态）**
Memory 是"长期记忆"，存储跨会话的信息。它让 Agent 能够"记住"之前的对话、偏好设置、项目背景等，实现真正的连续性。

**Rules（规则约束）**
Rules 是"行为边界"，定义了 Agent 能做什么、不能做什么。包括安全策略、权限控制、编码规范等，确保 AI 行为符合预期。

**Skill（能力模块）**
Skill 是"专业技能"，是可复用的能力单元。比如"Vue 开发规范"、"TDD 流程"等都是 Skill，让 Agent 具备特定领域的专业能力。

这是去年10月Anthropic 推出的，刚推出我就进行了试用，当时确实把我惊艳到了，然后引发了我对重塑工作流的思考。

**Commands（指令动作）**
Commands 是"具体动作"，是 Skills 中的原子操作。比如"读取文件"、"执行命令"、"调用 API"等都是 Commands。

这些都是AI Agent的核心组件，我这只引出概念，如果大家还不了解的，请下来自行学习了解。
-->
