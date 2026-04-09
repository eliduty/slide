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
  gap: var(--spacing-sm);
  margin-top: var(--spacing-sm);
}
.scenario {
  padding: var(--spacing-xs) var(--spacing-sm);
  border-radius: var(--radius-md);
  border: 1px solid;
}
.scenario:nth-child(1) { background: var(--color-accent-orange-light); border-color: var(--color-accent-orange); }
.scenario:nth-child(2) { background: var(--color-info-light); border-color: var(--color-info); }
.scenario:nth-child(3) { background: var(--color-success-light); border-color: var(--color-success); }
.scenario:nth-child(4) { background: var(--color-warning-light); border-color: var(--color-warning); }
.scenario:nth-child(5) { background: var(--color-accent-teal-light); border-color: var(--color-accent-teal); }
.scenario:nth-child(6) { background: var(--color-accent-gold-light); border-color: var(--color-accent-gold); }
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
**新项目启动的常见场景**

同样列了六个常见场景：

**场景1：需求到方案**
流程：AI结构化需求→AI提方案→人决策→AI生成设计
关键：每一步产出物固化成文件

**场景2：项目脚手架**
内容：目录结构、配置文件、CI/CD
要求：必须提供明确技术栈约束

**场景3：接口契约先行**
流程：生成完整API契约→前后端并行
审查：字段命名、错误码规范性

**场景4：原型快速验证**
目的：快速生成可交互原型确认方向
提醒：原型代码是一次性的

**场景5：上下文工程初始化**
内容：CLAUDE.md + rules + Skills
收益：前期投入持续产生回报

**场景6：测试策略前置**
时机：写第一行业务代码前
内容：测试策略、用例框架、mock数据

掌握了两种项目的策略，我们来看看支撑这些实践的标准化资产。
-->
