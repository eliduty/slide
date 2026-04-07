---
layout: TopTitleTwoCols
duration: 5min
---

::title::

# 标准化资产清单

::left::

<v-clicks>

## 培训后每个团队应持有的资产

| 资产类型 | 文件 | 用途 |
|---------|------|------|
| 需求模板 | prd-template.md | 写需求的标准格式 |
| 设计模板 | spec-template.md | 技术设计的标准格式 |
| AI规则文件 | CLAUDE.md | 告诉 AI 项目规则 |
| Prompt库 | prompts/*.md | 常用任务的 prompt |
| Review Checklist | rules/*.md | 开发规范检查清单 |
| Skills库 | skills/*/SKILL.md | 实操指南 |

</v-clicks>

::right::

<v-click>

## 标准化资产目录结构

```
team-ai-coding-toolkit/
├── CLAUDE.md
├── .claude/
│   ├── rules/
│   ├── commands/
│   └── skills/
├── docs/
│   ├── templates/
│   │   ├── prd-template.md
│   │   └─ spec-template.md
│   └─ prompts/
└── openspec/
    └── specs/
```

</v-click>