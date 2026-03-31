# OpenSpec 工作流

<div class="flex justify-center mt-6">

<div class="p-6 bg-gray-50 dark:bg-gray-800/50 rounded-xl">

```mermaid
graph TB
    P["/opsx:propose<br/>创建提案"] --> E["/opsx:explore<br/>探索想法"]
    E --> A["/opsx:apply<br/>实现任务"]
    A --> AR["/opsx:archive<br/>归档沉淀"]

    style P fill:#4caf50,stroke:#2e7d32,stroke-width:3px,color:#fff
    style E fill:#2196f3,stroke:#1565c0,stroke-width:3px,color:#fff
    style A fill:#ff9800,stroke:#e65100,stroke-width:3px,color:#fff
    style AR fill:#9c27b0,stroke:#6a1b9a,stroke-width:3px,color:#fff
```

</div>

</div>

<v-clicks>

<div class="mt-6 grid grid-cols-2 gap-6 max-w-3xl mx-auto">

<div class="p-4 bg-gray-50 dark:bg-gray-800/50 rounded-lg border border-gray-200 dark:border-gray-700">

**核心命令**

| 命令 | 说明 |
|------|------|
| `/opsx:propose` | 创建变更和规划文档 |
| `/opsx:explore` | 探索想法，调查问题 |
| `/opsx:apply` | 实现任务 |
| `/opsx:archive` | 归档完成的变更 |

</div>

<div class="p-4 bg-gray-50 dark:bg-gray-800/50 rounded-lg border border-gray-200 dark:border-gray-700">

**核心价值**

<v-clicks>

- ✅ 可预测性 — 明确规范带来可预测输出
- ✅ 组织性 — 每个变更独立文件夹结构
- ✅ 灵活性 — 随时更新任何文档
- ✅ 工具自由 — 支持 20+ AI 编码助手

</v-clicks>

</div>

</div>

</v-clicks>
