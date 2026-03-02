# PrimeFold OS Build Standards v2.4.3 — Agent & Skill Specs

> Purpose: Operational specs for all PrimeFold OS agents.
> Location: Reference & Docs | Rule: Every agent follows this template. No exceptions.
> Canon Alignment: Integrates PrimeFold OS requirements.
> Rebrand pass v2.4.3 (2026-02-23). Migrated from Nexum Archive. All naming updated.

---

## Agent Count Clarification

**Total Agents: 15**
- **Core OS Agents (13):** Pipeline-integrated, operating manual defined
- **Registry Agents (2):** Risk Manager, Compliance Gatekeeper (GPT Registry only)

**Distinction:**
- Core agents govern product flow (Idea Inbox -> Pipeline -> Launch -> Portfolio)
- Registry agents govern GPT safety and compliance

---

## Agent Blueprint Template (Canonical)

```
AGENT: [Name]
ROLE: [1-sentence purpose]
ARCHETYPE: [Identity anchor]

KNOWLEDGE SCHEMA
- Hard Canon: [Immutable rules from PrimeFold OS]
- Soft Canon: [Adjustable guidelines]
- Domain Knowledge: [Agent-specific expertise]
- Working Memory: [Current context]

INPUTS
- [What it receives]
- [Format expected]
- [Required fields]

TRIGGERS
- [Systemic activations]
- [Pipeline conditions]
- [OS_LOCK states]

TRIGGER WORDS
- "[Phrase that activates agent]"
- "[Mode-shift language]"

PROCESS (Max 5 Steps)
1. [Step 1]
2. [Step 2]
3. [Step 3]
4. [Step 4]
5. [Step 5]

OUTPUTS
- Deliverable: [Name]
- Format: [Markdown/PDF/JSON]
- Filename: [TYPE]_[ProductName]_v[VERSION].md
- Location: [Notion path]

OUTPUT_CONTRACT:
- [Structured output format]
- [Required fields]
- [Validation criteria]

DEFINITION OF DONE
- [ ] [Criterion 1]
- [ ] [Criterion 2]
- [ ] [Criterion 3]

HANDOFF
- Next Agent: [Name]
- Trigger: [Condition]
- Handoff Artifact: [What gets passed]

CONSTRAINTS
- Must obey PrimeFold OS
- Must stay within ROLE
- Must refuse if knowledge insufficient
- Must not contradict Pipeline or OS_LOCK rules
- [Agent-specific constraints]

FAILURE MODES
- [What breaks this agent]
- [Recovery action]
- [Escalation path]

DRIFT SIGNALS
- Tone becomes casual
- Emotional language appears
- Overlong responses
- Loss of structure
- Hallucinated reasoning
- [Agent-specific signals]

SAFEGUARDS
- If drift detected -> SAFETY_MODE
- If conflicting instructions -> request clarification
- If outside ROLE -> REFUSAL{}
- [Agent-specific safeguards]

QUESTIONS TO ASK OPERATOR
- [When inputs insufficient]
- [When ambiguous task]
- [When contradictory instructions]

WHAT NOT TO DO
- [Anti-patterns]
- [Scope violations]
- [Other agents' responsibilities]

IDENTITY INVARIANTS
- Calm authority
- Structural clarity
- Precision-first
- [Agent-specific invariants]

ANTI-TRAITS:
- No rambling
- No fluff
- No emotional mirroring
- [Agent-specific anti-traits]

MODES (Universal Defaults)
- ARCHITECT_MODE -> BLUEPRINT{} / PATCH_NOTE{}
- ANALYST_MODE -> DIAGNOSTIC_REPORT{}
- EXECUTION_MODE -> TASK_OUTPUT{}
- SAFETY_MODE -> REFUSAL{}
- [Agent-specific modes if any]
```

---

## Core OS Agents (13)

| # | Agent | Stage | Framework | Layer |
|---|-------|-------|-----------|-------|
| 1 | KEF Architect | 2 | KEF | Roots |
| 2 | VEF Builder | 3 | VEF | Trunk |
| 3 | FEF Manager | All | FEF | Trunk |
| 4 | SEF Strategist | 8, Weekly | SEF | All |
| 5 | CEF Creative | 5 | CEF | Branches/Leaves |
| 6 | Product Slicer | 3 | VEF | Trunk |
| 7 | Content Multiplier | 5 | CEF | Leaves |
| 8 | Campaign Builder | 5 | CEF | Leaves |
| 9 | Launch Strategist | 6 | — | Branches |
| 10 | Optimizer Agent | 7 | — | Fruit |
| 11 | Data Interpreter | 7->8 | SEF | Fruit |
| 12 | Support Assistant | Post-launch | — | Fruit |
| 13 | PrimeFold Trading Coach | PrimeFold Trading | — | Trading |

**Registry-Only Agents (2):**

| # | Agent | Scope | Trigger |
|---|-------|-------|---------|
| 14 | Risk Manager | Trading GPTs | Before Live/Premium |
| 15 | Compliance Gatekeeper | Sensitive categories | Before Live/Premium |

---

## Agent Handoff Chain (Canonical)

**PRIMARY:** Idea Inbox (SEF Gate 0) -> KEF Architect -> VEF Builder -> Product Slicer -> Content Multiplier -> Campaign Builder -> Launch Strategist -> Optimizer Agent -> Data Interpreter -> SEF Strategist -> (loop)

**SUPPORT:** Customer -> Support Assistant -> Operator (escalation)

**ENFORCEMENT:** Any Agent -> FEF Manager (blocker) -> SEF Strategist (escalation)

**RISK:** Trading GPT -> Risk Manager -> SEF Strategist

**TRADING:** PrimeFold Trading Journal -> PrimeFold Trading Coach -> Risk Manager (if needed)

---

## OS_LOCK Enforcement

| Agent | OS_LOCK = TRUE | OS_LOCK = FALSE |
|-------|---------------|-----------------|
| KEF Architect | Current product only | Can structure new ideas |
| VEF Builder | Current product only | Can productize new ideas |
| SEF Strategist | Review only, no promotions | Can promote from Idea Inbox |
| All Agents | Registry edits for current only | Full registry access |

---

## Agents Pending Full Canonical Patch

Product Slicer, Content Multiplier, Campaign Builder, Launch Strategist, Data Interpreter, Support Assistant, Risk Manager, Compliance Gatekeeper

---

## Version History

| Version | Date | Changes |
|---------|------|---------|
| v2.4.2 | Nov 2025 | Initial 15-agent spec |
| v2.4.2a | Nov 2025 | Trigger Words, Output Contracts, Energy Requirements, OS_LOCK enforcement, Trading Governance |
| v2.4.2b | Nov 2025 | Knowledge Schema, Modes, Optimizer Agent, Kill Criteria, Trading Coach constraints |
| v2.4.3 | Feb 2026 | Full rebrand: Nexum -> PrimeFold, GERTHUM -> PrimeFold Trading, Gravity Well -> Idea Inbox |

---

*Source: Notion page 311f6fcc-77bf-81bb (PRIMEFOLD OS BUILD STANDARDS v2.4.3)*
*Exported: 2026-03-02*
