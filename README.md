# Slide 演示文稿库

个人幻灯片项目，使用 [Slidev](https://sli.dev) 构建。

## 演示列表

| ID | 标题 | 状态 | 页数 | 标签 | 更新日期 |
|----|------|------|------|------|----------|

<!-- 添加新演示后，在此表格中添加条目 -->

## 目录结构

```
slide/
├── workspace/                   # 工作区（存放所有工作素材）
│   └── ai-coding/               # AI Coding 演示的工作内容
│       ├── content.md           # 内容草稿
│       ├── design.md            # 设计思路
│       ├── examples.md          # 示例收集
│       ├── notes.md             # 笔记整理
│       ├── references.md        # 参考资料
│       ├── research.md          # 调研笔记
│       ├── outline/             # 大纲目录
│       ├── scripts/             # 演讲脚本（逐字稿）
│       ├── drafts/              # 原始草稿文件
│       └── images/              # 图片素材
├── presentations/               # 演示文稿（AI生成的最终产出）
│   ├── _template/               # 新演示模板
│   ├── ai-coding-v1/            # AI Coding 版本1
│   ├── ai-coding-v2/            # AI Coding 版本2
│   └── ai-coding-v3/            # AI Coding 版本3
├── packages/                    # 共享主题包
│   └── slidev-theme-skill-ui/
├── assets-shared/               # 全局共享素材
├── docs/                        # 项目文档
└── README.md
```

## 工作流程

1. **工作阶段**：在 `workspace/` 目录中准备素材和内容
2. **生成阶段**：使用 AI 从 workspace 内容生成 slides 到 `presentations/`
3. **迭代阶段**：同一工作内容可生成多个版本的 slides（v1, v2, v3 等）

## 共享组件

| 组件 | 用途 |
|------|------|
| CodeBlock | 代码块展示 |
| TwoColumn | 双栏布局 |
| Cover | 封面布局 |

## 快速开始

```bash
# 安装依赖
pnpm install

# 运行模板演示
pnpm dev:template

# 构建演示
pnpm build:template
```

## 创建新演示

1. 在 `workspace/` 创建新的工作目录（如 `workspace/<topic>/`）
2. 在工作目录中准备素材（content.md、outline、scripts 等）
3. 在 `presentations/` 创建新的版本目录（如 `presentations/<topic-v1>/`）
4. 复制 `presentations/_template/` 的结构到新版本目录
5. 使用 AI 从 workspace 内容生成 slides
6. 在 README.md 演示列表中添加新条目