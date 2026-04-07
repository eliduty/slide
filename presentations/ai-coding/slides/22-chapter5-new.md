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
**场景1：从需求到技术方案的"冷启动"**

新项目最大的挑战是从零建立上下文。

**第一步**：用 AI 把模糊需求结构化，产出需求文档。
**第二步**：让 AI 提出技术方案选项并比较优劣。
**第三步**：你做决策后，让 AI 生成详细技术设计。

每一步的产出物都要固化成文件，作为后续对话的上下文输入。

**场景2：项目脚手架生成**

让 AI 生成项目初始结构、配置文件、CI/CD 管道。这是 AI 效率最高的场景之一。但要注意：必须提供明确的技术栈约束。

我们 skill 项目就是用 Monorepo + pnpm workspace 结构，这个结构就是 AI 帮我们生成的。

**场景3：接口契约先行**

前后端并行开发时，先用 AI 生成完整的 API 契约。AI 很擅长这个，但你需要审查：字段命名是否一致、错误码是否规范、分页过滤等通用模式是否符合团队标准。

**场景4：原型快速验证**

让 AI 快速生成可交互原型，用于和 PM 或业务方确认方向。这里的关键不是代码质量，而是速度。

但我要强调：**原型代码是一次性的**。确认方向后，要基于正式的技术设计重新实现，不要在原型上"长"出正式产品。

**场景5：上下文工程的初始化**

新项目启动时就建立好 AI 协作的基础设施：
- CLAUDE.md——项目规则文件
- .claude/rules/——开发规范
- .claude/skills/——Skills 配置

这些前期投入会在后续开发中持续产生回报。

**场景6：测试策略前置**

新项目的优势是可以从一开始就建立测试体系。让 AI 基于技术设计文档生成测试策略、测试用例框架、mock 数据方案。在写第一行业务代码之前就把测试基础设施搭好。
-->