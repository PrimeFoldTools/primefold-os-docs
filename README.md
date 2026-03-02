# PrimeFold OS — Architecture Documentation

Core operating system documentation for PrimeFold.Tools — the AI-powered publishing platform infrastructure.

## Contents

| File | Type | Description |
|------|------|-------------|
| `master-brand-architecture.md` | Brand | Brand hierarchy, color system, typography, logo assets, and usage rules |
| `five-pillar-architecture.md` | Architecture | 5-pillar publishing model with Memory Law and product inventory |
| `agent-blueprint-template.md` | Template | Canonical spec template for all PrimeFold agents and skills |
| `os-context-block.md` | Context | Compressed session loader — identity, decision gates, constraints, AI rules |
| `naming-versioning-standards.md` | Standards | Asset type definitions, sorting decision tree, versioning format |
| `workspace-architecture-map.md` | Infrastructure | Full workspace inventory — tiers, databases, agent tools, health metrics |
| `asset-index.md` | Reference | Claude quick-lookup with ~120 indexed entries across Prompt Vault and Skill Library |

## System Architecture

PrimeFold.Tools operates as a multi-agent AI publishing system with four execution layers:

```
Collin (Commander)         ← Approvals, strategy, final judgment
  ├── Cowork (Operator)    ← Notion, documents, skill orchestration
  ├── Claude Code (Builder)← Code, git, MCP servers, scripts
  └── Browser (Scout)      ← Web deployment, research
```

**Governance Model:**
- 4-gate system: GO / GROW / HOLD / KILL
- Family-test before market release
- AI advises, operator decides

## License

Private — internal use only.
