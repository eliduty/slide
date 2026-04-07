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