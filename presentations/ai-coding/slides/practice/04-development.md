# 开发阶段（核心流程）

<div class="flex justify-center mt-4">

<div class="p-6 bg-gray-50 dark:bg-gray-800/50 rounded-xl">

```mermaid
graph TB
    A[PRD 功能模块] --> B[propose<br/>提案]
    B --> C[explore<br/>探索代码库]
    C --> D[apply<br/>执行]
    D --> E[archive<br/>归档]

    style A fill:#e3f2fd,stroke:#1976d2,stroke-width:2px
    style B fill:#e8f5e9,stroke:#388e3c,stroke-width:2px
    style C fill:#fff3e0,stroke:#f57c00,stroke-width:2px
    style D fill:#fce4ec,stroke:#c2185b,stroke-width:2px
    style E fill:#f3e5f5,stroke:#7b1fa2,stroke-width:2px
```

</div>

</div>

<div class="grid grid-cols-2 gap-4 mt-6">

<div class="p-4 bg-blue-50 dark:bg-blue-900/20 rounded-lg">

### propose（提案）

<div class="text-sm mt-2 opacity-80">

生成规范文档：
- proposal.md（变更提案）
- design.md（技术设计）
- spec（功能规格）
- task（任务列表）

</div>

</div>

<div class="p-4 bg-green-50 dark:bg-green-900/20 rounded-lg">

### explore（探索）

<div class="text-sm mt-2 opacity-80">

探索代码库：
- 理解现有架构
- 找到相关代码
- 评估影响范围

</div>

</div>

<div class="p-4 bg-orange-50 dark:bg-orange-900/20 rounded-lg">

### apply（执行）

<div class="text-sm mt-2 opacity-80">

执行任务：
- 读取 tasks.md
- 触发 superpowers
- 生成代码

</div>

</div>

<div class="p-4 bg-purple-50 dark:bg-purple-900/20 rounded-lg">

### archive（归档）

<div class="text-sm mt-2 opacity-80">

归档变更：
- 移动到 archive/
- 保留历史记录
- 便于追溯

</div>

</div>

</div>
