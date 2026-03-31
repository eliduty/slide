# OpenSpec 工件体系

<div class="mt-6">

<v-click>

每个变更（Change）都被组织在独立的文件夹中：

</v-click>

<div class="grid grid-cols-4 gap-4 mt-6">

<div v-click class="p-4 bg-blue-50 dark:bg-blue-900/20 rounded-lg">

### proposal.md

<v-clicks>

<div class="text-sm mt-2">

**为什么做**

- 变更初衷
- 目标范围
- 风险评估
- 回滚计划

</div>

</v-clicks>

</div>

<div v-click class="p-4 bg-green-50 dark:bg-green-900/20 rounded-lg">

### specs/

<v-clicks>

<div class="text-sm mt-2">

**逻辑规格**

- 场景描述
- Given/When/Then
- 功能需求
- 非功能需求

</div>

</v-clicks>

</div>

<div v-click class="p-4 bg-purple-50 dark:bg-purple-900/20 rounded-lg">

### design.md

<v-clicks>

<div class="text-sm mt-2">

**技术方案**

- 架构概述
- 组件设计
- 数据设计
- API 设计

</div>

</v-clicks>

</div>

<div v-click class="p-4 bg-orange-50 dark:bg-orange-900/20 rounded-lg">

### tasks.md

<v-clicks>

<div class="text-sm mt-2">

**任务清单**

- 原子化任务
- 执行路径图
- 依赖关系
- 完成标准

</div>

</v-clicks>

</div>

</div>

</div>
