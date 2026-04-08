# Slide 项目结构设计

## 目录结构

```
slide/
│
├── workspace/                         # 工作区（存放所有工作素材）
│   ├── ai-coding/                     # AI Coding 演示的工作内容
│   │   ├── content.md                 # 内容草稿
│   │   ├── design.md                  # 设计思路
│   │   ├── examples.md                # 示例收集
│   │   ├── notes.md                   # 笔记整理
│   │   ├── references.md              # 参考资料
│   │   ├── research.md                # 调研笔记
│   │   ├── outline/                   # 大纲目录
│   │   ├── scripts/                   # 演讲脚本（逐字稿）
│   │   ├── drafts/                    # 原始草稿文件
│   │   └── images/                    # 图片素材
│   │
│   └── <other-topic>/                 # 其他演示的工作内容
│       └── ...（结构同上）
│
├── presentations/                     # 演示文稿（AI生成的最终产出）
│   ├── _template/                     # 新演示模板
│   │   ├── slides.md                  # 入口文件
│   │   └── slides/                    # 拆分的内容文件
│   │
│   ├── ai-coding-v1/                  # AI Coding 版本1
│   │   ├── slides.md
│   │   └── slides/
│   │
│   ├── ai-coding-v2/                  # AI Coding 版本2
│   │   ├── slides.md
│   │   └── slides/
│   │
│   └── <other-topic-v1>/              # 其他演示
│       └── ...
│
├── assets-shared/                     # 全局共享素材
│   ├── icons/
│   ├── brand/
│   ├── templates/
│   └── fonts/
│
├── packages/                          # 共享主题包
│   └── slidev-theme-skill-ui/
│       ├── layouts/
│       ├── components/
│       └── styles/
│
├── docs/                              # 项目文档
│   ├── project-structure.md
│   ├── metadata-spec.md
│   ├── workspace-spec.md
│   └── ui-spec/
│
├── README.md                          # 项目索引
└
└── package.json                       # 项目依赖
```

## 设计原则

1. **工作与产出分离** - workspace 存放工作素材，presentations 只存放 AI 生成的最终产出
2. **多版本管理** - 同一个工作内容可以生成多个版本的 slides（v1, v2, v3 等）
3. **符合 Slidev 设计哲学** - 每个演示独立，遵循单项目单入口原则
4. **AI 友好** - 扁平结构 + 元数据融入 Markdown，易于导航和理解
5. **共享通过 Theme** - Slidev 原生支持，组件自动注册

## 关键变化

**旧结构**：工作素材在 presentations 内的 workspace 目录
**新结构**：工作素材统一在根目录的 workspace，presentations 只存放最终产出

**优势**：
- 工作内容集中管理，便于维护
- 支持多版本迭代，同一工作内容可生成不同版本的 slides
- presentations 目录更简洁，职责更清晰