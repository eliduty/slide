OpenSpec 完全指南：让 AI 编码可预测的规范框架
tinyash
0 条评论
openspec
文章信息

发布时间
2026年3月22日
作者
tinyash
阅读时长
3 分钟阅读
分享文章


摘要：OpenSpec 是由 Fission AI 开发的轻量级规范框架，帮助团队在使用 AI 编码助手时保持可预测性和组织性。通过为每个变更创建独立的规范文件夹（提案、规格、设计、任务），OpenSpec 让你在与 AI 写代码之前先达成一致。本文详细介绍 OpenSpec 的核心理念、OPSX 工作流、命令参考和最佳实践。

一、OpenSpec 是什么？
1.1 核心理念
OpenSpec 是一个轻量级的规范框架，专为 AI 编码时代设计：

在写代码之前，先就”要构建什么”达成一致。

核心哲学：

→ fluid not rigid          (灵活而非僵化)
→ iterative not waterfall  (迭代而非瀑布)
→ easy not complex         (简单而非复杂)
→ built for brownfield     (为现有项目设计)
→ scalable                 (从个人项目到企业级)
1.2 解决的问题
AI 编码的痛点：

问题	传统方式	OpenSpec 方案
需求只在聊天记录	需求淹没在聊天历史中	独立的规范文件夹，可追溯
结果不可预测	模糊的提示导致不确定的输出	明确的规范带来可预测的结果
缺乏组织	多个功能混在一起	每个变更独立的文件夹结构
难以协作	个人与 AI 对话，团队不知情	规范文档可共享和审查
1.3 与其他工具对比
工具	特点	OpenSpec 优势
Spec Kit (GitHub)	彻底但重量级，刚性阶段门	OpenSpec 更轻量，支持灵活迭代
Kiro (AWS)	强大但锁定在特定 IDE	OpenSpec 支持 20+ 工具，自由选择
无规范	快速但不可预测	OpenSpec 带来可预测性，无繁文缛节
二、快速开始
2.1 安装
系统要求：Node.js 20.19.0 或更高

# 全局安装
npm install -g @fission-ai/openspec@latest
# 或使用其他包管理器
pnpm add -g @fission-ai/openspec
yarn global add @fission-ai/openspec
bun install -g @fission-ai/openspec
2.2 初始化项目
# 进入项目目录
cd your-project
# 初始化 OpenSpec
openspec init
初始化会创建：

openspec/ – OpenSpec 配置和规范目录
openspec/changes/ – 变更规范文件夹
AI 技能文件（自动检测）
2.3 配置工作流
OpenSpec 提供两种工作流模式：

默认模式（Core Profile）：

# 快速路径，包含 4 个命令
/opsx:propose   # 创建变更和规划文档
/opsx:explore   # 探索想法
/opsx:apply     # 实现任务
/opsx:archive   # 归档完成的变更
扩展模式（Expanded Profile）：

# 配置扩展工作流
openspec config profile  # 选择 workflows
openspec update          # 应用配置
# 扩展命令
/opsx:new         # 创建变更脚手架
/opsx:continue    # 逐个创建文档
/opsx:ff          # 快速创建所有规划文档
/opsx:verify      # 验证实现
/opsx:sync        # 同步增量规范
/opsx:bulk-archive # 批量归档
/opsx:onboard     # 引导教程
三、OPSX 工作流详解
3.1 工作流理念
传统线性工作流的问题：

规划阶段 → 实现阶段 → 完成
（但实际工作不是这样的！）
OPSX 的方法：

行动，而非阶段 — 创建、实现、更新、归档 — 随时执行任何操作
依赖是赋能者 — 显示什么是可能的，而非必须下一步做什么
文档依赖关系：

proposal → specs → design → tasks → implement
3.2 核心工作流（Core Profile）
步骤 1：探索想法（可选）
你：/opsx:explore 如何为移动应用处理认证
AI：让我调查一下你当前的认证设置...
    [分析代码库]
    我看到你的 Web 应用使用基于会话的认证。
    对于移动端，有三个主要选项：
    1. JWT 令牌（无状态，支持离线）
    2. OAuth2（如果需要第三方登录）
    3. 扩展现有会话（更简单，但需要连接）
    你的 API 已配置 CORS。哪个方向你感兴趣？
