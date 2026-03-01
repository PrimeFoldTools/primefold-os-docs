# PrimeFold Naming + Versioning Standard v2.0

**Version:** 2.0 | **Owner:** PrimeFold | **Migrated from:** Nexum Naming + Versioning Standards v2.4.2a
**Updated:** 2026-02-22 — Expanded definitions, sorting tests, loading model clarified.

---

## How Claude Loads Assets

All asset types below can be *used* by Claude. The difference is how they get loaded:

**Always-on (ambient):** Skills uploaded as `.md` files to Claude Projects (`/mnt/skills/user/`). Available in every conversation without asking. Claude can read and execute them automatically.

**On-demand (fetched):** Everything in Notion — prompts, stacks, frameworks, SOPs, templates. Claude fetches the page via Notion tools, reads the content, then executes it. Functionally identical to a skill once loaded, but requires a fetch step.

**Implication:** If a prompt is used every session, it should probably be a skill. If a skill is only used occasionally, it could live as a prompt in the Vault instead. The "Claude Can Load" checkbox in Prompt Vault tracks which prompts are formatted for direct Claude execution.

---

## Asset Type Definitions

### SKILL
**What it is:** A *behavior* Claude can perform autonomously. Has a trigger, defined inputs, defined outputs, and runs without operator copy-pasting.
**Sorting test:** "Can Claude run this without me pasting anything?" → Yes = Skill.
**Lives in:** Skill Library (database) + `/mnt/skills/user/` (file system for ambient loading)
**Examples:** PARSE, FILE, LIBRARIAN, CAPTURE, pinescript-architect, tone-tailer

### PROMPT
**What it is:** Text you paste into (or Claude fetches into) a conversation to get a specific output. Single-purpose, self-contained instructions.
**Sorting test:** "Is this a set of instructions for one specific task?" → Yes = Prompt.
**Lives in:** Prompt Vault (Category: 🤖 GPT System Prompt, or uncategorized)
**Examples:** Reddit Post Generator, Gumroad Ship Prompt, Trading Journal Review

### STACK
**What it is:** Multiple prompts chained in sequence. A *workflow* where each step's output feeds the next. Produces a larger deliverable than any single prompt.
**Sorting test:** "Does this have numbered phases where output flows forward?" → Yes = Stack.
**Lives in:** Prompt Vault (Category: 🔗 Stack)
**Examples:** Carrd Masterstack, Notion Brain Ingestion Engine, Knowledge Slicer & Funnel Builder

### FRAMEWORK
**What it is:** A *thinking model* — not executable instructions. Defines categories, decision trees, mental models, or taxonomies. You reference it to make decisions; you don't "run" it.
**Sorting test:** "Does this tell me *how to think about something* rather than *what to do*?" → Yes = Framework.
**Lives in:** Prompt Vault (Category: 📐 Framework)
**Examples:** KEF, Economy of Plenty, Intelligence Taxonomy, Cognition Primitives Reference

### SOP
**What it is:** A *human* procedure. Step-by-step instructions for Collin (or an agent acting as Collin), not for Claude to interpret creatively.
**Sorting test:** "Am I (the human) executing these steps in order?" → Yes = SOP.
**Lives in:** Prompt Vault (Category: 📏 SOP)
**Examples:** Strip Mine Protocol, Product Launch Checklist, Gumroad listing steps

### TEMPLATE
**What it is:** A fill-in-the-blank pattern. Structure is fixed; content varies per use.
**Sorting test:** "Do I replace [BRACKETED] fields to use this?" → Yes = Template.
**Lives in:** Prompt Vault (Category: 📋 Template)
**Examples:** GPT Standard Template, Compiled Prompt Output Format, Assembly Plan Templates

### Other Prompt Vault Categories
- **🎯 Context Loader** — Background information Claude reads before working. Not instructions, just context.
- **🔁 Ritual / Trigger** — Recurring prompts tied to a cadence (daily, weekly, per-session).
- **📦 Product Builder** — Prompts specifically for assembling sellable products.
- **📣 Marketing / Copy** — Prompts for content creation, landing pages, sales copy.
- **🧠 Meta / Infrastructure** — System-level prompts about the OS itself.

---

## Sorting Decision Tree

When filing a new asset, ask in order:

1. **Is it a `.md` file Claude loads automatically every session?** → SKILL (Skill Library)
2. **Is it a fill-in-the-blank pattern?** → TEMPLATE
3. **Is it a human step-by-step procedure?** → SOP
4. **Is it a thinking model / taxonomy / decision framework?** → FRAMEWORK
5. **Does it chain multiple steps where output feeds forward?** → STACK
6. **Is it instructions for one specific task?** → PROMPT

*When ambiguous:* Default to the type that matches the asset's *primary use*. A framework that includes execution steps is still a framework if its core value is the mental model. A prompt that references a framework is still a prompt.

---

## Versioning Format

- Major.Minor: v1.0, v1.1, v2.0
- Draft in progress: Add -DRAFT: v0.1-DRAFT
- Patches: v1.0.1 (hotfix only)

## File Naming

- Format: `TYPE_NAME_vX.X.md`
- Example: `FRAMEWORK_CAP_v1.0.md`
- No spaces in filenames, use underscores

---

## Version History

- **v2.0** (2026-02-22): Expanded all definitions with sorting tests, added loading model explanation, added decision tree, added Prompt Vault sub-categories.
- **v1.0** (2026-02-20): Initial migration from Nexum Naming Standards v2.4.2a. One-liner definitions only.
