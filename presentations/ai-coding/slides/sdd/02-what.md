# 什么是 SDD？

<div class="mt-8">

<v-clicks>

> **规格驱动开发（Spec-Driven Development）**
>
> 在写任何一行代码之前，先锁定机器可读、人可评审的规格文档。

</v-clicks>

<v-click>

<div class="mt-8 flex justify-center">

```mermaid {scale: 0.75}
graph LR
    A[Spec<br/>定义是什么] --> B[Design<br/>定义怎么做]
    B --> C[Implement<br/>执行实现]

    style A fill:#e3f2fd,stroke:#1976d2,stroke-width:2px
    style B fill:#bbdefb,stroke:#1976d2,stroke-width:2px
    style C fill:#90caf9,stroke:#1976d2,stroke-width:2px
```

</div>

</v-click>

<v-clicks>

<div class="mt-6 grid grid-cols-2 gap-6">

<div class="p-4 bg-red-50 dark:bg-red-900/20 rounded-lg border border-red-300 dark:border-red-800">

**❌ 传统方式的问题**

- 需求淹没在聊天历史中
- 模糊提示导致不确定输出
- 多个功能混在一起
- 团队不知情，难以协作

</div>

<div class="p-4 bg-green-50 dark:bg-green-900/20 rounded-lg border border-green-300 dark:border-green-800">

**✅ SDD 的优势**

- 独立规范文件夹，可追溯
- 明确规范带来可预测结果
- 每个变更独立文件夹结构
- 规范文档可共享和审查

</div>

</div>

</v-clicks>

</div>
