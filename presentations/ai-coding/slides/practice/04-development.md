# 开发阶段（核心流程）

<div class="flex justify-center mt-4">

<div class="p-5 bg-gray-50 dark:bg-gray-800/50 rounded-xl">

```mermaid
graph TB
    A[PRD功能模块] --> B[explore<br/>探索代码库]
    B --> C[propose<br/>创建提案]
    C --> D[apply<br/>执行任务]
    D --> E[verify<br/>验证结果]
    E --> F[archive<br/>归档沉淀]

    style A fill:#e8f5e9,stroke:#388e3c,stroke-width:2px
    style B fill:#e3f2fd,stroke:#1976d2,stroke-width:2px
    style C fill:#bbdefb,stroke:#1976d2,stroke-width:2px
    style D fill:#fff3e0,stroke:#f57c00,stroke-width:2px
    style E fill:#fce4ec,stroke:#c2185b,stroke-width:2px
    style F fill:#f3e5f5,stroke:#7b1fa2,stroke-width:2px
```

</div>

</div>

<v-clicks>

<div class="mt-4 grid grid-cols-3 gap-3">

<div class="p-3 bg-blue-50 dark:bg-blue-900/20 rounded-lg text-sm border-l-4 border-blue-500">

**explore**
探索现有代码库，理解架构

</div>

<div class="p-3 bg-blue-50 dark:bg-blue-900/20 rounded-lg text-sm border-l-4 border-blue-400">

**propose**
生成 proposal、design、spec、task

</div>

<div class="p-3 bg-orange-50 dark:bg-orange-900/20 rounded-lg text-sm border-l-4 border-orange-500">

**apply**
按 tasks.md 逐项执行，触发 superpowers

</div>

</div>

<div class="mt-3 grid grid-cols-2 gap-3 max-w-2xl mx-auto">

<div class="p-3 bg-pink-50 dark:bg-pink-900/20 rounded-lg text-sm border-l-4 border-pink-500">

**verify**
运行测试，验证实现符合规格

</div>

<div class="p-3 bg-purple-50 dark:bg-purple-900/20 rounded-lg text-sm border-l-4 border-purple-500">

**archive**
归档变更，知识固化到主规格

</div>

</div>

</v-clicks>
