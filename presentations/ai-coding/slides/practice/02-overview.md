# 全流程概览

<div class="mt-8 flex justify-center">

```mermaid {scale: 0.65}
graph LR
    R[需求] --> D[设计]
    D --> Dev[开发]
    Dev --> T[测试]
    T --> DP[部署]

    style R fill:#e8f5e9
    style D fill:#e3f2fd
    style Dev fill:#fff3e0
    style T fill:#fce4ec
    style DP fill:#f3e5f5
```

</div>

<v-clicks>

<div class="mt-8 grid grid-cols-5 gap-4">

<div class="p-4 text-center">
<div class="text-3xl mb-2">📋</div>
<div class="font-bold text-sm">需求阶段</div>
<div class="text-xs opacity-60 mt-1">PRD → 小系统拆分</div>
</div>

<div class="p-4 text-center">
<div class="text-3xl mb-2">🎨</div>
<div class="font-bold text-sm">设计阶段</div>
<div class="text-xs opacity-60 mt-1">架构 + 技术方案</div>
</div>

<div class="p-4 text-center">
<div class="text-3xl mb-2">⚙️</div>
<div class="font-bold text-sm">开发阶段</div>
<div class="text-xs opacity-60 mt-1">OpenSpec 工作流</div>
</div>

<div class="p-4 text-center">
<div class="text-3xl mb-2">🧪</div>
<div class="font-bold text-sm">测试阶段</div>
<div class="text-xs opacity-60 mt-1">E2E + 单元测试</div>
</div>

<div class="p-4 text-center">
<div class="text-3xl mb-2">🚀</div>
<div class="font-bold text-sm">部署阶段</div>
<div class="text-xs opacity-60 mt-1">CI/CD 集成</div>
</div>

</div>

</v-clicks>
