---
layout: Default
---

# 5.1 大型遗留项目治理

<div class="scenario-grid">

<div class="scenario">
<div class="header"><span class="num">01</span><span class="title">上下文爆炸</span></div>
<div class="body">
<p><strong>策略：</strong>分层摘要（项目→模块→文件）</p>
<p><strong>关键：</strong>目录树+关键文件代替全量代码</p>
</div>
</div>

<div class="scenario">
<div class="header"><span class="num">02</span><span class="title">故障定位</span></div>
<div class="body">
<p><strong>流程：</strong>AI分析堆栈→人筛选方向→AI深入</p>
<p><strong>关键：</strong>不让AI同时猜方向和找细节</p>
</div>
</div>

<div class="scenario">
<div class="header"><span class="num">03</span><span class="title">局部重构</span></div>
<div class="body">
<p><strong>流程：</strong>AI分析依赖→生成回归测试→小步验证</p>
<p><strong>关键：</strong>每一步人工确认</p>
</div>
</div>

<div class="scenario">
<div class="header"><span class="num">04</span><span class="title">补测试</span></div>
<div class="body">
<p><strong>流程：</strong>AI生成行为描述→人确认→生成测试</p>
<p><strong>避坑：</strong>不要说"给这个文件写测试"</p>
</div>
</div>

<div class="scenario">
<div class="header"><span class="num">05</span><span class="title">文档补全</span></div>
<div class="body">
<p><strong>流程：</strong>AI反向生成→人逐条审核</p>
<p><strong>关键：</strong>分模块进行，逐模块确认</p>
</div>
</div>

<div class="scenario">
<div class="header"><span class="num">06</span><span class="title">模块化拆分</span></div>
<div class="body">
<p><strong>原则：</strong>拆分策略人来定，AI只执行</p>
<p><strong>关键：</strong>明确当前状态和目标状态</p>
</div>
</div>

</div>

<style>
.scenario-grid {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: var(--spacing-sm);
  margin-top: var(--spacing-sm);
}
.scenario {
  padding: var(--spacing-xs) var(--spacing-sm);
  border-radius: var(--radius-md);
  border: 1px solid;
}
.scenario:nth-child(1) { background: var(--color-error-light); border-color: var(--color-error); }
.scenario:nth-child(2) { background: var(--color-warning-light); border-color: var(--color-warning); }
.scenario:nth-child(3) { background: var(--color-info-light); border-color: var(--color-info); }
.scenario:nth-child(4) { background: var(--color-success-light); border-color: var(--color-success); }
.scenario:nth-child(5) { background: var(--color-accent-gold-light); border-color: var(--color-accent-gold); }
.scenario:nth-child(6) { background: var(--color-accent-teal-light); border-color: var(--color-accent-teal); }
.header {
  display: flex;
  align-items: center;
  gap: var(--spacing-xs);
  margin-bottom: 4px;
}
.num {
  font-family: var(--font-family-display);
  width: 22px;
  height: 22px;
  border-radius: var(--radius-sm);
  display: flex;
  align-items: center;
  justify-content: center;
  font-weight: var(--font-weight-semibold);
  font-size: 12px;
  background: var(--color-primary);
  color: var(--color-bg-card);
}
.title {
  font-family: var(--font-family-display);
  font-weight: var(--font-weight-semibold);
  font-size: var(--font-size-card-title);
  color: var(--color-text-primary);
}
.body p { font-size: var(--font-size-card-meta); margin: 3px 0; color: var(--color-text-secondary); line-height: 1.55; }
.body strong { color: var(--color-primary); }
</style>

<!--
**场景1：上下文窗口爆炸**

你接手了一个百万行代码的项目，不可能一次性喂给 AI。怎么办？

**分层摘要策略**：项目级→模块级→文件级。先给 AI 一个高层的架构描述，再逐步展开。

**建立"基座上下文"**：写一份精简的架构描述文档，每次对话开始时先喂给 AI。

**利用目录树+关键文件**：不要把所有代码都喂过去，用目录树让 AI 理解结构，然后只看关键文件。

**场景2：故障定位与修复**

线上出问题了，怎么用 AI 排查？

**第一步**：让 AI 分析错误堆栈和日志，生成可能原因列表。
**第二步**：你根据业务知识筛选方向。
**第三步**：让 AI 在确定方向上深入排查。

**关键点**：不要让 AI 同时猜方向和找细节。方向要你来定，细节可以让 AI 找。

**场景3：局部重构与技术债清理**

要重构某个模块，怎么用 AI？

**第一步**：让 AI 分析目标模块的依赖关系图，明确影响范围。
**第二步**：重构时必须同步生成回归测试。
**第三步**：小步提交，每步验证。

**场景4：补测试**

遗留项目没有测试，怎么补？

**错误做法**：直接让 AI "给这个文件写测试"。它会写出能跑通但断言毫无业务意义的测试。

**正确做法**：
1. 先让 AI 阅读代码，生成行为描述
2. 人确认描述是否准确
3. 再基于确认后的描述生成测试用例

**场景5：文档补全与知识抢救**

老项目文档缺失，怎么用 AI 补？

让 AI 阅读代码反向生成架构文档。但注意：AI 会"脑补"它不确定的部分，你必须逐条审核。建议分模块进行，每个模块产出后由熟悉该模块的人确认。

**场景6：渐进式模块化拆分**

要把单体拆成微服务，怎么用 AI？

拆分策略——按业务域还是按技术层——必须你来决定。AI 只负责执行。要注意让 AI 理解"当前状态"和"目标状态"的差异，否则它会在两者之间反复横跳。
-->