# Slide 项目结构设计

## 目录结构

```
slide/
│
├── presentations/                    # 各演示文稿
│   ├── tech-intro/
│   │   ├── slides.md                 # 入口 + 演示级元数据
│   │   ├── slides/                   # 内容拆分（每页可带页级元数据）
│   │   │   ├── 01-cover.md
│   │   │   ├── 02-intro.md
│   │   │   └── 03-summary.md
│   │   ├── workspace/                # 素材工作区
│   │   │   ├── research.md           # 调研笔记
│   │   │   ├── outline.md            # 大纲草稿
│   │   │   ├── references.md         # 参考资料
│   │   │   ├── scripts/              # 演讲脚本
│   │   │   │   ├── cover.md
│   │   │   │   └── intro.md
│   │   │   ├── data/                 # 数据源
│   │   │   ├── drafts/               # 原始草稿
│   │   │   └── feedback.md           # 反馈记录
│   │   ├── public/                   # 最终资源（打包进演示）
│   │   │   ├── images/
│   │   │   └── diagrams/
│   │   └── archive/                  # 版本归档
│   │       └── 2026-03-15/           # 按日期命名
│   │           └── slides.md
│   │
│   ├── design-system/                # 演示2
│   │   └── ...（结构同上）
│   │
│   └── ai-workshop/                  # 演示3
│       └── ...（结构同上）
│       │
├── assets-shared/                    # 全局共享素材
│   ├── icons/
│   ├── brand/
│   ├── templates/
│   └── fonts/
│
├── theme-shared/                     # 共享主题
│   ├── layouts/
│   ├── components/
│   └── styles/
│
├── docs/                             # 项目文档
│   └── ...
│
├── README.md                         # 项目索引
│
└── package.json                      # 项目依赖
```

## 设计原则

1. **符合 Slidev 设计哲学** - 每个演示独立，遵循单项目单入口原则
2. **AI 友好** - 扁平结构 + 元数据融入 Markdown，易于导航和理解
3. **素材跟随演示** - 工作区与产出紧密关联，独立性强
4. **共享通过 Theme** - Slidev 原生支持，组件自动注册