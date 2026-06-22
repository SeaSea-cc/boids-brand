---
name: boids-brand
description: Apply the canonical Boids brand system v1.2 (positioning as the Expert Agent Platform with two product lines — Boids Product for regular users and Boids API / CLI for developers; Precision Mono + Ambient Glow visual identity; voice; messaging; and GPT Image 2 prompt preamble) when authoring or revising any Boids-branded artifact — pitch decks, product pages, sales collateral, GPT Image 2 prompts, brandbook output, client deliverables, or co-branded materials. Use whenever the user says "write/draft/refresh Boids copy", "build a Boids deck/page/social post", "generate Boids brand images", "apply the Boids brandbook", "apply Boids positioning", or any task that must comply with the Boids brand system. Boids is the expert agent platform by Nevamind — its visual register is Precision Mono + Ambient Glow: a strict black-and-white base with a three-color radial glow (cyan / violet / rose), never the AI-startup teal-blue cliché. Companion to `seasea-brand` (master-brand surfaces).
---

# Boids Brand — v1.2

> **Brandbook version:** v1.2 (confirmed by Nevamind / Boids founder Chen Hong — `brandbook.md`)
> **Skill version tag:** `release/2026-05-21-v1.2-expert-agent-platform`
> **Canonical source:** [`references/brandbook.md`](./references/brandbook.md)

Author and revise Boids-branded artifacts with the canonical v1.2 brand system applied — positioning, personality, voice, Precision Mono + Ambient Glow visual identity, messaging, and GPT Image 2 preamble — so every output is consistent, on-message, and ready for external audiences.

## Strategic Frame (v1.2)

**Boids is the Expert Agent Platform** for building, distributing, and working with AI agents. It ships as **two distinct products** on a single shared agent network:

| Product | Audience | Positioning |
|---|---|---|
| **Boids Product** | Regular users (C-end) | *Bring expert agents to work with you.* — the consumer app and integrations into Slack, Telegram, and the IM tools where work already happens |
| **Boids API / CLI** | Developers | *Build products with agents. Ship through API and CLI.* — developer infrastructure for building, distributing, and composing expert agents into other products via A2A |

Both products share the same network: every agent is **callable, composable, distributable, verifiable, and work-native**. What is published by one is callable by the other.

The brand must communicate **builder confidence, professional precision, systems thinking, empathetic peer, and measured ambition** — never hype, never magic framing, never consumer-chat playfulness.

**Canonical sentence:** *Boids is made for A2A: expert agents that can be called, composed, and distributed across human and agent workflows.*

## When to Use

- User asks to write, draft, refresh, or revise any Boids-branded copy (deck, pitch, page, social, ad)
- User asks to build any sales-conversion artifact: pitch deck, one-pager / solution brief, customer case study, RFP / procurement / trust pack, investor update, or board deck
- User asks to produce marketing & demand-gen artifacts: single image, performance / paid-social ad, OOH / billboard, long-form social or thread, email (transactional or nurture), press release / media kit, podcast or video-episode lockup, conference / event booth
- User asks to author web, product, or developer surfaces: web / landing page, documentation site, API reference, in-product UI, status page, trust center, app-store listing, GitHub org profile, OSS README, changelog / release notes, or CLI / terminal output
- User asks to write a voiceover, careers page, recruiting deck, incident / postmortem, security advisory, partner / co-marketing lockup, or swag / merch system
- User asks to generate brand visuals (GPT Image 2) for Boids
- User asks to apply the Boids brandbook (v1.2) to an existing draft
- User mentions Boids positioning, category labels, builder voice, Precision Mono + Ambient Glow visual identity, or one of the two product lines
- A new Boids artifact is being scaffolded that must comply with the Boids brand system

## Canonical Source Files

This skill is self-contained. All canonical brand rules live in this repository — never override them:

| Source | Path | Role |
|---|---|---|
| **Brandbook v1.2** | `references/brandbook.md` | Master document — full v1.2 brand system specification (confirmed by Nevamind / Boids founder Chen Hong) |
| Brand quick reference | `references/brand-quick-reference.md` | Derived quick-lookup cheat sheet |
| GPT Image 2 preamble | `references/gpt-image2-preamble.md` | Derived prompt rules |
| Messaging library | `references/messaging-library.md` | Derived messaging extracts |
| Application playbooks | `references/application-playbooks.md` | Derived scenario playbooks |
| Visual exemplars | `references/exemplars/` | Curated v1.2 visual exemplars (≤ 12 positive + ≤ 6 negative). Reference set only — NOT a gallery of outputs. See `references/exemplars/README.md` for curation rules. |

