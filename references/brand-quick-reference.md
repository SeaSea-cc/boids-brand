# Boids Brand — Quick Reference

> Extracted from `workspaces/nevamind/brand/boids-brandbook.md` §1–§4.
> Read this file before every Boids authoring task.

## Positioning

### What Boids Is

**Boids is an AI agent orchestration platform that lets professional users build, run, and publish AI agents into repeatable multi-step workflows.**

Boids is the **L2-1 professional layer** of Nevamind's persistent-AI architecture — sitting on top of MemU (memory) and beneath Antifomo (professional tools).

### Approved Category Labels

| Label | Context |
|---|---|
| **AI Agent Orchestration Platform** | Investor / category leadership / homepage |
| **Professional AI Agent Marketplace** | Partnership / B2B sales / enterprise |
| **Build, run, and publish AI agents** | Product surface / onboarding / first task |
| **Agent skill platform with credit loop** | Technical / investor / competitive positioning |

### What Boids Is NOT

| Never say this | Why |
|---|---|
| "AI chatbot marketplace" | L1a consumer framing |
| "Talk to AI celebrities" | Persona-agent framing (L1a) |
| "Memory infrastructure" | L3 developer framing; MemU owns this layer |
| "One-click AI automation" | Hype language that undercuts the builder narrative |
| "No-code AI tool" | Tool framing; Boids is a platform, not a tool |

### Layer Relationship

```
Nevamind (company)
  └── "Makes AI persistent"

  ├── Antifomo (L1-2 — work efficiency / productivity AI)
  ├── Boids (L2-1 — agent orchestration platform) ← YOU ARE HERE
  └── MemU (L3 — AI memory framework)
```

---

## Brand Personality

| Priority | Archetype | Expression |
| --- | --- | --- |
| Primary | **The Builder** | Mastery-enabling, construction-oriented, tool-forward |
| Secondary | **The Systems Thinker** | Orchestration-aware, process-obsessed, efficiency-driven |

In three words: **Build. Run. Publish.**

---

## Voice & Tone

**Builder's confidence · Professional precision · Systems thinking · Empathetic peer · Measured ambition.**

### Verb Register

| Register | Use | Avoid |
|---|---|---|
| **L2-1 verbs (use)** | build, run, publish, rank, credit, orchestrate | — |
| **L1a verbs (never)** | — | chat, discover, consume, talk, play |

---

## Visual Identity — Builder Ink Palette

### Color Tokens

| Role | Name | Hex | OKLCH | Use |
|---|---|---|---|---|
| Brand Primary | **Ink** | `#0F0F0E` | `oklch(0.16 0.003 60)` | Hero surfaces, primary text on light, brand-mark fill |
| Light Surface | **Bone** | `#F2EDE4` | `oklch(0.94 0.011 80)` | Workspace canvas, content backgrounds, deck pages |
| Single Accent | **Phosphor** | `#C7FF4A` | `oklch(0.94 0.20 122)` | CTAs, active workflow nodes, credit indicators, selection state — ONE accent, always flat |
| Neutral 100 | **Bone-200** | `#E8E2D6` | `oklch(0.89 0.014 80)` | Card surface on Bone, subtle dividers |
| Neutral 400 | **Stone** | `#A8A096` | `oklch(0.69 0.012 80)` | Secondary text, metadata, captions |
| Neutral 700 | **Ash** | `#3A3833` | `oklch(0.32 0.005 70)` | Body text on Bone, hairlines on Ink @ 12% |
| Deep Surface | **Onyx** | `#1A1916` | `oklch(0.20 0.004 70)` | Dark-mode surface, terminal frames |
| Functional Warning | **Ochre** | `#C99B3F` | `oklch(0.71 0.13 76)` | Retry / pending — state color only, never decoration |
| Functional Error | **Terracotta** | `#C24A3A` | `oklch(0.55 0.16 30)` | Build failure — state color only, never decoration |

### Color Hard Rules

- **One accent only.** Phosphor carries every emphasis state.
- **No gradient as a primary surface or background.** Phosphor is flat fill or 1px hairline only.
- **No pure black `#000000`.** Use Ink (`#0F0F0E`) or Onyx (`#1A1916`).
- **No cool gray.** Banned: `#FAFAFA`, `#F5F5F5`, `#E5E5E5`.
- **Tinted shadows only.** `oklch(0.16 0.003 60 / 0.08)` — never `rgba(0,0,0,*)`.
- **Texture mandate.** Every brand surface carries a fixed grain overlay at 3% opacity, `pointer-events:none`.

