---
layout: Default
---

# 2.3 规范 AI 工作环境

<div class="env-grid">

<div class="env-card card-green">
<div class="card-left">
<div class="card-num">01</div>
<div class="card-title">开发环境</div>
<div class="card-meta">SDE 负责</div>
</div>
<div class="card-right">
<div class="card-output">项目规则文件</div>
<div class="card-action">配置 CLAUDE.md + rules</div>
</div>
</div>

<div class="env-card card-blue">
<div class="card-left">
<div class="card-num">02</div>
<div class="card-title">测试环境</div>
<div class="card-meta">SDE + QA</div>
</div>
<div class="card-right">
<div class="card-output">测试用例 + Mock</div>
<div class="card-action">测试策略 + mock 数据</div>
</div>
</div>

<div class="env-card card-yellow">
<div class="card-left">
<div class="card-num">03</div>
<div class="card-title">联动调试</div>
<div class="card-meta">SDE 负责</div>
</div>
<div class="card-right">
<div class="card-output">集成验证记录</div>
<div class="card-action">前后端/模块间联调</div>
</div>
</div>

<div class="env-card card-teal">
<div class="card-left">
<div class="card-num">04</div>
<div class="card-title">领域知识</div>
<div class="card-meta">SDE + PM</div>
</div>
<div class="card-right">
<div class="card-output">领域知识文档</div>
<div class="card-action">业务术语 + 数据流图</div>
</div>
</div>

</div>

<div class="key-message">
<div class="key-icon">⚠</div>
<div class="key-text">进入实现阶段前，必须完成这四项环境准备工作</div>
</div>

<style>
.env-grid {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 16px;
  margin-top: 20px;
}

.env-card {
  display: flex;
  border-radius: 10px;
  overflow: hidden;
  box-shadow: 0 2px 4px rgba(0,0,0,0.1);
}

.card-green { background: #ecfdf5; }
.card-green .card-left { background: #10b981; }
.card-blue { background: #eff6ff; }
.card-blue .card-left { background: #3b82f6; }
.card-yellow { background: #fefce8; }
.card-yellow .card-left { background: #eab308; }
.card-teal { background: #f0fdfa; }
.card-teal .card-left { background: #14b8a6; }

.card-left {
  width: 100px;
  padding: 14px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  color: white;
}

.card-num {
  font-size: 28px;
  font-weight: 700;
  line-height: 1;
}

.card-title {
  font-size: 16px;
  font-weight: 600;
  margin-top: 6px;
}

.card-meta {
  font-size: 13px;
  opacity: 0.85;
  margin-top: 4px;
}

.card-right {
  flex: 1;
  padding: 14px 16px;
  display: flex;
  flex-direction: column;
  justify-content: center;
}

.card-output {
  font-size: 20px;
  font-weight: 600;
  color: #1f2937;
}

.card-action {
  font-size: 14px;
  color: #4b5563;
  margin-top: 6px;
}

.key-message {
  margin-top: 20px;
  display: flex;
  align-items: center;
  gap: 12px;
  padding: 14px 20px;
  background: linear-gradient(135deg, #fef3c7 0%, #fde68a 100%);
  border-radius: 10px;
  border-left: 5px solid #f59e0b;
}

.key-icon {
  font-size: 28px;
  color: #d97706;
}

.key-text {
  font-size: 17px;
  font-weight: 500;
  color: #92400e;
}

/* 暗色模式 */
.dark .card-green { background: #064e3b; }
.dark .card-blue { background: #1e3a5f; }
.dark .card-yellow { background: #422006; }
.dark .card-teal { background: #134e4a; }

.dark .card-output { color: #f3f4f6; }
.dark .card-action { color: #d1d5db; }

.dark .key-message {
  background: linear-gradient(135deg, #78350f 0%, #92400e 100%);
  border-left-color: #fbbf24;
}
.dark .key-icon { color: #fbbf24; }
.dark .key-text { color: #fef3c7; }
</style>