**Order of authority:** `references/brandbook.md` (v1.2) > other `references/*` files > derived artifacts. When any reference file conflicts with the brandbook, the brandbook wins. The skill repository at `github.com/SeaSea-cc/boids-brand` is the single source of truth.

## Skill Reference Files

Read the relevant reference file before every authoring task:

| File | When to Read |
|---|---|
| `references/brandbook.md` | When resolving conflicts, auditing brand compliance, or performing full-system reviews — the master v1.2 specification |
| `references/brand-quick-reference.md` | Every Boids authoring task — positioning labels, two product lines, personality, voice, color tokens, typography, forbidden visuals |
| `references/gpt-image2-preamble.md` | Any task that produces GPT Image 2 prompts for Boids decks/pages |
| `references/messaging-library.md` | Writing hero copy, headlines, audience messages, narrative arc, taglines |
| `references/application-playbooks.md` | Scenario-specific application: pitch deck, single image, social, voiceover, web |

## Authoring Workflow

Follow this loop for any Boids authoring task:

### 1. Identify the product line first

Every Boids artifact must declare which product line it serves:

- **Boids Product (C-end, regular users)** — copy uses verbs *bring, integrate, call, work with*; channels are Slack/Telegram/the Boids app; ICP is the non-technical professional who wants expert agents in their existing workflow.
- **Boids API / CLI (developers)** — copy uses verbs *build, ship, distribute, compose, integrate*; channels are docs, API reference, CLI, GitHub; ICP is the developer building agent-powered products on top of the Boids network.
- **Brand-level (universal / both)** — uses the master hero "Build expert agents. Bring them everywhere." and the canonical A2A sentence.

### 2. Identify the application scenario

Match the request to one of the **26 playbooks** in `references/application-playbooks.md`. The skill covers the full GTM brand surface organised into 7 categories:

| Category | Playbooks |
|---|---|
| **A. Sales & Conversion** | Pitch deck · One-pager / solution brief · Customer case study · RFP / procurement / trust pack · Investor update / board deck |
| **B. Marketing & Demand Gen** | Single marketing image · Performance ad / paid social · OOH / billboard · Long-form social / thread · Email system · Press release / media kit · Podcast / video lockup · Conference / event booth |
| **C. Web, Product & Developer** | Web / landing page · Documentation & API reference · In-product UI · Status & trust center · App-store listing · GitHub org / OSS README · Changelog / release notes · CLI / terminal output |
| **D. Video & Voice** | Voiceover / narration script |
| **E. Talent & Culture** | Careers page & recruiting deck |
| **F. Governance & Crisis** | Incident / postmortem / security advisory |
| **G. Community & Ecosystem** | Co-marketing / partner lockup · Swag / merch system |

Start with the application surface matrix at the top of `references/application-playbooks.md`, then read the matching playbook section before authoring.

### 3. Apply the brand layer in this order

1. **Positioning** — confirm the category label is one of the approved set in `references/brand-quick-reference.md`. Forbidden: "AI chatbot marketplace", "Talk to AI celebrities", "No-code AI tool", "Developer API marketplace", "AI app store".
2. **Verb discipline** — use Boids verbs: *build, distribute, publish, call, compose, deploy, ship, earn, compound, bring, integrate, run.* Avoid: *chat, discover, consume, talk, play, explore, connect.*
3. **Hero line** — open with the canonical hero line from `references/messaging-library.md`. Universal: *Build expert agents. Bring them everywhere.* C-end: *Bring expert agents to work with you.* API / CLI: *Build products with agents. Ship through API and CLI.*
4. **Voice & tone** — Builder confidence, professional precision, systems thinking, empathetic peer, measured ambition. Boids speaks like someone who has already shipped the system.
5. **Visual identity (v1.2)** — Precision Mono + Ambient Glow: Black `#0D0D0D` + White `#FFFFFF` base, three-color radial ambient glow (`#06B6D4` cyan / `#8B5CF6` violet / `#EC4899` rose), Builder Stack typography (PP Editorial New + Cabinet Grotesk + Geist + JetBrains Mono), Double-Bezel surface system with Gray-50 outer / White inner.
6. **Layout & governance** — 1920×1080 16:9 for decks, 5% top-left blank logo zone, page number top-right. `Privileged&Confidential` watermark only when the deliverable's distribution context requires it (internal / NDA / investor decks); omit for public, OSS, or developer-facing surfaces.

