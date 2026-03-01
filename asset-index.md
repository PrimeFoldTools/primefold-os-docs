# Asset Index — Claude Quick-Lookup (Prompts + Skills)

**Purpose:** Claude scans this page at session start (or when task-matching) to find the best asset for the job. Covers BOTH the Prompt Vault and the Skill Library.

**Rule:** If a prompt or skill exists for the task, use it instead of freestyling.

**Updated:** 2026-02-22 | Prompt Vault (~124 entries) + Skill Library (~62 entries, ~40 auto-loaded as .md)

**How loading works:**
- **Skills (.md files)** → Auto-loaded every conversation. Claude sees them without fetching. ✅ Already ambient.
- **Skills (Notion-only)** → In Skill Library DB but NOT auto-loaded. Must fetch from Notion. ⚠️ Indexed below.
- **Prompts/Stacks/Frameworks** → In Prompt Vault DB. Must fetch from Notion. ⚠️ Indexed below.

---

## 🔴 SHIP & SELL — Revenue-Critical Prompts

*Use these first. They directly support EXECUTE mode.*

| Task | Prompt | Type |
|------|--------|------|
| List a product on Gumroad | Gumroad Listing Generator | Prompt |
| Ship a product end-to-end | Gumroad Ship Prompt | SOP |
| Product launch checklist | Product Launch Checklist | SOP |
| Build a trading prompt pack | Trading Prompt Pack Generator | Stack |
| Standard output formats (Gumroad/Reddit/Ship) | Output Templates | Template |
| Write a Reddit value post | Reddit Post Generator | Prompt |
| Build/audit a Carrd site | Carrd Masterstack | Stack |
| Quick-audit a Carrd page | Carrd Surge | Stack |
| Carrd strategy + design | Carrd Expert | Stack |
| Price a product / build offer | Economy of Plenty Framework | Framework |
| Find monetization angles | Monetization Strategy Stack | Stack |
| Monetizable asset inventory | Monetizable Asset List v1.0 | Reference |
| Distribution channel strategy | Distribution Channel Strategy v1.0 | Framework |
| Offer matrix (pricing tiers) | Offer Matrix v1.0 | Framework |
| Product image brief | Gumroad Image Brief | SOP |

---

## 📈 TRADING — Products, GPTs, Indicators

*Trading-domain prompts for building and shipping trading tools.*

| Task | Prompt | Type |
|------|--------|------|
| Constraint Protocol reference | Constraint Protocol v1.3 | Framework |
| Anti-hallucination prompt pattern | Data Sandwich Architecture | Framework |
| GERTHUM discipline coaching prompt | GERTHUM Coach GPT | GPT Prompt |
| Trading drill system prompt | Trader DrillGPT | GPT Prompt |
| PineScript full system build | PineScript System Design Stack | Stack |
| PineScript audit + patch | PineScript Code Auditor | Stack |
| GERTHUMS indicator build | GERTHUMS TradingView Generator | Stack |
| Trading indicator user manual | Custom Trading Indicator Manual | Stack |
| GERTHUMS system extraction | GERTHUMS Playbook Extractor | Stack |
| GPT Store funnel strategy | GPT Store Funnel Strategy | Framework |
| GPT Store compliance | GPT Store Compliance Guide v1.0 | SOP |
| Bitcoin education system prompt | Bitcoin Scaffold GPT | GPT Prompt |
| Trading domain context | PrimeFold Trading Context Loader | Context |

---

## 🤖 GPT BUILDING — System Prompts, Templates, Architecture

*Use when building or refining any custom GPT.*

| Task | Prompt | Type |
|------|--------|------|
| GPT system prompt (blank template) | GPT System Prompt Template | Template |
| GPT build format (structured) | GPT Standard Template | Template |
| Design + build a custom GPT | Designing + Building a Custom GPT | Stack |
| GPT artifact builder | Integrated Artifact Builder | Stack |
| GPT system prompt audit | System Audit & Memory Update Engine | Stack |
| Token-aware patch consolidation | Token-Aware Production Patch | Template |
| AI publishing archetype framework | AI Publishing Stack | Framework |
| GPT role taxonomy (300+ roles) | GPT Taxonomy v1.0 | Framework |
| Multi-role orchestration | Multi-Role Fusion Template | Template |
| GPT monetization research | Market Intelligence Scan | Stack |

