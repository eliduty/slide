# 开发阶段（核心流程）

<div class="mt-6">

```mermaid {scale: 0.6}
graph TB
    A[PRD功能模块] --> B[explore<br/>探索代码库]
    B --> C[propose<br/>创建提案]
    C --> D[apply<br/>执行任务]
    D --> E[verify<br/>验证结果]
    E --> F[archive<br/>归档沉淀]

    style A fill:#e8f5e9
    style B fill:#e3f2fd
    style C fill:#bbdefb
    style D fill:#fff3e0
    style E fill:#fce4ec
    style F fill:#f3e5f5
```

</div>

<v-clicks>

<div class="mt-6 grid grid-cols-3 gap-4">

<div class="p-3 bg-blue-50 dark:bg-blue-900/20 rounded-lg text-sm">

**explore**
探索现有代码库，理解架构

</div>

<div class="p-3 bg-green-50 dark:bg-green-900/20 rounded-lg text-sm">

**propose**
生成 proposal、design、spec、task

</div>

<div class="p-3 bg-purple-50 dark:bg-purple-900/20 rounded-lg text-sm">

**apply**
按 tasks.md 逐项执行，触发 superpowers

</div>

</div>

<div class="mt-4 grid grid-cols-2 gap-4">

<div class="p-3 bg-orange-50 dark:bg-orange-900/20 rounded-lg text-sm">

**verify**
运行测试，验证实现符合规格

</div>

<div class="p-3 bg-pink-50 dark:bg-pink-900/20 rounded-lg text-sm">

**archive**
归档变更，知识固化到主规格

</div>

</div>

</v-clicks>
