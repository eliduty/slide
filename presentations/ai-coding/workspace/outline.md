# AI Coding 实践分享 - 大纲

## 分享定位
- **受众**：团队内部
- **时长**：约 20-30 分钟
- **目标**：分享 AI Coding 工作流变革的实践经验

---

## 结构概览

### Part 1: 开场（2 页）

1. **封面**
   - 标题：AI Coding 实践分享
   - 副标题：从对话到 Agent，重新定义开发流程

2. **为什么关注 AI Coding**
   - AI Coding 已从"辅助工具"进化为"开发伙伴"
   - Skill 的出现是关键转折点

---

### Part 2: AI Coding 演进史（3 页）

3. **发展历程**
   ```
   Web对话 → 浏览器插件 → AI IDE → 终端Agent
   ```

4. **每个阶段的特点**
   - Web对话：上下文断裂，复制粘贴
   - 浏览器插件：集成但受限
   - AI IDE：一体化体验（Cursor）
   - 终端Agent：深度理解，自主执行（Claude Code）

5. **主流 AI Coding 工具**
   - Claude Code
   - Cursor
   - GitHub Copilot
   - Windsurf

---

### Part 3: AI Agent 能力模型（4 页）

6. **AI Agent 核心组件**
   ```
   ┌───────────────────────────────────────────────────┐
   │  Rules │ Agent │ MCP │ Skill │ Memory             │
   └───────────────────────────────────────────────────┘
   ┌───────────────────────────────────────────────────┐
   │            Chat │ Plan │ Spec                      │
   └───────────────────────────────────────────────────┘
   ```

7. **关键概念解释**
   - Rules：行为约束和项目规范
   - MCP：工具扩展协议（Model Context Protocol）
   - Skill：可复用能力封装
   - Memory：上下文记忆

8. **Claude Code Agent 体系**
   - code-explorer：代码探索
   - code-architect：架构设计
   - code-reviewer：代码审查

9. **Skill 的意义**
   - 从"对话"到"结构化工作流"
   - 可复用、可组合的能力单元
   - 重新审视开发流程的契机

---

### Part 4: Spec-Driven Development（3 页）

10. **什么是 SDD？**
    - Spec → Design → Implement
    - 先定义"是什么"，再定义"怎么做"

11. **OpenSpec + Superpowers**
    - OpenSpec：Proposal / Design / Specs / Tasks
    - Superpowers：自动化能力增强

12. **最终方案**
    ```
    Claude Code + OpenSpec + Superpowers
    = 深度代码理解 + 结构化流程 + 自动化执行
    ```

---

### Part 5: 项目实战流程（5 页）

13. **全流程概览**
    ```
    需求 → 设计 → 开发 → 测试 → 部署
    ```

14. **需求 & 设计阶段**
    - 需求：PRD → 拆分小系统 PRD
    - 设计：Pencil Plugin + MCP + Claude Code
      → 架构设计 → 技术方案设计

15. **开发阶段（核心）**
    ```
    PRD功能模块
        ↓
    explore（探索代码库）
        ↓
    propose（提案：proposal, design, spec, task）
        ↓
    apply（执行，触发 superpowers）
        ↓
    verify（验证）
        ↓
    archive（归档）
    ```

16. **开发流程演示**
    - 展示一个具体功能的开发过程
    - 截图/录屏

17. **测试、部署 & 方法论融合**
    - E2E 测试
    - CI/CD 集成
    - SDD + DDD + TDD + 金字塔测试

---

### Part 6: 总结（2 页）

18. **Key Takeaways**
    - AI Coding 已进化为 Agent 模式
    - SDD 让人机协作更高效
    - 工作流变革 > 工具选择

19. **资源 & 讨论**
    - Claude Code: https://docs.anthropic.com/en/docs/claude-code
    - Cursor: https://docs.cursor.com
    - GitHub Copilot: https://docs.github.com/copilot
    - Q&A

---

## 素材状态

- [x] 幻灯片结构完成（slides.md）
- [ ] 开发流程截图/录屏（可补充）
- [ ] Pencil Plugin + MCP 示例（可补充）
- [ ] Superpowers 触发效果（可补充）
- [ ] 实际案例 Before/After 对比（可补充）

> 注：核心内容已完成，以上素材可根据实际需要后续补充。