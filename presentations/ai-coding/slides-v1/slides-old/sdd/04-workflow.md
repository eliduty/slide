# OpenSpec 工作流

<div class="flex justify-center mt-4">

<div class="p-6 bg-gray-50 dark:bg-gray-800/50 rounded-xl">

```mermaid
graph LR
    A[propose<br/>创建提案] --> B[explore<br/>探索代码库]
    B --> C[apply<br/>执行任务]
    C --> D[archive<br/>归档变更]

    style A fill:#e3f2fd,stroke:#1976d2,stroke-width:2px
    style B fill:#e8f5e9,stroke:#388e3c,stroke-width:2px
    style C fill:#fff3e0,stroke:#f57c00,stroke-width:2px
    style D fill:#f3e5f5,stroke:#7b1fa2,stroke-width:2px
```

</div>

</div>

<div class="grid grid-cols-2 gap-4 mt-6">

<div class="p-4 bg-blue-50 dark:bg-blue-900/20 rounded-lg">

### /opsx:propose

<div class="text-sm mt-2 opacity-80">

创建变更文件夹，自动生成：
- proposal.md
- specs/
- design.md
- tasks.md

</div>

</div>

<div class="p-4 bg-green-50 dark:bg-green-900/20 rounded-lg">

### /opsx:explore

<div class="text-sm mt-2 opacity-80">

探索代码库和需求

- 调查问题
- 需求不明确时使用

</div>

</div>

<div class="p-4 bg-orange-50 dark:bg-orange-900/20 rounded-lg">

### /opsx:apply

<div class="text-sm mt-2 opacity-80">

执行任务

- 读取 tasks.md
- 按顺序实现
- 生成代码

</div>

</div>

<div class="p-4 bg-purple-50 dark:bg-purple-900/20 rounded-lg">

### /opsx:archive

<div class="text-sm mt-2 opacity-80">

归档完成的变更

- 移动到 archive/
- 保留历史记录

</div>

</div>

</div>
