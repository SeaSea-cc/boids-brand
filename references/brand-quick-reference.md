# Boids Brand — Quick Reference (v1.2)

> **Brandbook version:** v1.2 — confirmed by Nevamind / Boids founder Chen Hong.
> **Source of truth:** [`brandbook.md`](./brandbook.md). When this file conflicts with the brandbook, the brandbook wins.
> Read this file before every Boids authoring task.

---

## Brand at a Glance

| | |
|---|---|
| **In three words** | Build. Distribute. Work. |
| **Universal hero** | Build expert agents. Bring them everywhere. |
| **C-end product hero** | Bring expert agents to work with you. |
| **API / CLI hero** | Build products with agents. Ship through API and CLI. |
| **Support line** | Build what you know. Deploy what you trust. Boids runs the loop. |
| **Canonical sentence** | Boids is made for A2A: expert agents that can be called, composed, and distributed across human and agent workflows. |

---

## Positioning (v1.2)

### What Boids Is

**Boids is the Expert Agent Platform** for building, distributing, and working with AI agents. It ships as **two distinct products** on the same shared agent network.

#### Two product lines

| Product | Audience | Positioning line |
|---|---|---|
| **Boids Product** | Regular users (C-end) | *Bring expert agents to work with you.* — consumer app + Slack / Telegram / IM integrations |
| **Boids API / CLI** | Developers | *Build products with agents. Ship through API and CLI.* — developer infrastructure + A2A network |

Every Boids agent is **callable, composable, distributable, verifiable, and work-native**. What is published by one product is callable by the other.

### Approved Category Labels

| Label | Context |
|---|---|
| **Expert Agent Platform** | Homepage / brand-level positioning |
| **Agent Build & Distribution Platform** | Product / investor / category leadership |
| **Professional AI Agent Network** | Partnership / B2B / ecosystem |
| **A2A-native Agent Platform** | Technical / protocol-facing |
| **Bring expert agents to work with you** | C-end product / user-facing |
| **Build products with agents, ship through API and CLI** | Developer / API-facing |
| **Agent skill platform with credit loop** | Technical / investor / competitive |

### What Boids Is NOT

| Never say this | Why |
|---|---|
| "AI chatbot marketplace" | Too consumer, too passive |
| "Talk to AI celebrities" | Persona-agent framing, not professional work |
| "No-code AI tool" | Tool framing; Boids is a platform |
| "Developer API marketplace" | Too narrow; ignores the consumer product |
| "AI app store" | Too static; agents on Boids are built, distributed, called, composed, and used |

### Nevamind Product Map

```
Nevamind
  └── Builds professional AI products
  └── Boids
      ├── Boids Product (C-end, regular users)
      └── Boids API / CLI (developers)
```

---

## Brand Personality

| Priority | Archetype | Expression |
|---|---|---|
| Primary | **The Builder** | Mastery-enabling, construction-oriented, distribution-forward |
| Secondary | **The Systems Thinker** | Orchestration-aware, composability-obsessed, work-native |

In three words: **Build. Distribute. Work.**

---

## Voice & Tone

**Builder's confidence · Professional precision · Systems thinking · Empathetic peer · Measured ambition.**

Boids speaks like someone who has already shipped the system — not someone trying to sell you on building it.

### Verb Register

| Register | Use | Avoid |
|---|---|---|
| **Boids verbs (use)** | build, distribute, publish, call, compose, deploy, ship, earn, compound, bring, integrate, run | — |
| **Banned verbs (never)** | — | chat, discover, consume, talk, play, explore, connect |

### Forbidden Phrasings

- "AI chatbot" / "chat with AI"
- "No-code"
- "Talk to your AI"
- "AI-powered" (vague, avoid)
- "Cutting-edge" / "state-of-the-art" / "revolutionary"
- Any framing that reduces Boids to a single use case or consumer product

---

## Visual Identity — "Precision Mono + Ambient Glow"

A strict black-and-white base with a three-color **ambient glow** as the decorative layer. Black and white carry the structure; the glow carries the energy. The decorative layer is **never a stripe gradient** — it is a radial, atmospheric wash. In dark mode: vibrant glows on deep black. In light mode: soft pastel washes on white. Both use the same color family.

### Base Palette

