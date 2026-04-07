---
layout: Default
---

# 5.2 新项目启动

<div class="scenario-grid">

<div class="scenario">
<div class="header"><span class="num">01</span><span class="title">需求到方案</span></div>
<div class="body">
<p><strong>流程：</strong>AI结构化需求→AI提方案→人决策→AI生成设计</p>
<p><strong>关键：</strong>每一步产出物固化成文件</p>
</div>
</div>

<div class="scenario">
<div class="header"><span class="num">02</span><span class="title">项目脚手架</span></div>
<div class="body">
<p><strong>内容：</strong>目录结构、配置文件、CI/CD</p>
<p><strong>要求：</strong>必须提供明确技术栈约束</p>
</div>
</div>

<div class="scenario">
<div class="header"><span class="num">03</span><span class="title">接口契约先行</span></div>
<div class="body">
<p><strong>流程：</strong>生成完整API契约→前后端并行</p>
<p><strong>审查：</strong>字段命名、错误码规范性</p>
</div>
</div>

<div class="scenario">
<div class="header"><span class="num">04</span><span class="title">原型快速验证</span></div>
<div class="body">
<p><strong>目的：</strong>快速生成可交互原型确认方向</p>
<p><strong>提醒：</strong>原型代码是一次性的</p>
</div>
</div>

<div class="scenario">
<div class="header"><span class="num">05</span><span class="title">上下文工程初始化</span></div>
<div class="body">
<p><strong>内容：</strong>CLAUDE.md + rules + Skills</p>
<p><strong>收益：</strong>前期投入持续产生回报</p>
</div>
</div>

<div class="scenario">
<div class="header"><span class="num">06</span><span class="title">测试策略前置</span></div>
<div class="body">
<p><strong>时机：</strong>写第一行业务代码前</p>
<p><strong>内容：</strong>测试策略、用例框架、mock数据</p>
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