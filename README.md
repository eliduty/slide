# Slide 演示文稿库

个人幻灯片项目，使用 [Slidev](https://sli.dev) 构建。

## 演示列表

| ID | 标题 | 状态 | 页数 | 标签 | 更新日期 |
|----|------|------|------|------|----------|

<!-- 添加新演示后，在此表格中添加条目 -->

## 目录结构

```
slide/
├── presentations/          # 各演示文稿
│   └── _template/          # 新演示模板
│       ├── slides.md       # 入口 + 元数据
│       ├── slides/         # 内容拆分
│       ├── workspace/      # 素材工作区
│       ├── public/         # 最终资源
│       └── archive/        # 版本归档
├── assets-shared/          # 全局共享素材
├── theme-shared/           # 共享主题
├── docs/                   # 项目文档
└── README.md
```

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

1. 复制 `presentations/_template/` 为新目录
2. 更新 `slides.md` 的元数据（id、title、tags 等）
3. 在 README.md 演示列表中添加新条目