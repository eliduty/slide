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
  gap: 0.4rem;
  margin-top: 0.3rem;
}
.scenario {
  background: var(--color-primary-light);
  padding: 0.5rem;
  border-radius: var(--radius-sm);
}
.header {
  display: flex;
  align-items: center;
  gap: 0.3rem;
  margin-bottom: 0.3rem;
}
.num {
  background: var(--color-primary);
  color: white;
  width: 22px;
  height: 22px;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  font-weight: 600;
  font-size: 0.7rem;
}
.title { font-weight: 600; font-size: 0.85rem; color: var(--color-text-primary); }
.body p { font-size: 0.7rem; margin: 0.1rem 0; color: var(--color-text-secondary); }
.body strong { color: var(--color-primary); }
</style>