你：我们用 JWT 吧。能开始一个变更吗？
AI：准备好了。运行 /opsx:propose add-jwt-auth 开始。
步骤 2：创建变更
你：/opsx:propose add-dark-mode
AI：已创建 openspec/changes/add-dark-mode/
    ✓ proposal.md — 为什么要做，改什么
    ✓ specs/      — 需求和场景
    ✓ design.md   — 技术方案
    ✓ tasks.md    — 实现清单
    准备好实现了！运行 /opsx:apply
步骤 3：实现任务
你：/opsx:apply
AI：正在实现任务...
    ✓ 1.1 添加主题上下文提供者
    ✓ 1.2 创建切换组件
    ✓ 2.1 添加 CSS 变量
    ✓ 2.2 连接 localStorage
    所有任务完成！
步骤 4：归档
你：/opsx:archive
AI：已归档到 openspec/changes/archive/2026-03-22-add-dark-mode/
    规范已更新。准备好下一个功能。
3.3 扩展工作流（Expanded Profile）
创建变更脚手架
你：/opsx:new add-user-profile
AI：已创建 openspec/changes/add-user-profile/
    ✓ .openspec.yaml (元数据)

    下一步：创建 proposal.md
    运行 /opsx:continue
逐个创建文档
你：/opsx:continue
AI：准备创建 proposal.md
    依赖：无
    模板：openspec/templates/proposal.md

    正在生成...
    ✓ proposal.md 创建完成
    下一步：创建 specs
    运行 /opsx:continue
快速创建所有规划文档
你：/opsx:ff
AI：快速创建所有规划文档...
    ✓ proposal.md
    ✓ specs/
    ✓ design.md
    ✓ tasks.md

    准备好实现。运行 /opsx:apply
验证实现
你：/opsx:verify
AI：验证实现是否符合文档...
    ✓ 检查 tasks.md 中的任务
    ✓ 验证代码实现
    ✓ 检查测试覆盖

    验证通过！所有任务正确实现。
四、项目配置
4.1 创建配置
配置在 openspec init 时自动创建，或手动创建：

# openspec/config.yaml
schema: spec-driven  # 默认规范
# 项目上下文，注入到所有文档
context: |
  技术栈：TypeScript, React, Node.js
  API 约定：RESTful, JSON 响应
  测试：Vitest 单元测试，Playwright e2e
  代码风格：ESLint + Prettier, 严格 TypeScript
# 每个文档的规则
rules:
  proposal:
    - 包含回滚计划
    - 识别受影响的团队
  specs:
    - 使用 Given/When/Then 格式编写场景
  design:
    - 复杂流程包含时序图
4.2 配置字段
字段	类型	说明
schema	string	新变更的默认规范（如 spec-driven）
context	string	注入到所有文档的项目上下文
rules	object	每个文档的规则，按文档 ID 键控
4.3 规范优先级
配置优先级（从高到低）：

CLI 标志 (--schema <name>)
变更元数据 (变更目录中的 .openspec.yaml)
项目配置 (openspec/config.yaml)
默认值 (spec-driven)
4.4 可用的规范模式
spec-driven（默认）：

