# AI Agent 核心组件

<div class="flex justify-center mt-4">

<div class="p-6 bg-gray-50 dark:bg-gray-800/50 rounded-xl">

```mermaid
graph TB
    A[Agent<br/>智能体主体] --> M[MCP<br/>调度协议]
    M --> S[Skill<br/>能力模块]
    M --> C[Commands<br/>指令动作]
    M --> Me[Memory<br/>记忆状态]
    M --> R[Rules<br/>规则约束]

    style A fill:#e3f2fd,stroke:#1976d2,stroke-width:2px
    style M fill:#f3e5f5,stroke:#7b1fa2,stroke-width:2px
    style S fill:#e8f5e9,stroke:#388e3c,stroke-width:2px
    style C fill:#fff3e0,stroke:#f57c00,stroke-width:2px
    style Me fill:#fce4ec,stroke:#c2185b,stroke-width:2px
    style R fill:#efebe9,stroke:#5d4037,stroke-width:2px
```

</div>

</div>

<div class="mt-4 grid grid-cols-3 gap-3 text-sm">

<div class="p-3 bg-blue-50 dark:bg-blue-900/20 rounded-lg">
<div class="font-bold">Agent</div>
<div class="text-xs opacity-60 mt-1">决策、规划、控制</div>
</div>

<div class="p-3 bg-purple-50 dark:bg-purple-900/20 rounded-lg">
<div class="font-bold">MCP</div>
<div class="text-xs opacity-60 mt-1">模型上下文协议</div>
</div>

<div class="p-3 bg-green-50 dark:bg-green-900/20 rounded-lg">
<div class="font-bold">Skill</div>
<div class="text-xs opacity-60 mt-1">能力模块</div>
</div>

<div class="p-3 bg-orange-50 dark:bg-orange-900/20 rounded-lg">
<div class="font-bold">Commands</div>
<div class="text-xs opacity-60 mt-1">指令动作</div>
</div>

<div class="p-3 bg-pink-50 dark:bg-pink-900/20 rounded-lg">
<div class="font-bold">Memory</div>
<div class="text-xs opacity-60 mt-1">记忆状态</div>
</div>

<div class="p-3 bg-amber-50 dark:bg-amber-900/20 rounded-lg">
<div class="font-bold">Rules</div>
<div class="text-xs opacity-60 mt-1">规则约束</div>
</div>

</div>
