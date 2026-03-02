# Framework Atlas — 9 Decision Frameworks for Agent Operations

> Generated: 2026-02-19 | Self-Improving Agent Forge output
> Purpose: Operational decision frameworks used across all PrimeFold OS agents

---

## FW-01: Output Type Decision Tree

**Purpose:** Determine correct output format BEFORE generating

```
IF output is code AND >20 lines -> FILE (file_create -> present_files)
IF output is code AND <=20 lines -> CODE BLOCK in chat
IF output is a document -> FILE (.md, .docx, etc.)
IF output is a diagram -> MERMAID file or SVG
IF output is a quick answer -> CHAT TEXT
IF output is a React component -> .jsx FILE
IF uncertain -> DEFAULT TO FILE (safer than chat text)
```

---

## FW-02: Task Complexity Estimator

**Purpose:** Right-size effort and token budget

| Level | Description | Token Budget | Example |
|-------|-------------|-------------|---------|
| L1 — Trivial | Quick answer, lookup | <200 | "What's the Pine Script function for X?" |
| L2 — Simple | Single focused task | 200-500 | Fix one error, write one function |
| L3 — Moderate | Multi-step task | 500-1500 | Build a module, write a prompt |
| L4 — Complex | Full build or analysis | 1500-3000 | Complete indicator, full product spec |
| L5 — Massive | Multi-artifact project | 3000+ (use files) | System architecture, full product build |

---

## FW-03: Confidence Scoring Model

**Purpose:** Tag every technical/factual claim with confidence level

| Level | Label | Definition | How to Communicate |
|-------|-------|-----------|-------------------|
| 6 | VERIFIED | Tested, compiled, confirmed | State as fact |
| 5 | HIGH CONFIDENCE | Strong evidence, high certainty | State normally |
| 4 | PROBABLE | Likely correct based on knowledge | "This should work" |
| 3 | UNCERTAIN | May be correct, haven't verified | "I believe X but haven't confirmed" |
| 2 | SPECULATIVE | Educated guess | "My best guess is X — verify before using" |
| 1 | UNKNOWN | No basis for claim | "I don't know" (say it) |

---

## FW-04: Edit vs Rebuild Decision Matrix

**Purpose:** Prevent wasteful recompilation

| Change Scope | Action | Confirmation Needed? |
|-------------|--------|---------------------|
| <10% of content | Surgical edit (str_replace) | No |
| 10-30% | Targeted section rewrite | No, but note what changed |
| 30-60% | Major revision | YES — ask operator first |
| >60% | Full rebuild | YES — explain why rebuild is better than edit |

**Default bias:** Always try edit first. Rebuild is the exception, never the default.

---

## FW-05: Pre-Flight Checklist

**Purpose:** Gate before any major output (>100 lines or code delivery)

```
[ ] 1. SCOPE: Does this match what was asked? (not what I think would be cool)
[ ] 2. FORMAT: Am I using the right output type? (FW-01)
[ ] 3. SIZE: Is this the minimum needed? (FW-02)
[ ] 4. CONFIDENCE: Are my technical claims verified? (FW-03)
[ ] 5. EDIT CHECK: Should I edit existing work instead of creating new? (FW-04)
[ ] 6. FRUSTRATION: Would this make the operator frustrated? (RED-01)
[ ] 7. DELIVERY: How will I confirm the operator received this?
```

---

## FW-06: Operator Communication Protocol

**Purpose:** Match response style to operator's current state

| Operator Signal | Agent Response Style |
|----------------|---------------------|
| Short, direct messages | Match brevity. Execute. Don't elaborate. |
| "Just do it" / "ship it" | Zero questions. Execute immediately. |
| Asking questions | Answer directly, then ask ONE follow-up max |
| Frustrated / terse | Acknowledge, fix, no excuses, no over-apologizing |
| Exploratory / brainstorming | Match energy, offer structured options |
| "Wrap" / "done" / "save" | Session commit (MEM-01), no new work |

---

## FW-07: Risk Classification for PrimeFold

**Purpose:** Score any proposed work on 5 dimensions

| Dimension | Weight | Score 1 (bad) | Score 5 (good) |
|-----------|--------|--------------|----------------|
| Revenue Connection | 30% | No path to revenue | Direct revenue |
| Time to Ship | 25% | >2 weeks | <2 days |
| Dependencies | 20% | Needs 3+ other things first | Self-contained |
| Validated Demand | 15% | Theory only | People asking for it |
| Maintenance Cost | 10% | Ongoing updates needed | Set and forget |

**Thresholds:** Score >3.5 = GO. Score 2.5-3.5 = HOLD. Score <2.5 = KILL.

---

## FW-08: PineScript Validation Pipeline

**Purpose:** Prevent chronic Pine Script failures

### Pre-Flight Checks (Before ANY Pine Script Output)

```
[ ] 1. Pine Script version declared (v5, v6)
[ ] 2. No Unicode characters in strings (use ASCII only)
[ ] 3. Argument order matches TradingView docs
[ ] 4. Multi-line boolean expressions use proper continuation
[ ] 5. String concatenation uses str.format() or + operator correctly
[ ] 6. No duplicate variable declarations
[ ] 7. All custom functions defined BEFORE first call
[ ] 8. indicator() / strategy() call has correct parameters
```

### Validation Steps
1. Write code in file (not chat)
2. Run Pre-Flight Checks above
3. Check line count vs TradingView limits (~25,000 chars)
4. Verify all plot() calls have valid series inputs
5. Check for table/label limits (max 500 labels)
6. Present to operator with known limitations noted

---

## FW-09: Existing Skill Ecosystem Map

**Purpose:** Know what already exists before building new

### 44 Skills by Category

| Category | Count | Skills |
|----------|-------|--------|
| Strategy & Governance | 7 | SEF, Core Governance, Strategist, Auditor, 80/20 Analysis, Reality Check, Intelligence Taxonomy |
| Product Design | 4 | VEF, Architect, Hormozi Offers, Economy of Plenty |
| Content & Copy | 4 | CEF, Copy Crafter, Forge, Tone Tailor |
| Build & Assembly | 5 | Builder, Assembler, Orchestrator, Slicer, GPT Product Engineer |
| Shipping & Launch | 6 | Deployer, Launch Readiness Gate, Pricing Sanity Check, Search Metadata Keywords, Copy Consistency Linter, Gumroad Listing Template |
| Trading | 2 | PrimeFold Trading, PineScript Architect |
| Knowledge & Learning | 3 | KEF, Cognition Primitives, LLM Primitives Atlas |
| Quality & Security | 3 | GPT Security Gate, FactGuard Pro, Schema Validator |
| System & Meta | 4 | Skill Forge, Skill Enforcement, Pipeline Manager, Prompt Compiler |
| Research & Analysis | 3 | Research Swarm, Simulation Framework, Legal Risk Assessment |
| Specialized | 3 | Reddit Risk Evaluator, TradingView Strategist, Post-Launch Signal Extractor |

### Coverage Gaps Identified
- No skill for: agent self-improvement, context management, token optimization, output verification

---

*Source: Notion page 30df6fcc-77bf-8193 (04 — Framework Atlas)*
*Exported: 2026-03-02*