### 4. Pre-flight Self-check

Before delivering output:

- [ ] Product line is declared: C-end product, API / CLI, or brand-level / universal
- [ ] No forbidden positioning labels ("AI chatbot marketplace", "Talk to AI celebrities", "no-code tool", "AI app store")
- [ ] Verbs are Boids verbs only (build · distribute · publish · call · compose · deploy · ship · earn · compound · bring · integrate · run)
- [ ] No avoided verbs (chat · discover · consume · talk · play · explore · connect)
- [ ] Hero line drawn from canonical v1.2 set (universal / C-end / API / CLI)
- [ ] Precision Mono base applied: Black `#0D0D0D` and White `#FFFFFF` carry the structure
- [ ] Ambient glow uses all three colors (`#06B6D4`, `#8B5CF6`, `#EC4899`) — radial, atmospheric, never stripe gradient, never single-color pull
- [ ] On dark surfaces: vibrant saturated glow. On white: desaturated pastel wash.
- [ ] No banned fonts (Inter, Roboto, Arial, Open Sans, Helvetica, SF Pro, Source Sans Pro, Space Grotesk)
- [ ] All numerics in JetBrains Mono with tabular-nums
- [ ] Double-Bezel card construction on all containers (24px outer / 18px inner concentric radii)
- [ ] 3% film-grain overlay on all brand surfaces (`pointer-events: none`)
- [ ] Tinted shadows only — Black at 8% opacity, never `rgba(0,0,0,*)`
- [ ] Sentence case only; no Title Case headers; no "AI-powered", "cutting-edge", "revolutionary"
- [ ] All GPT Image 2 prompts include canonical preamble from `references/gpt-image2-preamble.md`
- [ ] Slide decks: 5% top-left blank zone, page number top-right; confidentiality watermark only if required

## Companion Skills

These are optional companion skills that pair well with `boids-brand` when available in your environment:

| Skill | Use For |
|---|---|
| `high-end-visual-design` | Underlying anti-default UI rules — Boids adopts them as baseline |
| Markdown deck renderer | Render a markdown deck → 16:9 PNG slides |
| Video composition skill | Convert narration + visuals → final video |
| Image-generation skill | Image generation; chain with this skill for brand-correct prompts |

## Output Conventions

- Default language: English (canonical). Use Chinese only when audience is SOE / Chinese-domestic.
- Footer citation on deliverables: `Source: Boids Brand Skill v1.2 — [YYYY-MM-DD git-sha]`.
- Confidentiality watermarks (e.g. `Privileged&Confidential`) are **optional** and depend on the deliverable's distribution context — apply only when the brand owner or the producing organization requires it. External / public Boids assets typically should NOT carry an internal-confidentiality watermark.
- File path conventions are owned by the consuming organization. Recommended: decks under `<workspace>/decks/<deck-name>/`; rendered images under `<workspace>/brand-outputs/<artifact>/`.

## Versioning

This skill is **Git-versioned**. Filenames carry no version number, but the brandbook content itself is now at **v1.2** (see `references/brandbook.md` — confirmed by Nevamind / Boids founder Chen Hong). Significant brand-system releases are marked with annotated tags following the pattern `release/YYYY-MM-DD-<slug>`. See [`CHANGELOG.md`](./CHANGELOG.md) for the full guide.

```bash
git log --oneline                                       # Full history
git log --oneline --follow SKILL.md                     # SKILL.md history
git tag -l "release/*"                                  # All releases
git show release/2026-05-21-v1.2-expert-agent-platform  # v1.2 release notes
```

## License & Trademarks

Skill content is licensed under the [Apache License 2.0](./LICENSE). The Boids name, logo, and visual identity are trademarks of Nevamind — see [`TRADEMARKS.md`](./TRADEMARKS.md). For external use of brand assets: `brand@nevamind.ai` (5 business days standard).

---

**Brand operating motto (v1.2)** — *Build. Distribute. Work.*
