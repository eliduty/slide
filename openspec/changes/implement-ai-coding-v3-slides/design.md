## Context

ai-coding-v3 演示文稿基于 outline-v3.md 大纲实现，包含 39 页幻灯片。当前 v3 版本只有空的 slides.md 入口文件，需要创建完整内容。v2 版本已有成熟的结构和样式可供参考，Part 5-8 内容可直接复用 v2 版本对应章节。

**复用映射关系：**
- Part 5（对现有工作的影响）→ v2 第3章（17-21）
- Part 6（常见场景实操）→ v2 第5章（22-24）
- Part 7（标准化资产清单）→ v2 附录（25-26）
- Part 8（总结）→ v2 附录（27-29）

## Goals / Non-Goals

**Goals:**
- 创建 Part 0-4 新幻灯片内容（约 23 页）
- 复用 v2 版本 Part 5-8 内容（约 15 页）
- 更新 slides.md 入口文件元数据和 src 引用
- 保持与 v2 版本一致的样式风格

**Non-Goals:**
- Speaker notes（演讲脚本）后期补充
- 内容细节优化（本次只做结构化转换）

## Decisions

**1. 文件命名策略**

采用两位数字编号 + 主题描述的格式：
- `01-cover.md` → 封面
- `02-pain-points.md` → 痛点引入
- `03-industry-trend.md` → 行业趋势
- ...

章节页使用 `XX-chapterY-section.md` 格式保持一致性。

**2. 布局选择**

参考 v2 版本布局使用：
- `cover` → 封面页
- `Section` → 章节页
- `Default` → 内容页（带标题）
- `TwoCols` → 双栏内容页

**3. 复用策略**

Part 5-8 直接复制 v2 对应文件，调整编号后无需内容修改。编号从 24 开始（承接 Part 4 结尾的 23）。

**4. 目录结构**

```
presentations/ai-coding-v3/
├── slides.md          # 入口文件
└── slides/            # 内容目录
    ├── 01-cover.md
    ├── 02-pain-points.md
    ├── ...
    └── 39-qa.md
```

## Risks / Trade-offs

**[编号冲突] → 复用文件重新编号**

从 v2 复制的文件需要重新编号以衔接 Part 4，避免编号跳跃。

**[内容不完全匹配] → 微调标题**

Part 5-8 的内容可能与 outline-v3.md 描述有细微差异，允许标题微调但保持核心内容不变。