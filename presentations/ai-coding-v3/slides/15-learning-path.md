---
layout: Default
---

# 2.4 学习路径指引

<div class="learning-path">

<div class="level">
<div class="level-header">
<span class="level-num">01</span>
<span class="level-title">初级：会用工具</span>
</div>
<div class="level-body">
<div class="level-check">✓ 了解工作流和安装相关工具</div>
<div class="level-check">✓ 理解四阶段工作流</div>
<div class="level-check">✓ 能用 AI 完成单个任务</div>
</div>
</div>

<div class="level">
<div class="level-header">
<span class="level-num">02</span>
<span class="level-title">中级：能判质量</span>
</div>
<div class="level-body">
<div class="level-check">✓ 参考案例，独立完成简单变更</div>
<div class="level-check">✓ 能判断 AI 输出是否符合预期</div>
<div class="level-check">✓ 能写出合格的 spec 文档</div>
</div>
</div>

<div class="level">
<div class="level-header">
<span class="level-num">03</span>
<span class="level-title">高级：能设计策略</span>
</div>
<div class="level-body">
<div class="level-check">✓ 开发团队Skill，沉淀最佳实践</div>
<div class="level-check">✓ 能设计上下文策略</div>
<div class="level-check">✓ 能指导他人使用 AI Coding</div>
</div>
</div>

</div>

<style>
.learning-path {
  display: flex;
  flex-direction: row;
  gap: var(--spacing-md);
  margin: var(--spacing-md) 0;
  height: calc(100% - 80px);
}

.level {
  flex: 1;
  position: relative;
  border-radius: var(--radius-lg);
  padding: var(--spacing-md);
  background: var(--color-bg-card);
  border: 1px solid var(--color-border);
  box-shadow: var(--shadow-sm);
  overflow: hidden;
  display: flex;
  flex-direction: column;
}

/* 顶部色条 */
.level::before {
  content: '';
  position: absolute;
   left: 0;
  right: 0;
  top: 0;
  height: 4px;
}

.level:nth-child(1)::before { background: linear-gradient(90deg, var(--color-success) 0%, #38A169 100%); }
.level:nth-child(2)::before { background: linear-gradient(90deg, var(--color-info) 0%, #4299E1 100%); }
.level:nth-child(3)::before { background: linear-gradient(90deg, var(--color-accent-teal) 0%, #14B8A6 100%); }

.level-header {
  display: flex;
  align-items: center;
  gap: var(--spacing-sm);
  margin-bottom: var(--spacing-md);
  padding-bottom: var(--spacing-sm);
  border-bottom: 1px dashed var(--color-border-light);
}

.level-num {
  font-family: var(--font-family-display);
  width: 36px;
  height: 36px;
  border-radius: var(--radius-md);
  display: flex;
  align-items: center;
  justify-content: center;
  font-weight: var(--font-weight-bold);
  font-size: 16px;
  color: white;
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.15);
}

.level:nth-child(1) .level-num {
  background: linear-gradient(135deg, var(--color-success) 0%, #38A169 100%);
}
.level:nth-child(2) .level-num {
  background: linear-gradient(135deg, var(--color-info) 0%, #4299E1 100%);
}
.level:nth-child(3) .level-num {
  background: linear-gradient(135deg, var(--color-accent-teal) 0%, #14B8A6 100%);
}

.level-title {
  font-family: var(--font-family-display);
  font-weight: var(--font-weight-semibold);
  font-size: 20px;
  color: var(--color-text-primary);
}

.level-body {
  display: flex;
  flex-direction: column;
  gap: 12px;
}

.level-check {
  position: relative;
  font-size: 14px;
  color: var(--color-text-primary);
  line-height: 1.5;
  padding: 6px 10px;
  border-radius: 6px;
}

/* 彩色背景高亮 */
.level:nth-child(1) .level-check {
  background: var(--color-success-light);
}
.level:nth-child(2) .level-check {
  background: var(--color-info-light);
}
.level:nth-child(3) .level-check {
  background: var(--color-accent-teal-light);
}
</style>

<!--
学习 AI Coding 需要一个循序渐进的过程，我把它分为三个阶段。

**初级：会用工具**

这个阶段的目标是入门。你需要：
- 了解工作流和安装相关工具
- 理解四阶段工作流
- 能用 AI 完成单个任务

**中级：能判质量**

这个阶段的目标是独立工作。你需要：
- 参考变更案例，独立完成简单变更
- 能判断 AI 输出是否符合业务预期
- 能写出合格的 spec 文档

**高级：能设计策略**

这个阶段的目标是沉淀和分享。你需要：
- 开发团队专属 Skill，沉淀最佳实践
- 能设计上下文策略
- 能指导他人使用 AI Coding

**学习资源**

- Superpowers 完全指南（workspace/ai-coding/drafts/）
- OpenSpec 完全指南（workspace/ai-coding/drafts/）
- Claude Code 官方文档

根据自己的水平，选择合适的学习路径。

掌握了工具和学习路径，下面我们进入核心部分：四阶段工作流程的具体实践。
-->
