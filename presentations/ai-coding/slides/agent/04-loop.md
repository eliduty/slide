# Claude Code Agent 循环

<div class="flex justify-center mt-6">

<div class="p-6 bg-gray-50 dark:bg-gray-800/50 rounded-xl">

```mermaid
graph LR
    A[Gather Context<br/>收集上下文] --> B[Take Action<br/>采取行动]
    B --> C[Verify Results<br/>验证结果]
    C --> A

    style A fill:#4caf50,stroke:#2e7d32,stroke-width:3px,color:#fff
    style B fill:#2196f3,stroke:#1565c0,stroke-width:3px,color:#fff
    style C fill:#ff9800,stroke:#e65100,stroke-width:3px,color:#fff
```

</div>

</div>

<v-clicks>

<div class="mt-6 grid grid-cols-3 gap-4">

<div class="p-4 bg-green-50 dark:bg-green-900/20 rounded-lg border-l-4 border-green-500">

**收集上下文**
- 文件搜索
- Git 状态检查
- 读取 CLAUDE.md

</div>

<div class="p-4 bg-blue-50 dark:bg-blue-900/20 rounded-lg border-l-4 border-blue-500">

**采取行动**
- 跨文件编辑
- 终端工具操作
- 执行重构

</div>

<div class="p-4 bg-orange-50 dark:bg-orange-900/20 rounded-lg border-l-4 border-orange-500">

**验证结果**
- 自动运行测试
- 捕捉错误
- 调整方案

</div>

</div>

</v-clicks>