proposal – 变更提案
specs – 规格说明
design – 技术设计
tasks – 实现任务
五、文档模板
5.1 变更提案（proposal.md）
# 变更提案：{变更名称}
## 为什么要做这个
[问题陈述和动机]
## 目标
[具体、可衡量的目标]
## 范围
### 包含
- [ ] 功能 1
- [ ] 功能 2
### 不包含
- [ ] 明确排除的内容
## 风险
[潜在风险和缓解策略]
## 回滚计划
[如果需要回滚，如何操作]
## 相关方
[受此变更影响的团队或个人]
5.2 规格说明（specs/spec.md）
# 规格：{功能名称}
## 用户场景
### 场景 1：成功路径
- **Given** [前置条件]
- **When** [用户操作]
- **Then** [预期结果]
### 场景 2：异常处理
- **Given** [前置条件]
- **When** [异常操作]
- **Then** [错误处理]
## 功能需求
| ID | 需求 | 优先级 | 验收标准 |
|----|------|--------|---------|
| FR-001 | 描述 | P0 | 可验证的标准 |
## 非功能需求
### 性能
[性能指标]
### 安全
[安全要求]
### 可访问性
[无障碍要求]
5.3 技术设计（design.md）
# 技术设计：{功能名称}
## 架构概述
[系统架构图和描述]
## 组件设计
### 组件 1：名称
**职责**：[组件职责]
**接口**：
```typescript
interface Component1 {
  method1(): Promise<void>;
}
依赖：

依赖 1
依赖 2
数据设计
数据模型
[ER 图或数据模型]

数据库变更
ALTER TABLE users ADD COLUMN theme VARCHAR(20);
API 设计
端点 1：POST /api/feature
请求：

{
  "field": "value"
}
响应：

{
  "id": "123",
  "status": "success"
}
安全考虑
[认证、授权、数据加密等]

### 5.4 实现任务（tasks.md）
```markdown
# 实现任务：{功能名称}
## 任务列表
### 任务 1：组件开发
- [ ] 1.1 创建主题上下文提供者
  - 文件：`src/context/ThemeContext.tsx`
  - 测试：`src/context/ThemeContext.test.tsx`

- [ ] 1.2 创建切换组件
  - 文件：`src/components/ThemeToggle.tsx`
  - 测试：`src/components/ThemeToggle.test.tsx`
### 任务 2：样式实现
- [ ] 2.1 添加 CSS 变量
  - 文件：`src/styles/variables.css`

- [ ] 2.2 连接 localStorage
  - 文件：`src/hooks/useTheme.ts`
## 完成标准
- [ ] 所有任务完成
- [ ] 测试通过
- [ ] 代码审查通过
六、命令参考
6.1 核心命令（Core Profile）
命令	说明	何时使用
/opsx:propose	创建变更并生成规划文档	开始新功能
/opsx:explore	探索想法，调查问题	需求不明确时
/opsx:apply	实现任务	文档完成后
/opsx:archive	归档完成的变更	功能完成后
6.2 扩展命令（Expanded Profile）
命令	说明	何时使用
/opsx:new	创建变更脚手架	想逐步创建文档
/opsx:continue	创建下一个文档	逐个创建文档
/opsx:ff	快速创建所有规划文档	想跳过逐步创建
/opsx:verify	验证实现符合文档	实现完成后检查
/opsx:sync	同步增量规范到主规范	合并增量变更
/opsx:bulk-archive	批量归档多个变更	清理多个完成项
/opsx:onboard	端到端工作流教程	新手学习
6.3 命令详解
/opsx:propose [change-name]
参数：

change-name（可选）- 变更名称或描述
示例：

/opsx:propose add-dark-mode
/opsx:propose 添加用户个人资料功能
/opsx:explore [topic]
参数：

topic（可选）- 要探索的主题
示例：

/opsx:explore
/opsx:explore 移动端认证方案
/opsx:explore 如何优化数据库查询性能
/opsx:apply
无需参数，自动读取当前变更的任务列表并实现。

/opsx:archive
无需参数，归档当前变更并更新主规范。

七、最佳实践
7.1 文档编写
推荐做法：

✅ 使用项目配置注入上下文
✅ AI 生成初稿，人工审查完善
✅ 保持文档简洁，聚焦关键决策
✅ 使用 Given/When/Then 格式编写场景
✅ 定期归档完成的变更
避免做法：

❌ 过度详细，难以维护
❌ 完全依赖 AI，不人工审查
❌ 文档与代码脱节
❌ 使用模糊词汇
7.2 工作流选择
Core Profile 适合：

小型功能
快速迭代
个人项目
熟悉 OpenSpec 的团队
Expanded Profile 适合：

大型功能
需要逐步审查
团队协作
新手学习
7.3 模型选择
OpenSpec 最适合高推理能力的模型：

推荐模型：

Claude Opus 4.5
GPT-5.2
其他高推理模型
不推荐：

小型模型（可能无法理解复杂规范）
7.4 上下文管理
保持上下文清洁：

开始实现前清除上下文
定期总结长对话
使用文档而非聊天记录作为参考
八、团队协作
8.1 团队工作流
产品经理 → 创建变更提案 → 技术审查
    ↓
