# Claude Code Agent 循环

<div class="mt-8 flex justify-center">

```mermaid {scale: 0.85}
graph LR
    A[Gather Context<br/>收集上下文] --> B[Take Action<br/>采取行动]
    B --> C[Verify Results<br/>验证结果]
    C --> A

    style A fill:#4caf50,color:#fff
    style B fill:#2196f3,color:#fff
    style C fill:#ff9800,color:#fff
```

</div>

<v-clicks>

<div class="mt-8 grid grid-cols-3 gap-4">

<div class="p-4 bg-green-50 dark:bg-green-900/20 rounded-lg">

**收集上下文**
- 文件搜索
- Git 状态检查
- 读取 CLAUDE.md

</div>

<div class="p-4 bg-blue-50 dark:bg-blue-900/20 rounded-lg">

**采取行动**
- 跨文件编辑
- 终端工具操作
- 执行重构

</div>

<div class="p-4 bg-orange-50 dark:bg-orange-900/20 rounded-lg">

**验证结果**
- 自动运行测试
- 捕捉错误
- 调整方案

</div>

</div>

</v-clicks>
