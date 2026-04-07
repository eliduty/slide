---
layout: Default
---

# 2.2 人与AI的边界

| 阶段 | AI 负责 | 人 负责 |
|:----:|:--------|:--------|
| 需求 | 需求推演完善、结构化描述 | 业务目标定义、验收标准确定 |
| 设计 | 技术方案生成、接口契约设计 | 技术选型决策、架构边界定义 |
| 实现 | 根据规范生成代码、测试 | 验证输出质量、处理边界情况 |

<div class="principle-box">
<strong>核心原则</strong> — 决策在人，执行在AI
</div>

<div class="explain">
AI 可以帮你生成方案、生成代码，但决策——做什么、不做什么、怎么做——必须由人来决定。
</div>

<style>
.principle-box {
  margin-top: var(--spacing-lg);
  background: var(--color-primary);
  color: var(--color-bg-card);
  padding: var(--spacing-md) var(--spacing-lg);
  border-radius: var(--radius-md);
  text-align: center;
}
.principle-box strong { font-size: var(--font-size-card-title); }
.explain {
  margin-top: var(--spacing-md);
  padding: var(--spacing-md);
  background: var(--color-accent-teal-light);
  border-radius: var(--radius-md);
  border: 1px solid var(--color-accent-teal);
  font-size: var(--font-size-card-body);
  text-align: center;
  color: var(--color-text-primary);
}
</style>