技术负责人 → 审查设计 → 批准
    ↓
开发者 → 实现任务 → 验证
    ↓
测试 → 验证功能 → 归档
8.2 审查流程
提案审查清单：

[ ] 问题陈述清晰
[ ] 目标可衡量
[ ] 范围明确
[ ] 风险已识别
[ ] 回滚计划可行
设计审查清单：

[ ] 架构合理
[ ] 接口定义清晰
[ ] 数据设计正确
[ ] 安全考虑充分
[ ] 性能可接受
8.3 团队配置
# openspec/config.yaml
context: |
  团队：后端组
  代码审查：至少 2 人批准
  部署：自动 CI/CD
  监控：Datadog 告警
rules:
  proposal:
    - 包含产品负责人批准
    - 识别依赖团队
  design:
    - 架构审查会议记录
    - 性能基准测试计划
九、与 AI 工具集成
9.1 支持的工具
OpenSpec 支持 20+ AI 编码助手：

工具	集成方式
Claude Code	技能自动检测
Cursor	技能自动检测
Windsurf	技能自动检测
Codex	技能自动检测
OpenCode	技能自动检测
OpenClaw	技能自动检测
其他	通过技能文件
9.2 技能文件
OpenSpec 自动在以下位置创建技能：

.claude/skills/ – Claude Code
.cursor/skills/ – Cursor
.windsurf/skills/ – Windsurf
其他工具的等效位置
技能示例：

---
name: openspec-propose
description: Create a new OpenSpec change proposal
---
# OpenSpec Propose Skill
When user wants to create a new feature:
1. Run: openspec propose <change-name>
2. Review generated artifacts
3. Iterate on proposal if needed
4. Get stakeholder approval
9.3 提示词技巧
好的提示词：

/opsx:propose 添加深色模式支持
上下文：
- 用户要求深色模式已 3 个月
- 竞品都有此功能
- 技术栈支持 CSS 变量
目标：
- 用户可在设置中切换主题
- 自动检测系统偏好
- 记住用户选择
不好的提示词：

/opsx:propose 深色模式
（太模糊，缺少上下文和目标）
十、更新和维护
10.1 更新 OpenSpec
# 更新全局包
npm install -g @fission-ai/openspec@latest
# 更新项目技能
openspec update
10.2 版本兼容
OpenSpec 版本	最小 Node.js	备注
1.x	20.19.0	初始版本
2.x	20.19.0	OPSX 工作流
10.3 遥测
OpenSpec 收集匿名使用统计：

命令名称
版本号
不收集：

参数和路径
文档内容
个人信息
退出遥测：

export OPENSPEC_TELEMETRY=0
export DO_NOT_TRACK=1
十一、故障排查
11.1 常见问题
Q：技能未被 AI 检测？

A：

# 重新生成技能
openspec update
# 检查技能目录
ls -la .claude/skills/openspec*
Q：命令不工作？

A：

# 检查版本
openspec --version
# 重新安装
npm install -g @fission-ai/openspec@latest
Q：配置不生效？

A：

确保文件在 openspec/config.yaml（不是 .yml）
检查 YAML 语法
配置更改立即生效，无需重启
11.2 性能优化
大项目优化：

# 使用增量模式
openspec sync --incremental
# 批量归档
openspec bulk-archive --before 2026-01-01
十二、总结
OpenSpec 核心价值：

✅ 可预测性 — 明确的规范带来可预测的 AI 输出
✅ 组织性 — 每个变更独立的文件夹结构
✅ 灵活性 — 随时更新任何文档，无刚性阶段
✅ 工具自由 — 支持 20+ AI 编码助手
✅ 轻量级 — 最小开销，最大价值

适用场景：

🚀 新功能开发
🔧 重构和改进
🐛 复杂 Bug 修复
📋 团队协作文档
不适用场景：

❌ 简单修复（直接写代码更快）
❌ 快速原型（文档可能成为负担）
❌ 探索性工作（先用 /opsx:explore）
下一步行动：

安装 OpenSpec：npm install -g @fission-ai/openspec
初始化项目：openspec init
尝试第一个变更：/opsx:propose your-feature
加入社区：Discord
