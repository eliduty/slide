# AI Agent 核心组件

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
决策、规划、控制
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
具体调用什么工具和操作
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
记住上下文和历史信息
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
权限、安全、行为边界
</div>
</div>

</div>

<div class="mt-6 p-4 bg-gray-50 dark:bg-gray-800/50 rounded-lg border border-gray-200 dark:border-gray-700">

**协作关系**

<div class="mt-2 text-sm text-gray-600 dark:text-gray-300">
Agent 通过 MCP 协议调度各组件，Skill 定义能力边界，Commands 执行具体操作，Memory 保持上下文，Rules 确保安全合规。
</div>

</div>
