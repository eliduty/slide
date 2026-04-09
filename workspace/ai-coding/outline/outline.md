# AI Coding 实践分享 - 大纲

## 分享定位
- **受众**：团队内部
- **时长**：约 70-75 分钟
- **目标**：分享 AI Coding 工作流变革的实践经验
- **重点内容**：TRAE、OpenSpec、SuperPowers、实战项目流程

---

## 结构概览

### Part 1: 开场（3-5 分钟）

1. **封面**
   - 标题：AI Coding 实践分享
   - 副标题：从对话到 Agent，重新定义开发流程

2. **AI 编程的现状与痛点**
   - 你是否遇到过：
     - AI 生成的代码不符合项目规范？
     - AI 不理解你的项目架构？
     - AI 写的代码难以维护？
   - 这些问题的根源是什么？

3. **AI Coding 的现状与价值**
   - AI Coding 已从"辅助工具"进化为"开发伙伴"
   - Skill 的出现是关键转折点
   - 本次分享的目标和结构

4. **方法论演进：从 Prompt 到 Harness**
   - Prompt Engineering：提示词工程，上下文不足仍会失败
   - Context Engineering：上下文工程，管理依赖人工难以复用
   - Harness Engineering：编排工程，模板+规则+工作流可复用体系

5. **Harness 核心体系**
   - 核心理念：让 AI 在规范约束下执行任务，输出可预测、可追溯、可验证的结果
   - 三大要素：
     - 模板（PRD、design、tasks 等标准化文档）
     - 规则（CLAUDE.md + rules 约束文件）
     - 工作流（propose → explore → apply → archive）

---

### Part 2: AI Coding 演进史（4 页，5-8 分钟）

6. **发展历程**
   - 时间轴：2022-2025
   - Web对话 → 编辑器插件 → AI IDE → 终端Agent

7. **每个阶段的特点**
   - Web对话：上下文断裂，复制粘贴
   - 编辑器插件：集成但受限
   - AI IDE：一体化体验（Cursor）
   - 终端Agent：深度理解，自主执行（Claude Code）

8. **主流 AI Coding 工具**
   - GUI 工具：Cursor、GitHub Copilot、Windsurf、Trae、Qoder、CodeBuddy
   - 命令行工具：Claude Code、OpenCode、Codex CLI

9. **行业趋势**
   - AI 编程工具采用率
   - 开发效率提升数据

---

### Part 3: AI Agent 能力模型（5 页，12-15 分钟）

10. **AI Agent 核心组件**
    - 架构图：Agent、MCP、Skill、Memory、Rules、Commands
    - 一句话解释每个组件的作用

11. **以 TRAE 为例讲解**
    - TRAE 的两种主要模式：IDE 模式（Chat + Builder）和 Solo 模式
    - 演示：Builder 模式或 Solo 模式（二选一）

12. **关键概念解释**
    - Agent —— 智能体主体（决策、规划、控制）
    - Skill —— 能力模块（能做什么）
    - Commands —— 指令动作（具体调用什么）
    - Memory —— 记忆状态（记住上下文、历史）
    - Rules —— 规则约束（权限、安全、边界）
    - MCP —— 模型上下文协议（开放标准，允许 AI 代理安全地访问外部数据源）

13. **Skill 的意义**
    - 从"对话"到"结构化工作流"
    - 可复用、可组合的能力单元
    - 重新审视开发流程的契机

14. **Agent 模式的优势与挑战**
    - 优势：自主性、可预测性、可追溯性
    - 挑战：上下文管理、安全性、可控性

---

### Part 4: Spec-Driven Development（4 页，15-18 分钟）

15. **什么是 SDD？**
    - 一句话定义：先定义"是什么"，再定义"怎么做"
    - 对比：传统开发 vs SDD
    - 为什么需要 SDD？

16. **OpenSpec 讲解**
    - OpenSpec 是什么：Fission AI 开发的轻量级规范框架
    - 解决的问题：需求只在聊天记录、结果不可预测、缺乏组织、难以协作
    - 与传统方式对比：直接生成 vs 规范驱动
    - 市面上支持 SDD 的工具对比：Spec Kit、Kiro、OpenSpec
    - 两种工作流模式：
      - 默认模式（Core Profile）：propose → explore → apply → archive
      - 扩展模式（Expanded Profile）：new → continue → ff → verify → sync → bulk-archive
    - 重点介绍默认模式的流程
    - 文档结构：proposal.md、specs/、design.md、tasks.md
    - 演示：如何用 OpenSpec 生成规范文档

17. **Superpowers 讲解**
    - Superpowers 是什么：Superpowers是一套skill集合，为 AI 编程提供结构化工作流程
    - 核心技能：8 个技能（按完整工作流顺序）
    - 演示：brainstorm 或 TDD（二选一）
    - 对比：有 Superpowers vs 无 Superpowers

18. **完整方案**
    - Claude Code + OpenSpec + Superpowers
    - 三者如何配合工作
    - 架构图展示

---

### Part 5: 项目实战流程（6 页，20-25 分钟）⭐

19. **项目背景与数据概览**
    - 项目介绍
    - 关键数据：开发周期、代码量、工具调用次数
    - 数据可视化图表

20. **开发时间线**
    - 阶段一：设计阶段
    - 阶段二：项目搭建
    - 阶段三：功能开发
    - 阶段四：细节打磨与部署

21. **核心工作流**
    - 需求 → 设计 → 开发 → 测试 → 部署
    - 开发阶段详解：
    ```
    PRD功能模块
        ↓
    propose（提案：proposal, design, spec, task）
        ↓
    explore（探索代码库）
        ↓
    apply（执行，触发 superpowers）
        ↓
    archive（归档）
    ```

22. **典型案例演示**
    - 案例一：AI 驱动产品设计
    - 案例二：SDD 驱动前端功能研发
    - 配合截图/录屏

23. **方法论融合**
    - SDD + DDD + TDD 如何结合
    - 金字塔测试在 AI 编程中的应用
    - CI/CD 集成

24. **经验总结与建议**
    - 哪些做得好
    - 哪些踩了坑
    - 给团队的建议

---

### Part 6: 总结（3-5 分钟）

25. **Key Takeaways**
    - AI Coding 已进化为 Agent 模式
    - SDD 让人机协作更高效
    - 工作流变革 > 工具选择

26. **下一步行动建议**
    - 如何开始尝试
    - 推荐的学习路径
    - 团队如何落地

27. **Q&A**
    - 预留 5 分钟问答时间

---

## 素材状态

- [x] 幻灯片结构完成
- [ ] 开发流程截图/录屏（可补充）
- [ ] OpenSpec 演示素材（可补充）
- [ ] Superpowers 演示素材（可补充）
- [ ] 数据可视化图表（可补充）
- [ ] 实际案例 Before/After 对比（可补充）

> 注：核心内容已完成，以上素材可根据实际需要后续补充。