| Role | Name | Hex | Use |
|---|---|---|---|
| Brand Primary | **Black** | `#0D0D0D` | Hero surfaces, primary text, brand-mark fill |
| Light Surface | **White** | `#FFFFFF` | Workspace canvas, content backgrounds |
| Neutral 50 | **Gray-50** | `#F7F7F7` | Card surfaces on White |
| Neutral 400 | **Gray-400** | `#9E9E9E` | Secondary text, metadata, captions |
| Neutral 700 | **Gray-700** | `#3D3D3D` | Body text, hairlines |
| Deep Surface | **Onyx** | `#1A1916` | Dark-mode surface, terminal frames |
| Functional Warning | **Ochre** | `#C99B3F` | Retry / pending — never decorative |
| Functional Error | **Terracotta** | `#C24A3A` | Build failure — never decorative |

### Ambient Glow — Three-Color System

Three colors used **only** as radial ambient glows — never as stripe gradients, never as full background fills.

```
#06B6D4   Cyan / Deep Blue    — cool, technical, active
#8B5CF6   Purple / Violet     — depth, intelligence, brand
#EC4899   Pink / Rose         — warmth, energy, human
```

**Glow usage rules:**

| Context | Usage |
|---|---|
| CTA button border | 1–2px glow gradient stroke, Black fill inside |
| Active agent nodes / selected state | Glow via `box-shadow` |
| Brand moments (cover, hero) | Radial glow as background light source |
| Icon accent | Glow color stroke, 1.5px weight |
| Credit indicators / agent distribution state | Glow pulse animation |

**Hard rules:**
- Never fill large background surfaces with glow colors directly.
- Glow is always **radial, diffused, atmospheric** — never a sharp stripe or flat fill.
- On dark (Black / Onyx): full saturation. On White: desaturated, pastel tint.
- All three colors must coexist on a surface — **no single-color pulls**.

### Color Hard Rules

- **No cool gray.** Banned: `#FAFAFA`, `#F5F5F5`, `#E5E5E5`.
- **Tinted shadows only.** Black at 8% opacity, never `rgba(0,0,0,*)`.
- **Texture mandate.** Every brand surface carries a fixed grain overlay at 3% opacity, `pointer-events: none`.

### Typography — Builder Stack

| Level | Family | Weights | Use |
|---|---|---|---|
| Display | **PP Editorial New** | Ultralight (200), Italic | Hero headlines, brand moments |
| Display alt | **Cabinet Grotesk** | Bold (700), Extrabold (800) | Eyebrow tags, section titles, deck headers |
| Body | **Geist** | Regular (400), Medium (500), Semibold (600) | Product UI, documentation, body copy |
| Mono / Data | **JetBrains Mono** | Regular (400), Medium (500) | Agent logs, API configs, credit tables, tabular numbers |

**Banned families (auto-fail):** Inter, Roboto, Arial, Open Sans, Helvetica, SF Pro, Source Sans Pro, Space Grotesk.

**Rules:** Display headlines = `-0.03em` tracking. Eyebrow tags = `+0.2em uppercase 10px`. Title-to-subtitle ratio ≥ 3.0×. Tabular nums on all data. Italic PP Editorial New for single-word emphasis. Never bold for emphasis. Sentence case only. Numbers always in JetBrains Mono or tabular-nums Geist.

### Surface — Double-Bezel

Every card, panel, or major container uses nested-enclosure construction:

```
Outer Shell:  bg = Gray-50,  padding = 6px,  ring = 1px Black @ 5%,  radius = 24px
Inner Core:   bg = White,    padding = 24px,                          radius = 18px
              + inset highlight: shadow inset 0 1px 1px White @ 60%
```

**Primary CTA button:** pill (rounded-full), padding 12px 24px, fill = Black, text = White, **glow border** (1.5px gradient stroke). Trailing arrow ↗ inside its own 32×32 circle (glow @ 12%).

```
[ Build your first expert agent   ( ↗ ) ]
```

**Eyebrow tag:** Cabinet Grotesk 10px, +0.2em uppercase, bg: glow @ 10%, text: Black.

```
〔 EXPERT AGENT PLATFORM 〕
Build expert agents. Bring them everywhere.
```

### Texture & Shadow

