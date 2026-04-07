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
  padding: 0.4rem;
  border: 1px solid var(--color-border);
}
th {
  background: var(--color-primary-light);
  font-weight: 600;
}
td:first-child {
  text-align: center;
}
code, pre {
  font-size: 0.8rem;
}
</style>