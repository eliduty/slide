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
├── presentations/              # 各演示文稿
│   └── _template/              # 新演示模板
│       ├── slides.md           # 入口文件 + 元数据
│       ├── slides/             # 拆分的内容文件
│       └── workspace/          # 素材工作区
├── packages/
│   └── slidev-theme-skill-ui/  # 共享主题包
│       ├── layouts/            # 布局组件
│       ├── components/         # 通用组件
│       └── styles/             # 样式文件
├── docs/                       # 项目规范文档
│   ├── project-structure.md    # 目录结构设计
│   ├── metadata-spec.md        # 元数据规范
│   ├── workspace-spec.md       # 工作区规范
│   └── ui-spec/                # UI 设计规范
└── assets-shared/              # 全局共享素材（按需创建）
```

## 创建新演示

1. 复制 `presentations/_template/` 为新目录
2. 更新 `slides.md` 的 frontmatter 元数据（id、title、tags、status 等）
3. 在 package.json 添加对应的 npm scripts
4. 在 README.md 演示列表表格中添加新条目

## slides.md 元数据规范

每个演示的 slides.md 入口文件包含演示级元数据：

```yaml
---
# Slidev 配置
theme: ../../packages/slidev-theme-skill-ui
title: 演示标题
author: eliduty
aspectRatio: 16/9

# 自定义元数据
id: unique-id            # 与目录名一致
created: 2026-03-28
updated: 2026-03-28
tags: [tag1, tag2]
slidesCount: 12
estimatedTime: 15min
status: draft            # draft/reviewing/ready/published
---
```

## 主题使用

主题路径为相对路径：`../../packages/slidev-theme-skill-ui`

可用布局：
- `Cover` - 封面页
- `Default` - 默认布局
- `Section` - 章节分隔页
- `TwoCols` - 双栏布局
- `TopTitle` - 顶部标题布局
- `Quote` - 引用布局
- `Credits` - 结尾页

可用组件：
- `Admonition` - 提示框
- `Badge` - 标签徽章
- `CodeBlock` - 代码块
- `QRCode` - 二维码

## workspace 目录用途

每个演示的 workspace/ 存放工作素材，与最终产出分离：
- `research.md` - 调研笔记
- `outline.md` - 大纲草稿
- `references.md` - 参考资料
- `scripts/` - 演讲脚本（逐字稿）
- `data/` - 数据源文件
- `drafts/` - 原始草稿
- `feedback.md` - 反馈记录