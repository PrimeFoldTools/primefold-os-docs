# PrimeFold OS — Architecture Documentation

Core operating system documentation for PrimeFold.Tools — the AI-powered publishing platform infrastructure.

## Contents

### Core Architecture

| File | Type | Description |
|------|------|-------------|
| `master-brand-architecture.md` | Brand | Brand hierarchy, color system, typography, logo assets, and usage rules |
| `five-pillar-architecture.md` | Architecture | 5-pillar publishing model with Memory Law and product inventory |
| `os-context-block.md` | Context | Compressed session loader — identity, decision gates, constraints, AI rules |
| `workspace-architecture-map.md` | Infrastructure | Full workspace inventory — tiers, databases, agent tools, health metrics |

### Agent System

| File | Type | Description |
|------|------|-------------|
| `build-standards-v2.4.3.md` | Standards | OS Build Standards — 15-agent spec, canonical blueprint template, handoff chains, OS_LOCK enforcement |
| `agent-blueprint-template.md` | Template | Canonical spec template for all PrimeFold agents and skills |
| `agent-class-architecture.md` | Framework | GPT Inheritance Framework — shared kernel -> base class -> subclass specialization |
| `agent-specs-rebranded.md` | Specs | Full specs for KEF Architect, SEF Strategist, Optimizer Agent, Trading Coach |

### Frameworks & Standards

| File | Type | Description |
|------|------|-------------|
| `framework-atlas.md` | Frameworks | 9 decision frameworks — output types, complexity, confidence, edit vs rebuild, pre-flight, comms protocol |
| `naming-versioning-standards.md` | Standards | Asset type definitions, sorting decision tree, versioning format |
| `launch-roadmap.md` | Roadmap | 6-phase launch sequence with hard gates, revenue scenarios, and scale criteria |

### Reference

| File | Type | Description |
|------|------|-------------|
| `asset-index.md` | Reference | Claude quick-lookup with ~120 indexed entries across Prompt Vault and Skill Library |

## System Architecture

PrimeFold.Tools operates as a multi-agent AI publishing system with four execution layers:

```
Collin (Commander)         <- Approvals, strategy, final judgment
  |- Cowork (Operator)     <- Notion, documents, skill orchestration
  |- Claude Code (Builder) <- Code, git, MCP servers, scripts
  '- Browser (Scout)       <- Web deployment, research
```

### Agent Pipeline (15 Agents)

```
Idea Inbox (SEF Gate 0)
    |
KEF Architect -> VEF Builder -> Product Slicer
    |
Content Multiplier -> Campaign Builder -> Launch Strategist
    |
Optimizer Agent -> Data Interpreter -> SEF Strategist -> (loop)
```

**Support:** FEF Manager (blockers), Support Assistant (customers)
**Trading:** PrimeFold Trading Coach -> Risk Manager
**Registry:** Risk Manager, Compliance Gatekeeper

### Governance Model
- 4-gate system: GO / GROW / HOLD / KILL
- Family-test before market release
- AI advises, operator decides
- OS_LOCK enforcement across all agents

## License

Private — internal use only.
