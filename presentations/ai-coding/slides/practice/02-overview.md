# 全流程概览

<div class="flex justify-center mt-6">

<div class="p-6 bg-gray-50 dark:bg-gray-800/50 rounded-xl">

```mermaid
graph LR
    R[📋 需求] --> D[🎨 设计]
    D --> Dev[⚙️ 开发]
    Dev --> T[🧪 测试]
    T --> DP[🚀 部署]

    style R fill:#e8f5e9,stroke:#388e3c,stroke-width:2px
    style D fill:#e3f2fd,stroke:#1976d2,stroke-width:2px
    style Dev fill:#fff3e0,stroke:#f57c00,stroke-width:2px
    style T fill:#fce4ec,stroke:#c2185b,stroke-width:2px
    style DP fill:#f3e5f5,stroke:#7b1fa2,stroke-width:2px
```

</div>

</div>

<v-clicks>

<div class="mt-6 grid grid-cols-5 gap-3">

<div class="p-4 text-center bg-green-50 dark:bg-green-900/20 rounded-lg border-t-4 border-green-500">
<div class="font-bold text-sm">需求阶段</div>
<div class="text-xs opacity-60 mt-2">PRD → 小系统拆分</div>
</div>

<div class="p-4 text-center bg-blue-50 dark:bg-blue-900/20 rounded-lg border-t-4 border-blue-500">
<div class="font-bold text-sm">设计阶段</div>
<div class="text-xs opacity-60 mt-2">架构 + 技术方案</div>
</div>

<div class="p-4 text-center bg-orange-50 dark:bg-orange-900/20 rounded-lg border-t-4 border-orange-500">
<div class="font-bold text-sm">开发阶段</div>
<div class="text-xs opacity-60 mt-2">OpenSpec 工作流</div>
</div>

<div class="p-4 text-center bg-pink-50 dark:bg-pink-900/20 rounded-lg border-t-4 border-pink-500">
<div class="font-bold text-sm">测试阶段</div>
<div class="text-xs opacity-60 mt-2">E2E + 单元测试</div>
</div>

<div class="p-4 text-center bg-purple-50 dark:bg-purple-900/20 rounded-lg border-t-4 border-purple-500">
<div class="font-bold text-sm">部署阶段</div>
<div class="text-xs opacity-60 mt-2">CI/CD 集成</div>
</div>

</div>

</v-clicks>
