# Workspace Architecture Map — PrimeFold OS

*Complete inventory, canonical structure, and cleanup directives.*
*Maintained by: PrimeFold Scribe | Last audit: 2026-02-21 (Pass 11 — deep clean + canonical DB alignment)*
*Load this before any restructuring session.*

---

## How to Read This Map

Every page in the workspace belongs to one of 5 tiers:

- **ACTIVE** — In COLLIN OPS, Claude-loadable, current
- **DOMAIN** — Under a domain hub, operational but not daily
- **ARCHIVE** — Preserved reference, no active editing
- **DUPLICATE** — Redundant copy, safe to delete after review
- **HOMELESS** — Exists but not properly nested, needs a move

Status tags: `✅ DONE` | `⏳ PENDING MOVE` | `🗑️ MARK FOR DELETION` | `🔗 NEEDS LINK`

### Agent-Touch Convention (established 2026-02-20)

**Purpose:** Track which pages have been created or modified by a Claude agent vs. human-only.

**Markers:**
- `🤖` prefix in title = page was **created** by agent
- `🤖 Agent-touched: [YYYY-MM-DD] | [action]` footer callout = page was **edited** by agent
- `📋 [COPY]` prefix = confirmed duplicate, archived for reference
- `📋 [SUPERSEDED]` prefix = replaced by newer canonical version

**Date stamps:** All agent edits include the date of change. All archive moves include date + reason.

**Rule:** Agent never deletes — only archives with clear labeling. Operator deletes.

---

## Tier 1: Active — COLLIN OPS Core

*These pages are the live operating system. Claude loads these.*

### Control Pages

| Page | Status |
|------|--------|
| COLLIN OPS Master Hub | ✅ Canonical |
| Production Work Order | ✅ Canonical |
| Active Products — Ship Ready | ✅ Canonical |

### Databases (all Claude-searchable)

| Database | Count |
|----------|-------|
| Product Hub | 14 products (3 Live, 1 Ship-Ready, 3 Build, 4 Research, 3 Parked) |
| Thread Harvest | 57 entries |
| Strip Mine Queue | 5 entries (4 complete + 1 batch) |
| GPT Registry | 29 agents ✅ PrimeFold branded |
| Prompt Vault | 124+ entries (canonical asset store) |
| [SUPERSEDED] Projects DB | → Merged into Master Project Registry |
| Evolution Log | 15+ entries |
| Agent Inbox | 0 items pending (10 archived Feb 21) |
| Master Project Registry | active |

### Agent Tools (all Claude-loadable)

| Tool | Vault Entry |
|------|-------------|
| Session Starter | ✅ |
| Gumroad Ship Prompt | ✅ |
| Reddit Post Generator | ✅ |
| Self-Eval Protocol | ✅ |
| Trading Journal Review | ✅ |
| Weekly Review | ✅ |
| GPT Standard Template | ✅ |
| OS Context Block | ✅ |
| Notion Workspace Loader | ✅ |
| Weekly Review (Vault) | ✅ |

### Memory Files (Claude reference — do not delete)

| File | Notes |
|------|-------|
| ChatGPT Core Memory v3.1 | Harvested ✅ Thread #18 |
| Collin Core Memory v3 | ✅ Thread Harvest entry #19 |
| Condensed Profile v1 | ✅ Thread Harvest entry #20 |
| System Architecture v2.2 | ✅ Thread Harvest entry #21 |
| Unified Synthesis v2.0 | ✅ Thread Harvest entry #22 (flagged 🔁 Needs Revisit) |
| Prompt Signature | ✅ Thread Harvest entry #23 |

---

## Tier 2: Domain Hubs

*All 5 domains clean and organized as of 2026-02-21.*

| Domain | Hub | Status |
|--------|-----|--------|
| Trading | Trading Hub | ✅ 8 sections, duplicate removed, URLs fixed |
| RENU | RENU Hub | ✅ 13 pages nested, CRM + Maintenance active |
| Family | Family Tools Hub | ✅ 3 tools + trip + product map |
| Content | Brand Hub → Content/Marketing | ✅ RAA v1.6 nested |
| Brand | Brand Hub | ✅ Brand architecture + memory files |

