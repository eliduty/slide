# OpenSpec 工件体系

<v-click>

<div class="text-sm opacity-70 mb-4">每个变更（Change）都被组织在独立的文件夹中：</div>

</v-click>

<div class="grid grid-cols-4 gap-3">

<div v-click class="p-3 bg-blue-50 dark:bg-blue-900/20 rounded-lg">

### proposal.md

<div class="text-xs mt-2 opacity-80">

**为什么做**
- 变更初衷
- 目标范围
- 风险评估
- 回滚计划

</div>

</div>

<div v-click class="p-3 bg-green-50 dark:bg-green-900/20 rounded-lg">

### specs/

<div class="text-xs mt-2 opacity-80">

**逻辑规格**
- 场景描述
- Given/When/Then
- 功能需求
- 非功能需求

</div>

</div>

<div v-click class="p-3 bg-purple-50 dark:bg-purple-900/20 rounded-lg">

### design.md

<div class="text-xs mt-2 opacity-80">

**技术方案**
- 架构概述
- 组件设计
- 数据设计
- API 设计

</div>

</div>

<div v-click class="p-3 bg-orange-50 dark:bg-orange-900/20 rounded-lg">

### tasks.md

<div class="text-xs mt-2 opacity-80">

**任务清单**
- 原子化任务
- 执行路径图
- 依赖关系
- 完成标准

</div>

</div>

</div>