| Element | Spec |
|---|---|
| Grain overlay | Fixed, `inset: 0`, `pointer-events: none`, `opacity: 0.03` |
| Card shadow | `0 1px 2px Black/0.04, 0 8px 24px Black/0.06` |
| Hover lift | `translateY(-2px)` + shadow → Black/0.10, `cubic-bezier(0.32, 0.72, 0, 1)` 400ms |
| Banned | `shadow-md`, `rgba(0,0,0,0.3)`, glassmorphism on scrolling content |

### Layout Archetypes

| Archetype | Use For |
|---|---|
| **Asymmetric Bento** | Marketing pages, product showcases — CSS Grid, varied col-span. Never 3-equal-card row. |
| **Editorial Split** | Narrative landing, About, Manifesto — `w-1/2` Editorial New left + scrollable interactive right. |
| **Document Bento** | Docs, API reference, agent configs — max-width 1200px, asymmetric grid, 65-char body |

**Universal:** Section padding `py-32` desktop / `py-16` mobile minimum. Whitespace ≥ 40%. Max content width 1200–1440px. Body ≤ 65ch. `min-height: 100dvh` for full-screen sections. Mobile (<768px): single column, `w-full`, `px-4`. Sentence case only.

### Slide / Deck Format (1920×1080)

- 5% top-left blank logo zone (never draw the logo in generated images)
- `Privileged&Confidential` watermark: 10px JetBrains Mono, Black @ 35%, bottom-right (optional — internal / NDA decks only)
- Whitespace ≥ 40%
- One core insight per page; never two H1s
- Footer source citation on data slides: 9px JetBrains Mono, Gray-400, left-aligned
- Grain overlay at 3% mandatory on every slide
- Page number: JetBrains Mono, Gray-400, top-right, every slide except cover
- **Glow rule:** radial ambient light source only — never stripe wash across slide

### Iconography

| Tier | System | Use |
|---|---|---|
| Primary | **Phosphor Icons (Light, 1.5px stroke)** | All UI iconography |
| Brand | **Custom Boids glyphs** | Build / Distribute / Call / Compose / Credit |
| Banned | Lucide, Feather, FontAwesome, Material Icons | Generic AI default |

One stroke weight: **1.5px** across all surfaces.

### Forbidden Visuals

**Always banned:**
- Emojis in brand contexts
- Cartoon / 3D-glossy "AI brains" or robots
- Stock-photo people
- Handshake / coin / rocket / flag / globe metaphors
- Centered all-caps body text
- Isolated chat-input screenshots
- Equal-height 3-card feature rows

**Color / surface bans:**
- Glow colors as full background fills
- Teal-to-blue or purple-to-blue stripe gradients
- Glassmorphism on scrolling content
- Cool grays (`#FAFAFA`, `#F5F5F5`, `#E5E5E5`)
- Generic `box-shadow: rgba(0,0,0,0.1)`
- Centered hero with ghost-button-pair below H1

### Logo Direction

- Communicates: agent network, distribution flow, professional confidence
- Wordmark: Cabinet Grotesk Extrabold, `-0.04em` tracking
- Approved on: Black, White, Onyx — with ambient glow as background accent only
- **Never on**: gradient fills, busy photography, low-contrast surfaces
- **In GPT Image 2 prompts**: never draw the logo; reserve 5% top-left blank square
- Tagline: Geist Medium 60% size of wordmark, `+0.05em` tracking, Gray-400

---

## Authoring Checklist

Before publishing any Boids copy:
- [ ] Is it clear which product line this is for? (C-end product, API / CLI, or universal / brand-level)
- [ ] Does it use the right verbs? (build / ship / distribute / call / compose / integrate / earn)
- [ ] Does it avoid consumer chat framing? (no "chat", "talk", "discover")
- [ ] Does it treat agents as callable, composable, distributable?
- [ ] Is it sentence case? No Title Case headers.
- [ ] Does it avoid "AI-powered", "cutting-edge", "revolutionary"?

---

## Partner & Brand Approval

For uses outside the Permitted Uses defined in `TRADEMARKS.md`, request brand approval:

**Contact:** `brand@nevamind.ai` — 5 business days standard.

See [`TRADEMARKS.md`](../TRADEMARKS.md) for the full trademark usage policy.