### Typography — Builder Stack

| Level | Family | Weights | Use |
|---|---|---|---|
| Display | **PP Editorial New** | Ultralight (200), Italic | Hero headlines, brand moments |
| Display alt | **Cabinet Grotesk** | Bold (700), Extrabold (800) | Eyebrow tags, section titles, deck headers |
| Body | **Geist** | Regular (400), Medium (500), Semibold (600) | Product UI, documentation, body copy |
| Mono / Data | **JetBrains Mono** | Regular (400), Medium (500) | Agent logs, skill configs, execution data, credit tables, tabular numbers |

**Banned families (auto-fail):** Inter, Roboto, Arial, Open Sans, Helvetica, SF Pro, Source Sans Pro, Space Grotesk.

**Rules:** Display headlines = `-0.03em` tracking. Eyebrow tags = `+0.2em uppercase 10px`. Title-to-subtitle ratio ≥ 3.0×. Tabular nums on all data. Italic PP Editorial New for single-word emphasis. Never bold for emphasis. Sentence case only. Numbers always in JetBrains Mono or tabular-nums Geist.

### Surface — Double-Bezel

Every card, panel, or major container:

```
Outer Shell:  bg = Bone-200, padding = 6px, ring = 1px Ink @ 5%, radius = 24px
Inner Core:   bg = Bone,     padding = 24px,                     radius = 18px
              + inset highlight: shadow inset 0 1px 1px Bone @ 60%
```

### Layout Archetypes

| Archetype | Use For |
|---|---|
| **Asymmetric Bento** | Marketing pages, product showcases |
| **Editorial Split** | Narrative landing, About, Manifesto |
| **Document Bento** | Docs, agent config, skill marketplace |

**Universal:** Section padding ≥ 32px desktop. Whitespace ≥ 40%. Max content width 1200–1440px. 65ch body max. Sentence case only.

### Slide / Deck Format (1920×1080)

- 5% top-left blank logo zone (never draw the logo in generated images)
- `Privileged&Confidential` watermark: 10px JetBrains Mono, Ink @ 35%, bottom-right
- Whitespace ≥ 40%
- One core insight per page
- Grain overlay at 3% mandatory
- Page number: JetBrains Mono, Stone, top-right

### Iconography

| Tier | System | Use |
|---|---|---|
| Primary | **Phosphor (Light, 1.5px stroke)** | All UI iconography |
| Brand | **Custom Boids glyphs** | Build / Run / Publish / Rank / Credit |
| Banned | Lucide, Feather, FontAwesome, Material Icons | Generic AI default |

All icons use **one stroke weight**: 1.5px.

### Forbidden Visuals

**Never:** Emojis. Cartoon / 3D-glossy AI brains or robots. Stock-photo people. Handshake / coin / rocket / flag / globe metaphors. Centered all-caps body. Saturated brand-color washes. Isolated chat-input screenshots. Overcrowded UI.

**Newly banned:** Pure `#000000` or `#FFFFFF` backgrounds. Linear gradients across full surfaces. Teal-to-blue or purple-to-blue gradients. Glassmorphism on scrolling content. Lucide / Feather / Material default icons. Inter / Roboto / Open Sans / Helvetica / Space Grotesk. Equal-height 3-card feature rows. Cool gray `#FAFAFA`. `box-shadow: 0 4px 6px rgba(0,0,0,0.1)`. Centered hero with ghost-button-pair below H1.

### Logo Direction

- Communicates: orchestration, agent swarm, directional flow, professional confidence
- Wordmark: Cabinet Grotesk Extrabold, `-0.04em` tracking
- Approved on: Ink, Bone, Onyx, Phosphor (accent under Ink wordmark only)
- **Never on**: gradients, pure black, pure white, busy photography
- **In GPT Image 2 prompts**: never draw the logo; reserve 5% top-left blank square
- Tagline: Geist Medium 60% size of wordmark, `+0.05em` tracking, Stone color

---

## Partner Rules

Brand approval: `brand@nevamind.ai` — 5 business days standard.
