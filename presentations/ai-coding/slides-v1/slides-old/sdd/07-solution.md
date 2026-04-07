# 完整方案

<div class="p-4 bg-blue-50 dark:bg-blue-900/20 rounded-lg border-l-4 border-blue-500 mt-4">

**Claude Code + OpenSpec + Superpowers**

三者协同，构建完整的 AI 编程工作流

</div>

<div class="flex justify-center mt-6">

<div class="p-6 bg-gray-50 dark:bg-gray-800/50 rounded-xl">

```mermaid
graph LR
    A[OpenSpec<br/>规范生成] --> B[Superpowers<br/>规范审查/优化]
    B --> C[Claude Code<br/>代码执行/验证]
    C --> B

    style A fill:#e3f2fd,stroke:#1976d2,stroke-width:2px
    style B fill:#e8f5e9,stroke:#388e3c,stroke-width:2px
    style C fill:#fff3e0,stroke:#f57c00,stroke-width:2px
```

</div>

</div>

<div class="grid grid-cols-3 gap-4 mt-6">

<div class="p-4 bg-blue-50 dark:bg-blue-900/20 rounded-lg">

### OpenSpec

<div class="text-sm mt-2 opacity-80">

结构化规范

- 定义"是什么"
- 生成规范文档
- 可追溯、可沉淀

</div>

</div>

<div class="p-4 bg-green-50 dark:bg-green-900/20 rounded-lg">

### Superpowers

<div class="text-sm mt-2 opacity-80">

自动化能力增强

- 审查和优化规范
- TDD 质量保证
- 结构化工作流

</div>

</div>

<div class="p-4 bg-orange-50 dark:bg-orange-900/20 rounded-lg">

### Claude Code

<div class="text-sm mt-2 opacity-80">

深度代码理解

- 根据规范执行
- 自主编程
- 验证结果

</div>

</div>

</div>
