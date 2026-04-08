# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## 项目概述

这是一个基于 Slidev 的幻灯片演示文稿库，用于管理多个独立的演示项目。

## 常用命令

```bash
# 安装依赖
pnpm install

# 运行开发服务器（以 ai-coding 为例）
pnpm dev:ai-coding

# 构建演示
pnpm build:ai-coding

# 导出 PDF/SPA
pnpm export:ai-coding
```

添加新演示时，需要在 package.json 中添加对应的 npm scripts：
- `dev:<name>`: 开发模式
- `build:<name>`: 构建输出
- `export:<name>`: 导出文件

## 目录架构

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
│   │   ├── slides.md            # 入口文件 + 元数据
│   │   └── slides/              # 拆分的内容文件
│   ├── ai-coding-v1/            # AI Coding 版本1
│   ├── ai-coding-v2/            # AI Coding 版本2
│   └── ai-coding-v3/            # AI Coding 版本3
├── packages/
│   └── slidev-theme-skill-ui/   # 共享主题包
│       ├── layouts/             # 布局组件
│       ├── components/          # 通用组件
│       └── styles/              # 样式文件
├── docs/                        # 项目规范文档
│   ├── project-structure.md     # 目录结构设计
│   ├── metadata-spec.md         # 元数据规范
│   ├── workspace-spec.md        # 工作区规范
│   └── ui-spec/                 # UI 设计规范
└── assets-shared/               # 全局共享素材（按需创建）
```

## 创建新演示

1. 在 `workspace/` 创建新的工作目录（如 `workspace/<topic>/`）
2. 在 `presentations/` 创建新的版本目录（如 `presentations/<topic-v1>/`）
3. 复制 `presentations/_template/` 的结构到新版本目录
4. 更新 `slides.md` 的 frontmatter 元数据（id、title、tags、status 等）
5. 在 package.json 添加对应的 npm scripts
6. 在 README.md 演示列表表格中添加新条目

## 工作与产出分离

- **workspace/ 目录**：存放所有工作素材（调研、笔记、大纲、脚本等）
- **presentations/ 目录**：只存放 AI 生成的最终 slides 产出
- **多版本管理**：同一个工作内容可以生成多个版本的 slides（v1, v2, v3 等）

## workspace 目录用途

工作区存放演示的工作素材：
- `content.md` - 内容草稿
- `design.md` - 设计思路
- `examples.md` - 示例收集
- `notes.md` - 笔记整理
- `references.md` - 参考资料
- `research.md` - 调研笔记
- `outline/` - 大纲目录
- `scripts/` - 演讲脚本（逐字稿）
- `drafts/` - 原始草稿文件
- `images/` - 图片素材