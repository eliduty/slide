---
layout: TwoCols
---

# 6.2 完整项目结构参考

::left::

<div class="directory-tree">

```
project-root/
├── .agents/               # Agent技能库
├── .claude/               # Claude配置
├── apps/                  # 应用层（前端/后端）
│   └── {app}/
│       ├── CLAUDE.md
│       ├── openspec/
│       └── src/
├── packages/              # 共享包
│   ├── shared-domain/
│   └── ui-components/
├── docs/                  # 文档分层
├── openspec/              # 功能规格管理
├── scripts/               # 脚本工具
├── deploy/                # 部署配置
├── CLAUDE.md              # 根规则文件
├── pnpm-workspace.yaml
└── tsconfig.base.json
```

</div>

::right::

| 目录 | 用途 |
|:-----|:-----|
| .agents/ | Agent核心技能库 |
| .claude/ | Claude命令+技能链接 |
| apps/ | 前端/后端应用 |
| packages/ | 领域/基础设施/UI共享包 |
| docs/ | architecture/requirements/design/standards |
| openspec/ | specs + changes 变更追踪 |
| scripts/ | 构建/部署脚本 |
| deploy/ | Docker/K8s配置 |

<style>
.directory-tree pre {
  font-size: 12px;
  line-height: 1.4;
}
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
}
td:first-child {
  font-family: var(--font-family-code);
  font-weight: var(--font-weight-medium);
}
</style>

<!--
这是 skill 项目实际使用的完整目录结构。

Monorepo 的核心优势：
- **apps/** 集中管理所有应用，每个应用有自己的 CLAUDE.md 和 openspec
- **packages/** 共享代码，避免重复，领域层和基础设施层清晰分离
- **docs/** 分层组织：architecture（架构）、requirements（PRD）、design（UI/UX）、standards（规范）、guides（指南）各自独立，易于查找
- **openspec/** 功能规格管理，支持从提案到实现的完整追踪

这套结构已经在 skill 项目验证，可直接复用。

接下来是课后自学指引。
-->
