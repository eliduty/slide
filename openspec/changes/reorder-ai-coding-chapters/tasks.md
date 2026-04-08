## 1. 准备工作

- [x] 1.1 备份当前 slides 目录，防止操作失误
- [x] 1.2 确认当前文件编号和内容对应关系

## 2. 文件重命名

- [x] 2.1 将 11-15 文件临时重命名为 temp-11 到 temp-15
  - `11-chapter3-section.md` → `temp-11-chapter3-section.md`
  - `12-chapter3-pm.md` → `temp-12-chapter3-pm.md`
  - `13-chapter3-sdeqa.md` → `temp-13-chapter3-sdeqa.md`
  - `14-chapter3-review.md` → `temp-14-chapter3-review.md`
  - `15-chapter3-summary.md` → `temp-15-chapter3-summary.md`

- [x] 2.2 将 16-21 文件重命名为 11-16
  - `16-chapter4-section.md` → `11-chapter4-section.md`
  - `17-chapter4-requirement.md` → `12-chapter4-requirement.md`
  - `18-chapter4-design.md` → `13-chapter4-design.md`
  - `19-chapter4-implementation.md` → `14-chapter4-implementation.md`
  - `20-chapter4-global.md` → `15-chapter4-global.md`
  - `21-chapter4-context.md` → `16-chapter4-context.md`

- [x] 2.3 将临时文件重命名为 17-21
  - `temp-11-chapter3-section.md` → `17-chapter3-section.md`
  - `temp-12-chapter3-pm.md` → `18-chapter3-pm.md`
  - `temp-13-chapter3-sdeqa.md` → `19-chapter3-sdeqa.md`
  - `temp-14-chapter3-review.md` → `20-chapter3-review.md`
  - `temp-15-chapter3-summary.md` → `21-chapter3-summary.md`

## 3. slides.md 入口文件更新

- [x] 3.1 更新 slides.md 中的 src 引用顺序
  - 调整第3章和第4章的 src 引用位置
  - 保持第1章、第2章、第5章、附录顺序不变

- [x] 3.2 更新 slides.md 中的章节注释
  - 更新 `<!-- 第3章 -->` 和 `<!-- 第4章 -->` 注释位置

## 4. 新增内容

- [x] 4.1 创建环境规范阶段应用页面（整合到 15-chapter4-global.md，更新标题为"环境规范与全局规则"）
  - 内容：开发环境配置、测试环境准备、领域知识文档、验证方法
  - 位置：在 14-chapter4-implementation 之后

- [x] 4.2 增强 21-chapter3-summary 页面，增加能力培养路线图
  - 内容：初级/中级/高级能力定义、学习路径、具体任务建议
  - 格式：参考 27-self-study.md 的样式，增加能力培养表格

- [x] 4.3 在 11-chapter4-section.md 开头增加过渡语句
  - Speaker notes 增加："上一章我们讲了四阶段工作流，这章我们来看每个阶段具体怎么用 AI"

- [x] 4.4 在 17-chapter3-section.md 开头增加过渡语句
  - Speaker notes 增加："前面讲了各阶段怎么用，现在来看对你的影响"

## 5. 内容优化

- [x] 5.1 更新 02-agenda.md 的议程顺序描述
  - 调整第3章和第4章的时间分配描述

- [x] 5.2 检查所有章节页的 speaker notes，确保过渡语句连贯

## 6. 验证

- [x] 6.1 运行 `pnpm dev:ai-coding` 验证幻灯片顺序正确
- [x] 6.2 检查所有 src 引用路径有效，无缺失文件
- [x] 6.3 验证新增内容渲染正确，样式一致
- [x] 6.4 预览演讲流程，确认叙事逻辑连贯