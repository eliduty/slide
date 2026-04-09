## Why

ai-coding-v3 版本的演示文稿需要基于 outline-v3.md 大纲实现完整的幻灯片内容。当前 slides.md 入口文件为空，slides/ 目录不存在。本次变更将完成约 39 页幻灯片的创建，包括新建 Part 0-4（约 23 页）和复用 v2 版本的 Part 5-8（约 15 页）。

## What Changes

- 创建 `presentations/ai-coding-v3/slides/` 目录结构
- 新建 Part 0-4 幻灯片内容文件（约 23 页）
- 复制 v2 版本 Part 5-8 对应幻灯片到 v3 目录（约 15 页）
- 更新 `slides.md` 入口文件的元数据和 src 引用
- 更新 slidesCount、estimatedTime、status 元数据

## Capabilities

### New Capabilities

- `ai-coding-v3-slides`: v3 版本演示文稿的完整幻灯片结构和内容

### Modified Capabilities

- `presentation-structure`: 扩展以支持 v3 版本的 8 个部分结构（Part 0-8）

## Impact

- `presentations/ai-coding-v3/` 目录
- `slides.md` 入口文件
- 新建 `slides/*.md` 约 39 个内容文件