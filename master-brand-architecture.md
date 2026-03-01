# PRIMEFOLD — Master Brand Architecture

## Brand Hierarchy

```
PRIMEFOLD (CanonicalSystem)
│
├── PrimeFold.Tools      → Infrastructure / Authority (parent brand)
├── PrimeFold Trading    → Traders, market tools, execution signals
├── PrimeFold Family     → Parents, couples, households
├── PrimeFold Life       → Singles, personal stack, high-agency individuals
└── Collin Nerdahl       → Operator / Proof
```

## Product Vertical Map (Feb 28, 2026)

| Vertical | Avatar | Products |
|----------|--------|----------|
| PrimeFold Trading | Active traders | Drill Coach GPT, Bear Pack, Blindspot Quiz, TradingView indicators |
| PrimeFold Family | Parents, couples, households | PlaySpark, StoryScape, NOM NOM, CloserConnection |
| PrimeFold Life | Singles, self-directed individuals | Dream Day, personal decision tools, solo lifestyle stack |

**Overlap rule:** Products serving both avatars listed in both verticals with different positioning copy. Same product, different angle.

> One system, four expressions. No fragmentation.

---

## Color System

### Core Foundations
| Token | Hex |
|-------|-----|
| PrimaryBackground | #121212 |
| AbsoluteBlack | #000000 |
| PrimaryText | #FFFFFF |
| SecondaryText | #FFFFFF94 |

### Signal / Authority Accents
| Token | Hex |
|-------|-----|
| Signal Gold | #FFD900 |
| Soft Gold | #FFE552 |

### Structural UI Neutrals
| Token | Hex |
|-------|-----|
| Surface Dark | #1E1E1E |
| Divider Dark | #2A2A2A |
| Muted / Disabled | #3A3A3A |

### Cognitive Accent (ONE ONLY)
| Token | Hex |
|-------|-----|
| Cognitive Blue | #7AA2F7 |

## Color Usage Rules

### Backgrounds
- Pages: `#121212`
- Hero / logo-only zones: `#000000`
- Cards & panels: `#1E1E1E`

### Text
- Primary: `#FFFFFF`
- Secondary / explanatory: `#FFFFFF94`
- Muted / disabled: `#3A3A3A`

### Accents
- **Gold** → authority, CTAs, key emphasis
- **Blue** → cognition, links, charts, verification

### Hard NOs
- No gradients by default
- No green, purple, or bright blue
- No playful or expressive colors

---

## Typography

### Primary Typeface (LOCKED): Inter
- Body, UI, Headings, Docs, PDFs, Stripe, Notion

| Weight | Usage |
|--------|-------|
| 400 | Body |
| 500 | Labels |
| 600 | Section headers |
| 700 | Emphasis (rare) |

### Secondary Typeface: IBM Plex Mono
- Code, Metrics, Signals, Logs, System outputs

---

## Brand Feel
Reads as: Bloomberg terminal, Aerospace / capital infrastructure, Durable, sober, precise.
Used everywhere: Website, Products, Stripe, Canva, PDFs, Gumroad.
**This palette never rotates.**

---

## Logo Asset Inventory

### PrimeFold.Tools Assets

**Asset 1 — Full Lockup (landscape):** Emblem + wordmark + circuit atmosphere + blue glow
- USE FOR: Profile header, hero/banner backgrounds, brand announcement contexts

**Asset 2 — Emblem Only on Black (1:1 square):** Sigil + gold inner ring + blue outer ring on #000000
- USE FOR: Profile avatar, thumbnail badge, square branding zones
- THIS IS: The primary recognition mark

**Asset 3 — Wordmark Only (landscape):** Wordmark + gold divider rule, no emblem
- USE FOR: Cover images where product visuals take center

**Asset 4 — Raw Trace / Sigil (1:1, transparent-ready):** Base mark, no color, no ring
- USE FOR: PDF watermarks, document headers, low-profile brand stamps

### Logo Usage Rules
- **Thumbnail (600×600):** Asset 2 as badge/corner mark — bottom-right, ~15% of frame
- **Cover (1280×720):** Asset 3 bottom-left — or Asset 1 if no product visual present
- **PDFs / Docs:** Asset 4 as watermark or header stamp
- **Profile Header:** Asset 1
- Never invert logos to light backgrounds

### PrimeFold Trading Sub-Brand

**Asset T1 — Trading Emblem (1:1):** Geometric bull/bison + crossed swords + sacred geometry. Signal Gold on black.
**Asset T2 — Trading Full Lockup (portrait):** Emblem + gold serif wordmark on dark texture.

- Trading assets for trading products only
- Never mix Trading + Tools logos in same asset

---

## Brand Separation Rule

> RENU Property Partners is a separate operating entity. RENU assets, colors, and typography NEVER appear in PrimeFold materials. PrimeFold assets NEVER appear in RENU materials.

---

## Asset Folder Structure

```
PrimeFold_Brand_v1/
├── Logos/
│   ├── PrimeFold_Primary_Dark.png
│   ├── PrimeFold_Flat_White.png
│   ├── PrimeFold_Gold.png
│   ├── PrimeFold_Blue.png
│   ├── PrimeFold_Light_BG.png
│   ├── PrimeFold_Icon_Favicon.png
│   └── PrimeFold_Master_Vector.svg
├── Social/
│   ├── Profile_Icon_1x1.png
│   ├── Banner_16x9.png
├── Canva_Templates/
│   ├── PDF_Cover_Template
│   ├── PDF_Interior_Template
│   ├── Lead_Magnet_Template
│   ├── Case_Study_Template
│   ├── Trading_Report_Template
└── Brand_Guide.pdf
```
