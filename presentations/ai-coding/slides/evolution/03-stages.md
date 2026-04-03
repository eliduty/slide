# 每个阶段的特点

<div class="stages-container mt-6">

<div class="stage-row">
  <div class="stage-marker">
    <span class="stage-year">2022</span>
    <span class="stage-dot"></span>
  </div>
  <div class="stage-card">
    <div class="stage-header">
      <span class="stage-title">Web 对话时代</span>
      <span class="stage-tag">起点</span>
    </div>
    <div class="stage-points">
      <span>上下文断裂 · AI 不知道项目结构</span>
      <span>复制粘贴地狱 · 浏览器与编辑器切换</span>
      <span>无法调试 · AI 看不到运行结果</span>
    </div>
  </div>
</div>

<div class="stage-row">
  <div class="stage-marker">
    <span class="stage-year">2022-23</span>
    <span class="stage-dot"></span>
  </div>
  <div class="stage-card">
    <div class="stage-header">
      <span class="stage-title">编辑器插件时代</span>
      <span class="stage-tag">集成</span>
    </div>
    <div class="stage-points">
      <span>集成但受限 · 嵌入 IDE 按 Tab 补全</span>
      <span>上下文有限 · 只能看到当前文件</span>
      <span>能力边界 · 单文件补全函数级生成</span>
    </div>
  </div>
</div>

<div class="stage-row">
  <div class="stage-marker">
    <span class="stage-year">2024</span>
    <span class="stage-dot"></span>
  </div>
  <div class="stage-card">
    <div class="stage-header">
      <span class="stage-title">AI IDE 时代</span>
      <span class="stage-tag">融合</span>
    </div>
    <div class="stage-points">
      <span>一体化体验 · AI 原生 IDE 对话式编程</span>
      <span>项目级理解 · 通过 RAG 索引代码库</span>
      <span>跨文件修改 · 同时修改多个文件</span>
    </div>
  </div>
</div>

<div class="stage-row">
  <div class="stage-marker">
    <span class="stage-year">2025</span>
    <span class="stage-dot active"></span>
  </div>
  <div class="stage-card highlight">
    <div class="stage-header">
      <span class="stage-title">终端 Agent 时代</span>
      <span class="stage-tag current">当前</span>
    </div>
    <div class="stage-points">
      <span>深度理解 · 项目架构依赖规范</span>
      <span>自主执行 · 自己规划执行验证</span>
      <span>长时间工作 · 连续数小时不偏离</span>
    </div>
  </div>
</div>

</div>

<style>
.stages-container {
  display: flex;
  flex-direction: column;
  position: relative;
  padding-left: 64px;
}

.stage-row {
  display: flex;
  align-items: flex-start;
  gap: 16px;
  position: relative;
  padding-bottom: 14px;
}

.stage-row:last-child {
  padding-bottom: 0;
}

.stage-row::before {
  content: '';
  position: absolute;
  left: -32px;
  top: 24px;
  bottom: 0;
  width: 2px;
  background: var(--color-border);
}

.stage-row:last-child::before {
  display: none;
}

.stage-row:has(.stage-dot.active)::before {
  background: linear-gradient(to bottom, var(--color-border) 0%, var(--color-primary) 100%);
}

.stage-marker {
  position: absolute;
  left: -64px;
  top: 0;
  display: flex;
  flex-direction: column;
  align-items: center;
  width: 64px;
}

.stage-year {
  font-size: 12px;
  font-weight: 600;
  color: var(--color-text-secondary);
  letter-spacing: -0.02em;
  margin-bottom: 4px;
}

.stage-dot {
  width: 12px;
  height: 12px;
  border-radius: 50%;
  background: var(--color-bg-card);
  border: 2px solid var(--color-border);
  position: relative;
  z-index: 2;
}

.stage-dot.active {
  background: var(--color-primary);
  border-color: var(--color-primary);
  box-shadow: 0 0 0 3px color-mix(in srgb, var(--color-primary) 30%, transparent);
}

.stage-card {
  flex: 1;
  background: var(--color-bg-card);
  border: 1px solid var(--color-border);
  border-radius: var(--radius-md);
  padding: 12px 16px;
  transition: all var(--transition-normal);
}

.stage-card.highlight {
  border-color: var(--color-primary);
  background: linear-gradient(135deg,
    var(--color-bg-card) 0%,
    color-mix(in srgb, var(--color-primary) 5%, var(--color-bg-card)) 100%);
}

.stage-header {
  display: flex;
  align-items: center;
  gap: 10px;
  margin-bottom: 8px;
}

.stage-title {
  font-size: 16px;
  font-weight: 600;
  color: var(--color-text-primary);
}

.stage-tag {
  font-size: 10px;
  font-weight: 500;
  padding: 2px 8px;
  border-radius: var(--radius-full);
  background: var(--color-bg-hover);
  color: var(--color-text-secondary);
  text-transform: uppercase;
  letter-spacing: 0.05em;
}

.stage-tag.current {
  background: var(--color-primary);
  color: white;
}

.stage-points {
  display: flex;
  flex-wrap: wrap;
  gap: 4px 12px;
}

.stage-points span {
  font-size: 13px;
  color: var(--color-text-secondary);
  line-height: 1.4;
}

.stage-points span::before {
  content: '·';
  margin-right: 4px;
  color: var(--color-text-disabled);
}

html.dark .stage-card.highlight {
  background: linear-gradient(135deg,
    var(--color-bg-card) 0%,
    color-mix(in srgb, var(--color-primary) 12%, var(--color-bg-card)) 100%);
}
</style>
