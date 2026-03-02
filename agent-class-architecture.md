# PrimeFold Agent Class Architecture — GPT Inheritance Framework

| Field | Value |
|-------|-------|
| Status | Draft |
| Category | Framework |
| Domain | PrimeFold Publishing |
| Era | PrimeFold |
| Claude Can Load | Yes |
| Origin | Layer 15 — The Nexum AgentOS Inheritance Model (Dec 2025) |
| Harvested | 2026-02-25 |

**What This Solves:** Building 10, 50, 100 product-grade GPTs without rebuilding the entire system every time. Same pattern real operating systems use: shared kernel -> class structure -> specializations.

---

## Base Class: `PrimeFoldAgent`

Abstract class every product GPT inherits from.

```yaml
class PrimeFoldAgent:

  kernel: PRIMEFOLD_COGNITIVE_CORE

  # MUST override in subclass
  identity: SYSTEM_IDENTITY
  intent: SYSTEM_INTENT
  constraints: SYSTEM_CONSTRAINTS
  role: ROLE_DEFINITION
  scope: TASK_SCOPE
  knowledge: KNOWLEDGE_BASE

  # MAY override
  modes: MODE_ARCHITECTURE
  commands: COMMAND_STACK
  output_format: OUTPUT_FORMATS
  calibration_rules: USER_CALIBRATION
  archetypes: USER_ARCHETYPE_DETECTION

  # SHOULD NOT override (inherited from kernel)
  safety: SYSTEM_SAFETY
  truth_stack: TRUTH_ENFORCEMENT
  drift_detection: DRIFT_CORRECTION
  recovery: HARD_BLOCK_RECOVERY
```

Each subclass changes **only its personality and domain.** Safety, logic, identity enforcement, truth stack, drift protection — all inherited automatically from the kernel.

---

## Inheritance Pyramid

```
        PRIMEFOLD_COGNITIVE_CORE
                  |
                  v
         PrimeFoldAgent Base Class
                  |
   +--------------+---------------+--------------+
   v              v               v              v
Trading        Intelligence     Family        Publishing
Agents         Agents           Agents        Agents
   |              |               |              |
   v              v               v              v
Drill Coach    FactGuard Pro   StoryScape    PromptCraft
Bear Pack GPT  Bias Detective  DreamDay      Copy Crafter
Blindspot GPT  Claim Mapper    NOM NOM       Tone Tailor
```

Not writing GPTs. Writing **agent species** with shared DNA.

---

## 5 Specialization Layers (per subclass)

Each subclass selectively overrides:

1. **Identity Layer** — unique persona, epistemic stance, tone
2. **Intent Layer** — what transformation/outcome it creates
3. **Scope Layer** — what it does vs. refuses to do
4. **Knowledge Packs** — domain-specific files only
5. **Output Schema** — format varies by product (JSON, narrative, citations, structured analysis)

Everything else stays inherited.

---

## Kernel Binding Process

When instantiating a new agent:

```yaml
Agent = TradingDrillCoach()
```

Binding steps:
1. Load Kernel (PrimeFold Cognitive Core)
2. Override identity
3. Override intent
4. Override constraints
5. Override role
6. Load knowledge packs
7. Seal inheritance
8. Activate runtime cycle

You never rebuild: safety, truth stack, drift correction, mode state machines, output contracts, archetype detection, recovery pathways. They're universal.

---

## Competitive Advantage

- **Most GPT Store creators** mix architecture and content. This separates them: Kernel + Class + Overrides.
- **Most creators** copy-paste messy prompts. This uses inheritance and canonical configuration.
- **Most creators** build one-offs. This builds product families with shared DNA.
- **Most creators** can't guarantee consistency across products. This enforces it structurally.

---

## PrimeFold Implementation Notes

The Claude Skills system partially implements this pattern:
- Skills = specialized knowledge packs
- User Preferences = kernel-level configuration
- Skill SKILL.md files = class definitions with scope/constraints

What's NOT yet implemented:
- Formal base class that all GPT system prompts inherit from
- Automated binding process
- Shared safety/truth layer across all shipped GPTs

**When to implement:** After 3+ GPTs are live on GPT Store. The pattern becomes essential when maintaining consistency across 5+ products.

---

## Related

- PrimeFold Cognitive Core (skill: primefold-cognitive-core)
- GPT Product Engineer (skill: gpt-product-engineer)
- GPT Security Gate (skill: gpt-security-gate)

---

*Source: Notion page 313f6fcc-77bf-81c1 (PrimeFold Agent Class Architecture)*
*Exported: 2026-03-02*
