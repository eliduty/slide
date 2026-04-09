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
**大型遗留项目治理的常见场景**

这里列了六个常见场景，每个场景都有对应的策略：

**场景1：上下文窗口爆炸**
策略：分层摘要（项目→模块→文件）
关键：目录树+关键文件代替全量代码

**场景2：故障定位**
流程：AI分析堆栈→人筛选方向→AI深入
关键：不让AI同时猜方向和找细节

**场景3：局部重构**
流程：AI分析依赖→生成回归测试→小步验证
关键：每一步人工确认

**场景4：补测试**
流程：AI生成行为描述→人确认→生成测试
避坑：不要说"给这个文件写测试"

**场景5：文档补全**
流程：AI反向生成→人逐条审核
关键：分模块进行，逐模块确认

**场景6：模块化拆分**
原则：拆分策略人来定，AI只执行
关键：明确当前状态和目标状态

接下来是新项目启动的场景。
-->
