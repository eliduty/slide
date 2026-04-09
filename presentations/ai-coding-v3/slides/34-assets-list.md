---
layout: TwoCols
---

::left::

# 6.1 标准化资产清单

| 资产类型 | 文件 |
|:--------:|:-----|
| 需求模板 | prd-template.md |
| 设计模板 | spec-template.md |
| AI规则 | CLAUDE.md |
| Prompt库 | prompts/*.md |
| Review清单 | rules/*.md |
| Skills库 | skills/*/SKILL.md |

::right::

<strong>资产目录结构</strong>

```
team-ai-coding-toolkit/
├── CLAUDE.md              # 项目开发规则
├── docs/
│   ├── architecture/      # 架构设计
│   ├── requirements/      # PRD、需求规范
│   ├── design/            # UI/UX设计
│   ├── standards/         # 技术规范
│   ├── guides/            # 操作指南
│   └── prompts/           # Prompt库
├── openspec/
│   ├── specs/             # 功能规格库
│   └── changes/           # 变更追踪
├── .agents/
│   └── skills/            # Agent技能库
└── .claude/
    ├── rules/             # 开发规范检查
    └── skills/            # Claude技能链接
```

<style>
table {
  width: 100%;
  border-collapse: collapse;
}
th, td {
  padding: var(--spacing-xs) var(--spacing-sm);
  border: 1px solid var(--color-border);
  font-size: var(--font-size-card-meta);
}
th {
  background: var(--color-bg-subtle);
  font-family: var(--font-family-display);
  font-weight: var(--font-weight-medium);
}
td:first-child {
  text-align: center;
}
code, pre {
  font-family: var(--font-family-code);
  font-size: 13px;
}
</style>

<!--
培训结束后，每个团队应该持有这些资产：

- **需求模板**：prd-template.md，写需求的标准格式
- **设计模板**：spec-template.md，技术设计的标准格式
- **AI规则文件**：CLAUDE.md，告诉 AI 项目规则
- **Prompt库**：prompts/*.md，常用任务的 prompt
- **Review Checklist**：rules/*.md，开发规范检查清单
- **Skills库**：skills/*/SKILL.md，实操指南

这些资产在职业素养测评项目中都已经有了，大家有些可以直接复用。

接下来看这些资产的具体目录结构。
-->
