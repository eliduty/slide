# 元数据规范

## slides.md 演示级元数据

每个演示的 `slides.md` 入口文件包含完整的元数据配置：

```markdown
---
# Slidev 标准配置
theme: ../theme-shared
title: 技术介绍
author: eliduty
aspectRatio: 16/9
colorSchema: auto

# 自定义元数据（AI管理用）
id: tech-intro
created: 2026-03-28
updated: 2026-03-28
tags: [tech, intro, frontend]
slidesCount: 12
estimatedTime: 15min
status: draft
---
```

### 字段说明

| 字段 | 类型 | 必需 | 说明 |
|------|------|------|------|
| `theme` | string | 是 | 共享主题路径：`../theme-shared` |
| `title` | string | 是 | 演示标题 |
| `author` | string | 否 | 作者名称 |
| `aspectRatio` | string | 否 | 宽高比，默认 `16/9` |
| `colorSchema` | string | 否 | 颜色模式：`auto` / `light` / `dark` |
| `id` | string | 是 | 演示唯一标识，与目录名一致 |
| `created` | date | 是 | 创建日期 |
| `updated` | date | 是 | 最后更新日期 |
| `tags` | array | 否 | 标签列表，便于分类 |
| `slidesCount` | number | 否 | 总页数 |
| `estimatedTime` | string | 否 | 预计时长 |
| `status` | string | 是 | 状态：`draft` / `reviewing` / `ready` / `published` |

---

## slides/*.md 页级元数据

每个拆分的内容文件可包含页级元数据：

```markdown
---
title: 项目介绍
order: 2
duration: 3min
keyPoints:
  - 了解项目背景
  - 理解核心概念
---

## 项目背景

内容...
```

### 字段说明

| 字段 | 类型 | 必需 | 说明 |
|------|------|------|------|
| `title` | string | 否 | 该页标题 |
| `order` | number | 否 | 在演示中的顺序 |
| `duration` | string | 否 | 该页预计时长 |
| `keyPoints` | array | 否 | 关键要点列表 |