# 什么是 SDD？

<v-clicks>

<div class="p-4 bg-blue-50 dark:bg-blue-900/20 rounded-lg border-l-4 border-blue-500">

> **规格驱动开发（Spec-Driven Development）**
>
> 在写任何一行代码之前，先锁定机器可读、人可评审的规格文档。

</div>

</v-clicks>

<v-click>

<div class="flex justify-center mt-8">

<div class="p-6 bg-gray-50 dark:bg-gray-800/50 rounded-xl">

```mermaid
graph LR
    A[Spec<br/>定义是什么] --> B[Design<br/>定义怎么做]
    B --> C[Implement<br/>执行实现]

    style A fill:#e3f2fd,stroke:#1976d2,stroke-width:3px,color:#1565c0
    style B fill:#bbdefb,stroke:#1976d2,stroke-width:3px,color:#0d47a1
    style C fill:#90caf9,stroke:#1976d2,stroke-width:3px,color:#0d47a1
```

</div>

</div>

</v-click>

<v-clicks>

<div class="mt-6 grid grid-cols-2 gap-6">

<div class="p-4 bg-red-50 dark:bg-red-900/20 rounded-lg border-l-4 border-red-500">

**❌ 传统方式的问题**

- 需求淹没在聊天历史中
- 模糊提示导致不确定输出
- 多个功能混在一起
- 团队不知情，难以协作

</div>

<div class="p-4 bg-green-50 dark:bg-green-900/20 rounded-lg border-l-4 border-green-500">

**✅ SDD 的优势**

- 独立规范文件夹，可追溯
- 明确规范带来可预测结果
- 每个变更独立文件夹结构
- 规范文档可共享和审查

</div>

</div>

</v-clicks>