---

## ✍️ WRITING & BRAND — Voice, Copy, Content

*Use when writing anything public-facing.*

| Task | Prompt | Type |
|------|--------|------|
| Match Collin's writing voice | Voice Shaper / Voice Engine | Prompt |
| Amplify human writing style | Voice Shaper Stack | Stack |
| PrimeFold brand copy + positioning | PrimeFold Brand Copy Engine | Stack |
| Brand voice for ads/content | Brand Voice Engine | Stack |
| Competitive positioning copy | Competitive Positioning Copy Bank | Reference |
| Content strategy GPT builder | Content Strategy GPT Designer | Stack |
| YouTube strategy (compressed) | YouTube Strategy GPT | GPT Prompt |
| Resume / authority extraction | Resume & Authority Extractor | Stack |
| Copy GPT research + build | Copy GPT Architect | Stack |

---

## 🎯 CONTEXT LOADERS — Background for Claude

*Load these before working in a specific domain. They're not instructions — they're context.*

| Domain | Loader |
|--------|--------|
| Collin's full identity | Master Identity Context Loader |
| PrimeFold Trading system | PrimeFold Trading Context Loader |
| RENU Property Partners | RENU Context Loader |
| PrimeFold.Tools infrastructure | AI Infrastructure Context Loader |
| Manufacturing background | Manufacturing Operations Context Loader |
| Teaching + frameworks | Teaching & Framework Education Context Loader |
| Leadership patterns | Leadership Pattern Context Loader |
| GPT role work | GPT Role Context Loader |
| Personal timeline + background | Personal Background & Timeline |
| Proof points + credentials | RENU Complete Proof Points |
| Operating philosophy | Proof Before Promises |

---

## 📐 FRAMEWORKS — Thinking Models (Reference, Don't Run)

*Load when making decisions. These shape thinking, not output.*

| Decision | Framework |
|----------|-----------|
| How to price / tier a product | Economy of Plenty |
| How to prevent AI hallucination | Data Sandwich Architecture |
| GPT archetype classification | AI Publishing Stack |
| Trading constraint enforcement | Constraint Protocol v1.3 |
| Symbolic cognition interface | MythOS v1.2 |
| Symbolic-technical bridge | Nerdahl Symbolic-Technical Bridge |
| Risk management philosophy | Risk Management Philosophy |
| Knowledge embodiment (KEF) | KEF Identity Contract v1.0 |
| KEF compression | KEF Compression Protocol v1.0 |
| Deep symbolic/meta systems | Symbolic Cognition & Meta-Systems Framework |
| Content velocity per platform | FORGE Content Velocity Matrix |

---

## Skill Library (Notion-Only) — Not Auto-Loaded

*These are in the Skill Library DB but NOT uploaded as .md files. Claude must fetch them from Notion.*
*Auto-loaded .md skills (forge, sef, vef, tone-tailor, pinescript-architect, etc.) are NOT listed here — Claude already sees those.*

### Trading Stack Recipes

| Task | Skill |
|------|-------|
| Reversal / counter-trend setup | Reversal Stack |
| Breakout / compression break | Breakout Stack |
| Trend continuation | Continuation Stack |
| Scalping (1m-5m, advanced) | Scalp Stack |
| Multi-ticker scanning | Scanner Stack |

### Trading Knowledge Assets

| Asset | Skill |
|-------|-------|
| 6 personality-based blindspot profiles | 6 Trading Blindspot Profiles |
| Per-profile constraint rules | Trading Constraint Library |
| AI + trading psychology integration | Systematic Trading Psychology |
| Safety metadata for trading tools | Tool Safety Metadata Pattern |
| PineScript modular architecture | PineScript Modular Indicator Architecture |
| Make.com + TradingView scanner | Multi-Timeframe Trading Scanner Automation |