---

## Tier 3: Framework & Nexum Archive

*All framework pages have Notion Source URLs in Prompt Vault. All Nexum-branded pages archived.*

**Framework Archive:** All canonical frameworks (Agent Brain Standards, KEF Primitive Atlas, Pipeline Operator Guide, GERTHUMS Protocol v2.3) are in Prompt Vault with source URLs. ✅ 100% cross-linked.

**Nexum Archive:** NEXUM ARCHIVE — Preserved Reference Era 2024–2025. 18+ pages archived (Pass 6–7). Zero stragglers. Read-only reference.

**Legacy PARA containers** (3. RESOURCES, 4. ARCHIVES) marked with warning banners. Read-only.

---

## Completed Tiers (Historical Reference)

**Delete Candidates:** All 4 confirmed duplicates archived to Nexum Archive (Pass 7). Zero remaining.

**Machine Readability:** All Prompt Vault source URLs populated (100%). Memory files in Thread Harvest. Product pages in Project Registry. Family Hub created and populated.

---

## Execution Order

*All 12 items complete as of 2026-02-21. No pending moves.*

✅ Family Hub created • RENU docs linked • Trading pages archived • Nexum pages archived • Duplicates resolved • Source URLs added • Memory docs harvested • RAA homed • OS Context Block updated • COLLIN OPS link fixed • 1. PROJECTS cleaned

---

## Workspace Health Metrics

*Snapshot as of 2026-02-21 Pass 11. All metrics current.*

| Metric | Count | Target |
|--------|-------|--------|
| Total databases (Claude-queryable) | 10 (9 canonical + 1 superseded) | 10 ✅ |
| Prompt Vault entries | 124+ ✅ | 50+ |
| Thread Harvest entries | 57 ✅ | 50+ |
| GPT Registry entries | 29 ✅ PrimeFold | All current GPTs |
| Projects with descriptions | 18/20+ ✅ | All ACTIVE |
| Homeless pages (estimated) | 0 ✅ | 0 |
| NEXUM-branded pages needing archive | 0 ✅ (18 archived) | 0 |
| Confirmed duplicates | 0 ✅ (4 archived) | 0 |
| Superseded DBs migrated | 5/5 ✅ | All |
| Framework pages with Notion Source URL in Vault | 100% ✅ | 100% |

---

*This map is the source of truth. Update it as pages move. Claude uses this to navigate the workspace.*
*Next full audit: after first revenue or 90 days, whichever comes first.*

---

### Natural Selection Log — 11 Passes completed (Feb 19–21)

- **Pass 1** (Feb 19): RAA → Brand Hub, COLLIN OPS link fix, 5 memory files → Thread Harvest.
- **Pass 2** (Feb 19): Strip Mine infrastructure (Queue DB + Protocol SOP).
- **Pass 3** (Feb 19): Gap analysis — Thread Harvest 23 → 42 entries.
- **Pass 4** (Feb 19): PROJECT STATUS rebuilt. Vault count synced.
- **Pass 5** (Feb 20): Overnight harvest — Thread Harvest 42 → 56.
- **Pass 6** (Feb 20): STACK uploaded. 43 pages moved (Nexum, GERTHUMS, RENU, legacy).
- **Pass 7** (Feb 20): GPT Registry 100% branded. Vault URLs added. 4 duplicates archived.
- **Pass 8** (Feb 20): Final organizer sweep. OS Context Block updated. All items clear.
- **Pass 8b** (Feb 20): Strip Mine Queue 4/4 processed. 2 Vault extractions.
- **Pass 9** (Feb 21): Feb 22 Work Orders — 9/9 tasks. 18 project pages. 4 Vault migrations.
- **Pass 10** (Feb 21): Condensation pass. ONDOUSD/AMPUSD URL fix. Domain hub audit. Architecture Map compressed.
- **Pass 11** (Feb 21): Deep clean. Product Hub canonicalized as 10th DB in BRAIN. Projects DB superseded. Agent Inbox schema fixed + processed to zero. Intelligence Hub diagram repaired. COLLIN OPS completed with all 10 DB links + Intelligence Hub.
