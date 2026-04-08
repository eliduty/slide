---
layout: TwoCols
---

::left::

# 上下文工程

<div class="ce-definition">
<div class="def-label">定义</div>
<div class="def-content">管理"在什么时机、给 AI 什么信息"的能力</div>
</div>

<div class="ce-stack">

<div class="stack-layer layer-top">
<div class="layer-badge">L1</div>
<div class="layer-body">
<div class="layer-title">项目层</div>
<div class="layer-info">架构概述 + 技术栈 + 命名规范</div>
<div class="layer-file">CLAUDE.md</div>
</div>
</div>

<div class="stack-layer layer-mid">
<div class="layer-badge">L2</div>
<div class="layer-body">
<div class="layer-title">模块层</div>
<div class="layer-info">模块职责 + 接口契约 + 数据模型</div>
<div class="layer-file">docs/modules/*.md</div>
</div>
</div>

<div class="stack-layer layer-bottom">
<div class="layer-badge">L3</div>
<div class="layer-body">
<div class="layer-title">任务层</div>
<div class="layer-info">当前任务的目标 + 约束 + 期望输出</div>
<div class="layer-file">design.md / tasks.md</div>
</div>
</div>

</div>

::right::

<div class="harness-card">

<div class="harness-head">
<div class="harness-label">Harness Engineering</div>
<div class="harness-title">渐进式披露原则</div>
</div>

<div class="harness-stages">

<div class="stage-row">
<div class="stage-num">01</div>
<div class="stage-info">
<div class="stage-name">需求阶段</div>
<div class="stage-feed">业务背景 + 用户角色</div>
</div>
</div>

<div class="stage-row">
<div class="stage-num">02</div>
<div class="stage-info">
<div class="stage-name">设计阶段</div>
<div class="stage-feed">技术规范 + 架构约束</div>
</div>
</div>

<div class="stage-row">
<div class="stage-num">03</div>
<div class="stage-info">
<div class="stage-name">实现阶段</div>
<div class="stage-feed">具体模块 + 边界情况</div>
</div>
</div>

<div class="stage-row">
<div class="stage-num">04</div>
<div class="stage-info">
<div class="stage-name">验证阶段</div>
<div class="stage-feed">测试结果 + 用户反馈</div>
</div>
</div>

</div>

<div class="harness-footer">
<span class="footer-icon">💡</span>
<span class="footer-msg">不要一次性把所有信息扔给 AI，按阶段逐步喂入</span>
</div>

</div>

<style>
/* 左侧 - 上下文工程 */
.ce-definition {
  display: flex;
  gap: 10px;
  padding: 10px 14px;
  margin-top: 10px;
  border-radius: 8px;
  background: rgba(59, 130, 246, 0.1);
  border: 1px solid rgba(59, 130, 246, 0.3);
}
.def-label {
  font-size: 11px;
  font-weight: 600;
  padding: 3px 6px;
  background: #3b82f6;
  color: white;
  border-radius: 4px;
  height: fit-content;
}
.def-content {
  font-size: 14px;
  color: var(--color-text-primary);
  line-height: 1.4;
}

.ce-stack {
  margin-top: 12px;
  display: flex;
  flex-direction: column;
  gap: 8px;
  position: relative;
}

.stack-layer {
  display: flex;
  gap: 10px;
  padding: 10px 14px;
  border-radius: 8px;
  position: relative;
}

.layer-top { background: rgba(16, 185, 129, 0.12); border: 1px solid rgba(16, 185, 129, 0.4); }
.layer-mid { background: rgba(59, 130, 246, 0.12); border: 1px solid rgba(59, 130, 246, 0.4); }
.layer-bottom { background: rgba(245, 158, 11, 0.12); border: 1px solid rgba(245, 158, 11, 0.4); }

