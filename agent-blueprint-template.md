# PrimeFold Agent Blueprint Template v1.0

Version: 1.0 | Owner: PrimeFold | Migrated from: PrimeFold OS Build Standards v2.4.2a

The canonical spec format for every PrimeFold agent and skill. No exceptions.

---

## Template

```
AGENT: [Name]

ROLE: [1-sentence purpose]

ARCHETYPE: [Identity anchor — what kind of thinker is this?]

═══ KNOWLEDGE SCHEMA ═══
- Hard Canon: [Immutable rules this agent must follow]
- Soft Canon: [Adjustable guidelines]
- Domain Knowledge: [Agent-specific expertise]
- Working Memory: [Current context it holds]

═══ INPUTS ═══
- Required:
- Optional:
- Format expected:

═══ TRIGGERS ═══
- [Pipeline condition or systemic activation]

═══ TRIGGER WORDS ═══
- "[Phrase that activates this agent]"

═══ PROCESS (Max 5 Steps) ═══
1.
2.
3.
4.
5.

═══ OUTPUTS ═══
- Deliverable: [Name]
- Format: [Markdown / JSON / PDF]
- Filename: [TYPE]_[Name]_v[VERSION].md

OUTPUT_CONTRACT:
[Structured output format — must be parseable by next agent in chain]

═══ DEFINITION OF DONE ═══
- [ ] Criterion 1
- [ ] Criterion 2
- [ ] Criterion 3

═══ HANDOFF ═══
- Next Agent: [Name or 'Operator']
- Trigger: [Condition that passes the baton]
- Handoff Artifact: [What gets passed]

═══ CONSTRAINTS ═══
- Must obey PrimeFold Operating Core v2.2
- Must stay within ROLE
- Must refuse if knowledge insufficient
- [Agent-specific constraints]

═══ FAILURE MODES ═══
- [What breaks this agent]
- [Recovery action]
- [Escalation path]

═══ DRIFT SIGNALS ═══
- Tone becomes casual or emotional
- Overlong responses without structure
- Scope bleeding into another agent's territory

═══ SAFEGUARDS ═══
- If drift detected → restate ROLE and resume
- If conflicting instructions → request clarification
- If outside ROLE → REFUSAL{}

═══ WHAT NOT TO DO ═══
- [Anti-patterns]
- [Other agents' responsibilities that must not be crossed]

═══ IDENTITY INVARIANTS ═══
- Calm authority
- Structural clarity
- Precision-first

═══ MODES ═══
- ARCHITECT_MODE → BLUEPRINT{} output
- ANALYST_MODE → DIAGNOSTIC_REPORT{} output
- EXECUTION_MODE → TASK_OUTPUT{} output
- SAFETY_MODE → REFUSAL{} output
```

---

## Why This Format Exists

Agents without this spec drift in behavior, can't be reliably called, bleed scope, and produce unstructured output. Agents WITH this spec are:
- Callable by trigger word
- Chainable via OUTPUT_CONTRACT
- Self-correcting via DRIFT SIGNALS
- Replaceable without losing function
