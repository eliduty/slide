# 工作区目录规范

工作区目录统一放在项目根目录的 `workspace/` 下，存放所有工作素材，与 `presentations/` 目录中的最终产出分离。

## 目录结构

```
workspace/
├── ai-coding/                    # AI Coding 演示的工作内容
│   ├── content.md                # 内容草稿
│   ├── design.md                 # 设计思路
│   ├── examples.md               # 示例收集
│   ├── notes.md                  # 笔记整理
│   ├── references.md             # 参考资料
│   ├── research.md               # 调研笔记
│   ├── outline/                  # 大纲目录
│   ├── scripts/                  # 演讲脚本（逐字稿）
│   ├── drafts/                   # 原始草稿文件
│   └── images/                   # 图片素材
│
└── <other-topic>/                # 其他演示的工作内容
    └── ...（结构同上）
```

## 各目录用途

### content.md

内容草稿，整合所有素材后的完整内容草稿。

**用途**：
- 整合 research、notes、examples 等素材
- 作为 AI 生成 slides 的主要输入源
- 包含完整的演示内容结构

### design.md

设计思路，记录演示的设计决策和视觉风格。

**用途**：
- 记录配色方案、字体选择等设计决策
- 说明各章节的视觉风格
- 作为主题定制的参考

### examples.md

示例收集，记录可用于演示的代码示例、案例等。

**用途**：
- 收集代码示例
- 收集实际案例
- 收集图表和数据示例

### notes.md

笔记整理，记录学习过程中的要点和思考。

**用途**：
- 整理学习笔记
- 记录要点和思考
- 作为 content.md 的素材来源

### research.md

调研笔记，记录知识搜集、来源链接、要点整理。

**格式示例**：

```markdown
# 调研笔记

## 来源

- [文章链接1](url) - 关键要点
- [文章链接2](url) - 关键要点

## 核心概念

- 概念1：说明
- 概念2：说明

## 待深入

- 问题1
- 问题2
```

### outline/

大纲目录，存放演示结构规划文件。

**用途**：
- 规划演示的整体结构
- 定义各章节的内容要点
- 作为 slides 生成的结构指导

**常见文件**：
- `main.md` - 主大纲，定义整体结构
- `chapter1.md` - 章节1大纲
- `chapter2.md` - 章节2大纲

### scripts/

演讲脚本（逐字稿），与 slides 文件对应。

**用途**：
- 记录演讲的详细脚本
- 包含时长估计和重点提示
- 作为演讲练习的参考

**命名规则**：与 slides 文件名对应。

- `slides/cover/01-title.md` → `scripts/cover-title.md`
- `slides/evolution/01-history.md` → `scripts/evolution-history.md`

**格式示例**：

```markdown
# 封面页脚本

时长：约 1 分钟

## 开场白

大家好，今天我要分享的是...

## 重点提示

- 强调标题关键词
- 简短自我介绍
```

### drafts/

原始草稿文件，存放未处理的原始素材。

**常见内容**：

- `.excalidraw` - Excalidraw 图表源文件
- `.drawio` - Draw.io 图表源文件
- `.png/.jpg` - 手绘草稿、未处理图片
- `.md` - 原始笔记和草稿

### images/

图片素材，存放演示所需的图片资源。

**用途**：
- 存放演示中使用的图片
- 按章节或类型组织图片
- 作为 slides 中图片引用的来源