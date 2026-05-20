---
name: boids-brand
description: Apply the canonical Boids brand system (positioning as the L2-1 AI agent orchestration platform for professional builders, Builder Ink visual identity, voice, messaging, and GPT Image 2 prompt preamble) when authoring or revising any Boids-branded artifact — pitch decks, product pages, sales collateral, GPT Image 2 prompts, brandbook output, client deliverables, or co-branded materials. Use whenever the user says "write/draft/refresh Boids copy", "build a Boids deck/page/social post", "generate Boids brand images", "apply the Boids brandbook", "apply Boids positioning", or any task that must comply with the Boids brand system. Boids is the AI agent orchestration platform by Nevamind-AI — its visual register is Linear/Vercel-adjacent: Dark Developer / Builder with Editorial Luxury restraint, never the AI-startup teal-blue cliché. Companion to `seasea-brand` (master-brand surfaces).
---

# Boids Brand

Author and revise Boids-branded artifacts with the canonical brand system applied — positioning, personality, voice, Builder Ink visual identity, messaging, and GPT Image 2 preamble — so every output is consistent, on-message, and ready for external audiences.

## Strategic Frame

**Boids is the L2-1 professional efficiency workflow layer** of Nevamind's persistent-AI stack. It is the tool studio that lets builders construct, deploy, and monetize AI agent workflows — not a chatbot, not a consumer app, not a developer-only API.

The brand must communicate **builder confidence, professional precision, and orchestration mastery** — never hype, never magic framing, never L1a consumer playfulness.

## When to Use

- User asks to write, draft, refresh, or revise any Boids-branded copy (deck, pitch, page, social, ad)
- User asks to build a Boids pitch deck or client-facing deliverable
- User asks to generate brand visuals (GPT Image 2) for Boids
- User asks to apply the Boids brandbook to an existing draft
- User mentions Boids positioning, category labels, builder voice, or visual identity
- A new Boids workspace artifact is being scaffolded under `seasea-gtm-os/workspaces/nevamind/`

## Canonical Source Files

The skill relies on these canonical references — never override them:

| Source | Path |
|---|---|
| **Brandbook (canonical)** | `seasea-gtm-os/workspaces/nevamind/brand/boids-brandbook.md` |
| Brand quick reference | `.agents/skills/boids-brand/references/brand-quick-reference.md` |
| GPT Image 2 preamble | `.agents/skills/boids-brand/references/gpt-image2-preamble.md` |
| Messaging library | `.agents/skills/boids-brand/references/messaging-library.md` |
| Application playbooks | `.agents/skills/boids-brand/references/application-playbooks.md` |
| Brandbook one-page prompt | `seasea-gtm-os/workspaces/nevamind/brand/gpt-image2-prompts/boids-brandbook-one-page-prompt.md` |
| Positioning prompt | `seasea-gtm-os/workspaces/nevamind/brand/gpt-image2-prompts/nevamind-brand-positioning-one-page-prompt.md` |

**Order of authority:** brandbook > skill reference files > derived artifacts.

## Skill Reference Files

Read the relevant reference file before every authoring task:

| File | When to Read |
|---|---|
| `references/brand-quick-reference.md` | Every Boids authoring task — positioning labels, personality, voice, color tokens, typography, forbidden visuals |
| `references/gpt-image2-preamble.md` | Any task that produces GPT Image 2 prompts for Boids decks/pages |
| `references/messaging-library.md` | Writing hero copy, headlines, audience messages, narrative arc, taglines |
| `references/application-playbooks.md` | Scenario-specific application: pitch deck, single image, social, voiceover, web |

## Authoring Workflow

Follow this loop for any Boids authoring task:

### 1. Identify the application scenario

Match the request to one of the scenarios in `references/application-playbooks.md`:
- `pitch-deck` — investor or sales pitch deck
- `single-image` — single marketing image
- `long-form-social` — long-form social post or thread
- `voiceover` — TTS narration script for video
- `web-landing` — web or landing page

### 2. Apply the brand layer in this order

1. **Positioning** — confirm the category label is one of the approved set (§1). Forbidden: "AI chatbot marketplace", "AI celebrity app", "one-click AI automation", "no-code AI tool", "memory infrastructure" (MemU owns L3).
2. **Layer discipline** — confirm verbs are L2-1: build, run, publish, rank, credit, orchestrate. Never L1a: chat, discover, consume, talk, play.
3. **Hero line** — open with the canonical hero line from `references/messaging-library.md`.
4. **Voice & tone** — Builder confidence, professional precision, systems thinking, empathetic peer, measured ambition.
5. **Visual identity** — Builder Ink palette (Ink #0F0F0E + Bone #F2EDE4 + Phosphor #C7FF4A flat), Builder Stack typography (PP Editorial New + Cabinet Grotesk + Geist + JetBrains Mono), Double-Bezel surface system.
6. **Layout & governance** — 1920×1080 16:9, 5% top-left blank logo zone, `Privileged&Confidential` bottom-right, page number top-right.

### 3. Pre-flight Self-check

Before delivering output:

- [ ] No forbidden positioning labels ("AI chatbot marketplace", "AI celebrity app", "one-click", "no-code tool")
- [ ] Verbs are L2-1 only (build · run · publish · rank · credit · orchestrate)
- [ ] Hero line drawn from canonical set
- [ ] Builder Ink palette applied: Bone background, Ink text, Phosphor single accent flat
- [ ] No teal, no azure, no navy, no purple-to-blue gradient anywhere
- [ ] No banned fonts (Inter, Roboto, Open Sans, Helvetica, Space Grotesk, SF Pro)
- [ ] All numerics in JetBrains Mono with tabular-nums
- [ ] Double-Bezel card construction on all containers (24px/18px concentric radii)
- [ ] 3% film-grain overlay on all brand surfaces
- [ ] All GPT Image 2 prompts include canonical preamble from `references/gpt-image2-preamble.md`
- [ ] Slide decks: 5% top-left blank zone, P&C watermark bottom-right, page number top-right

## Companion Skills

| Skill | Use For |
|---|---|
| `seasea-brand` | Master-brand surfaces; switch when artifact is Seasea, not Boids |
| `musein-brand` | Switch when artifact is Musein.ai creative surface |
| `modelapi-brand` | Switch when artifact is ModelAPI.co developer surface |
| `high-end-visual-design` | Underlying anti-default UI rules — Boids adopts them as baseline |
| `seasea-deck` | Render a markdown deck → 16:9 PNG slides |
| `hyperframes` / `heygen` | Convert narration + visuals → final video |
| `higgsfield-generate` | Image generation; chain with this skill for brand-correct prompts |

## Output Conventions

- Default language: English (canonical). Use Chinese only when audience is SOE / Chinese-domestic.
- Footer citation on client deliverables: `Source: Boids Brandbook — [YYYY-MM-DD git-sha]`.
- All image-prompt blocks end with the `Privileged&Confidential` watermark clause.
- File path conventions: decks under `seasea-gtm-os/workspaces/nevamind/decks/`; rendered images under `workspaces/nevamind/brand/outputs/<artifact>/`.

## Versioning

This skill and the canonical brandbook it references are **Git-versioned**. There are no version numbers in filenames. All historical states are preserved in Git commits and tags. To see the full change history:

```bash
git log --oneline --follow workspaces/nevamind/brand/boids-brandbook.md
git tag -l "boids-brand/*"
```

---

**Brand operating motto** — *Build. Run. Publish.*