### FORGE Sub-Skills (Content System)

| Component | Skill |
|-----------|-------|
| Hook archetypes by intent | FORGE — Hook Library |
| Content decision routing | FORGE — Content Decision Engine |
| Cross-platform adaptation | FORGE — Repurposing Workflows |
| Platform specs (2025 verified) | FORGE — Platform Specifications |
| 5 content intents framework | FORGE — Intent Framework |

### Workspace Meta-Skills

| Task | Skill |
|------|-------|
| Intake + classify new content | CAPTURE |
| Route parsed content to vaults | FILE |
| Parse raw input into structured data | PARSE |
| Maintain + version library entries | LIBRARIAN |
| Reddit reputation management | Reddit Authority Architect |

### Cross-Domain Knowledge

| Domain Transfer | Skill |
|-----------------|-------|
| Pattern transfer across domains | Cross-Domain Pattern Recognition |
| Holding contradictions productively | Asymmetric Integration |
| Context window optimization | Token Economics |
| Lean/Kaizen applied to AI | Paul Akers Lean — Applied Kaizen |
| 5S system for empowerment | 5S Kaizen Empowerment System |
| Teaching frameworks methodology | Teach to Fish |
| Self-directed learning patterns | Self-Directed Learning Methodology |
| Thread mining + Notion org | Thread Archaeology & Notion Organization |
| GPT + Make.com + Claude API integration | Custom GPT + Make.com + Claude API Integration |
| RENU adaptive reuse specialty | RENU Adaptive Reuse Specialization |
| Manufacturing documentation | Manufacturing Documentation System |

---

## 🧠 META / SYSTEM — Workspace & OS Prompts

*Prompts about the system itself.*

| Task | Prompt | Type |
|------|--------|------|
| Notion brain ingestion | Notion Brain Ingestion Engine | Stack |
| Notion superstructure | Notion Superstructure Stack | Stack |
| Context reset + clean restart | Context Reset + Production Prompt Constructor | Stack |
| Skill extraction audit | Skill Extraction & Embodiment Auditor | Stack |
| Claude Skills R&D | Claude Skills R&D Lab | Stack |
| Priority audit + orchestration | Priority Orchestrator | Stack |
| Total system audit | Total System Audit Stack v1.0 | Stack |
| Prompt Compiler reference | Prompt Compiler v3.0 Index | Reference |
| PrimeFold Agent blueprint | Agent Blueprint Template v1.0 | Template |
| Mark DB as superseded | Mark Superseded Database Prompt | Prompt |
| Naming + versioning rules | Naming + Versioning Standard v2.0 | Framework |

---

## 👨‍👩‍👧 FAMILY & LIFESTYLE — Parked Products

*Not revenue-priority. Reference only until after first sale.*

| Tool | Prompt |
|------|--------|
| NOM NOM meal planner | NOM NOM Production Stack |
| StoryScape bedtime stories | Story Engine v1.0 |
| CloserConnection integration | CloserConnection Ecosystem Stack |
| Email Detox inbox system | Email Detox GPT |
| FactGuard verification | FactGuard Pro GPT |
| Soul Signal consciousness | Soul Signal Concept Spec |
| Dream Day GPT | Dream Day Pricing + Monetization |

---

## Not Indexed

**Prompt Vault:** ~40 remaining entries (KEF sub-specs, GPT Role Explorer implementation details, Prompt Compiler internals, NEXUM-era stacks). Findable via Notion search.

**Skill Library:** ~20 remaining entries are mirror copies of auto-loaded .md skills (already ambient) + 2 flagged duplicates pending kill.

---

*Claude: Fetch this page at session start or when you're about to freestyle a task that might have a dedicated prompt. If a prompt exists, use it — it'll produce better output than general knowledge.*
