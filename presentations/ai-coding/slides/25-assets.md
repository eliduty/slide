---
layout: TwoCols
---

::left::

# 标准化资产清单

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
├── CLAUDE.md
├── .claude/
│   ├── rules/
│   └── skills/
└── docs/templates/
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
好，我们接近尾声了。最后，我要给大家一份"武器清单"。

培训结束后，每个团队应该持有这些资产：

- **需求模板**：prd-template.md，写需求的标准格式
- **设计模板**：spec-template.md，技术设计的标准格式
- **AI规则文件**：CLAUDE.md，告诉 AI 项目规则
- **Prompt库**：prompts/*.md，常用任务的 prompt
- **Review Checklist**：rules/*.md，开发规范检查清单
- **Skills库**：skills/*/SKILL.md，实操指南

这些资产在 skill 项目中都已经有了，大家可以直接复用。
-->