.layer-badge {
  width: 28px;
  height: 28px;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 12px;
  font-weight: 700;
  border-radius: 5px;
  color: white;
}
.layer-top .layer-badge { background: #10b981; }
.layer-mid .layer-badge { background: #3b82f6; }
.layer-bottom .layer-badge { background: #f59e0b; }

.layer-body {
  flex: 1;
}
.layer-title {
  font-size: 14px;
  font-weight: 600;
  color: var(--color-text-primary);
}
.layer-info {
  font-size: 12px;
  color: var(--color-text-secondary);
  margin-top: 1px;
}
.layer-file {
  font-size: 11px;
  color: var(--color-primary);
  margin-top: 2px;
}

/* 右侧 - Harness面板 */
.harness-card {
  background: linear-gradient(135deg, #0f172a 0%, #1e293b 100%);
  border-radius: 12px;
  display: flex;
  flex-direction: column;
  overflow: hidden;
}

.harness-head {
  padding: 10px 14px;
  border-bottom: 1px solid rgba(255,255,255,0.1);
}
.harness-label {
  font-size: 10px;
  font-weight: 600;
  color: #60a5fa;
  letter-spacing: 1px;
}
.harness-title {
  font-size: 15px;
  font-weight: 600;
  color: white;
  margin-top: 2px;
}

.harness-stages {
  padding: 10px 14px;
  display: flex;
  flex-direction: column;
  gap: 6px;
}

.stage-row {
  display: flex;
  align-items: center;
  gap: 10px;
  padding: 8px 10px;
  background: rgba(255,255,255,0.06);
  border-radius: 6px;
  border: 1px solid rgba(255,255,255,0.1);
}

.stage-num {
  width: 26px;
  height: 26px;
  display: flex;
  align-items: center;
  justify-content: center;
  background: rgba(96, 165, 250, 0.2);
  border-radius: 5px;
  font-size: 12px;
  font-weight: 700;
  color: #60a5fa;
}

.stage-info {
  flex: 1;
}

.stage-name {
  font-size: 14px;
  font-weight: 600;
  color: white;
}

.stage-feed {
  font-size: 12px;
  color: rgba(255,255,255,0.6);
}

.harness-footer {
  padding: 10px 14px;
  background: rgba(251, 191, 36, 0.15);
  border-top: 1px solid rgba(251, 191, 36, 0.3);
  display: flex;
  align-items: center;
  gap: 8px;
}
.footer-icon {
  font-size: 14px;
}
.footer-msg {
  font-size: 12px;
  color: rgba(255,255,255,0.9);
}

/* 暗色模式适配 */
.dark .ce-definition {
  background: rgba(59, 130, 246, 0.2);
}
.dark .layer-top { background: rgba(16, 185, 129, 0.2); }
.dark .layer-mid { background: rgba(59, 130, 246, 0.2); }
.dark .layer-bottom { background: rgba(245, 158, 11, 0.2); }
</style>

<!--
现在我们来讲一个关键能力：**上下文工程**。

什么是上下文工程？简单说，就是管理"在什么时机、给 AI 什么信息"的能力。

很多人用 AI 不顺手，不是因为 AI 不行，是因为上下文没给好。上下文给太多，AI 信息过载，抓不住重点；上下文给太少，AI 缺乏背景，瞎猜乱编。

**上下文要分层管理：**

**第一层：项目层**

放在 CLAUDE.md 里。包括：架构概述、技术栈选择、命名规范。这是每次对话的"基座上下文"，AI 每次都会自动读取。

**第二层：模块层**

放在 docs/modules/*.md 里。包括：模块职责、接口契约、数据模型。当你让 AI 做某个模块的开发时，就把对应模块文档喂给它。

**第三层：任务层**

放在 design.md 和 tasks.md 里。包括：当前任务的目标、约束、期望输出。这是最细粒度的上下文，告诉 AI 这一次对话具体要做什么。

**Harness Engineering：渐进式披露**

这是一个专业术语，翻译过来就是"渐进式披露"。什么意思？不要一次性把所有信息扔给 AI，要按阶段逐步喂入。

**需求阶段**：只给业务背景和用户角色。让 AI 理解"我们在做什么"，不要给技术细节，否则 AI 会过早陷入技术实现。

**设计阶段**：给技术规范和架构约束。让 AI 知道"我们用什么技术、有什么限制"，开始生成技术方案。

**实现阶段**：给具体模块和边界情况。让 AI 知道"这个模块的边界在哪、特殊情况怎么处理"，生成高质量代码。

**验证阶段**：给测试结果和用户反馈。让 AI 知道"输出是否正确、哪里需要修正"，形成迭代闭环。这是很多人忽略的一步——AI 生成的代码不是一次就完美的，需要基于反馈持续优化。

**记住一个规则：上下文要分层，披露要渐进。**

一次性喂太多，AI 会迷失；喂太少，AI 会瞎猜。把握好节奏，才能让 AI 发挥最大价值。
-->
