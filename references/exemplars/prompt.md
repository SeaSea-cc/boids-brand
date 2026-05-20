# Exemplar Prompts & Approval Log

> Brandbook target: **v1.2 — Precision Mono + Ambient Glow** (release `2026-05-21-v1.2-expert-agent-platform`).
> One row per exemplar. Every exemplar in [`./README.md`](./README.md) must have a corresponding entry here before it ships.
> Brand-owner sign-off (`brand@nevamind.ai`) is recorded in the **Approved** column with the approval date in `YYYY-MM-DD` format.
> When an exemplar is replaced (cap is reached, brand version bump, etc.), strike through the row with `~~...~~` and add the replacement below.
> All prompts assume the canonical preamble defined in [`../gpt-image2-preamble.md`](../gpt-image2-preamble.md). The full prompt body lives in the per-exemplar section below the tables; the **Prompt** column links to that section.

---

## Positive exemplars

| # | File | Intent (what this exemplar teaches) | Prompt | Generated | Approved | Notes |
|---|---|---|---|---|---|---|
| 01 | `01-cover-white-glow.png` | White canvas + three-color desaturated radial Ambient Glow as background light source — universal hero cover | [§ P01](#p01--cover-white--desaturated-glow) | 2026-05-21 | — | Generated via GPT Image 2 (16:9, high) — awaiting brand-owner sign-off |
| 02 | `02-cover-black-glow.png` | Black canvas + vibrant saturated three-color radial Ambient Glow — inverted-night hero cover | [§ P02](#p02--cover-black--saturated-glow) | 2026-05-21 | — | Generated via GPT Image 2 (16:9, high) — awaiting sign-off |
| 03 | `03-bento-asymmetric.png` | Asymmetric Bento layout showing the two product lines (Boids Product + Boids API/CLI) with Double-Bezel cards | [§ P03](#p03--asymmetric-bento-two-product-lines) | 2026-05-21 | — | Generated via GPT Image 2 (3:2, high) — awaiting sign-off |
| 04 | `04-double-bezel-card.png` | Double-Bezel close-up: Gray-50 outer / White inner, 24/18 px concentric radii, inset highlight | [§ P04](#p04--double-bezel-card-close-up) | 2026-05-21 | — | Generated via GPT Image 2 (4:3, high) — awaiting sign-off |
| 05 | `05-cta-glow-stroke.png` | Primary CTA pill: Black fill, White text, 1.5 px three-color glow stroke, trailing arrow circle | [§ P05](#p05--primary-cta-pill-component-scale) | 2026-05-21 | — | Generated via GPT Image 2 (4:3, high) — awaiting sign-off |
| 06 | `06-eyebrow-tag.png` | Cabinet Grotesk eyebrow tag at 10 px / +0.2 em uppercase, glow @ 10% background | [§ P06](#p06--eyebrow-tag-component-scale) | 2026-05-21 | — | Generated via GPT Image 2 (4:3, high) — awaiting sign-off |
| 07 | `07-data-table-jbm.png` | JetBrains Mono tabular-nums agent credit ledger on White, hairlines at Black @ 5% | [§ P07](#p07--data-table-jetbrains-mono-tabular) | 2026-05-21 | — | Generated via GPT Image 2 (3:2, high) — awaiting sign-off |
| 08 | `08-editorial-split.png` | Editorial Split: PP Editorial New italic display left + narrative-arc card stack right | [§ P08](#p08--editorial-split-narrative-landing) | 2026-05-21 | — | Generated via GPT Image 2 (16:9, high) — awaiting sign-off |

## Negative exemplars (`donts/`)

| # | File | Anti-pattern shown | Prompt | Generated | Approved | Notes |
|---|---|---|---|---|---|---|
| 01 | `donts/01-stripe-gradient.png` | Stripe gradient across the surface (must be radial) | [§ N01](#n01--stripe-gradient-banned) | 2026-05-21 | — | Generated via GPT Image 2 (16:9, high) — awaiting sign-off |
| 02 | `donts/02-single-color-pull.png` | Single-color glow pull (all three colors must coexist) | [§ N02](#n02--single-color-glow-pull-banned) | 2026-05-21 | — | Generated via GPT Image 2 (16:9, high) — awaiting sign-off |
| 03 | `donts/03-cool-gray-bg.png` | Cool gray background `#FAFAFA` / `#F5F5F5` / `#E5E5E5` | [§ N03](#n03--cool-gray-background-banned) | 2026-05-21 | — | Generated via GPT Image 2 (16:9, high) — awaiting sign-off |
| 04 | `donts/04-glow-full-fill.png` | Glow color used as full background fill | [§ N04](#n04--glow-as-full-background-fill-banned) | 2026-05-21 | — | Generated via GPT Image 2 (16:9, high) — awaiting sign-off |
| 05 | `donts/05-banned-font.png` | Inter / Roboto / Open Sans / Helvetica / Space Grotesk in display | [§ N05](#n05--banned-display-font-banned) | 2026-05-21 | — | Generated via GPT Image 2 (3:2, high) — awaiting sign-off |
| 06 | `donts/06-equal-three-card.png` | Equal-height three-card feature row | [§ N06](#n06--equal-height-3-card-row-banned) | 2026-05-21 | — | Generated via GPT Image 2 (3:2, high) — awaiting sign-off |

---

## Prompt bodies

> Every prompt below begins with the canonical preamble token — agents should literally prepend the preamble paragraph from [`../gpt-image2-preamble.md`](../gpt-image2-preamble.md) when sending to GPT Image 2. The body text below is the **scene-specific block** that follows the preamble.

### P01 — Cover, White + Desaturated Glow

**File:** `01-cover-white-glow.png` · **Aspect:** 16:9 (1600×900) · **Glow mode:** Ambient (desaturated, low-opacity)

```
Brand: Boids — Precision Mono + Ambient Glow (v1.2). Pure White #FFFFFF canvas, full-bleed,
absolutely no cool gray. Three desaturated radial Ambient Glow blooms living BEHIND the
content layer: Cyan #06B6D4 bloom anchored top-left, Violet #8B5CF6 bloom anchored center-
right, Rose #EC4899 bloom anchored bottom-left. Each bloom 32–40% canvas-width radius,
opacity 12–18%, soft Gaussian falloff to 0, no banding, no stripe, no linear gradient.
Center the headline “Build expert agents. Bring them everywhere.” in PP Editorial New
Regular Italic, 96px, color Black #0D0D0D, tight tracking -0.01em, two lines, line-height
1.05. Above headline, an eyebrow tag in Cabinet Grotesk Medium, 10px, uppercase, +0.2em
tracking, color Black #0D0D0D, reading “BOIDS // EXPERT AGENT PLATFORM”. Below headline,
a single subhead line in Geist Regular, 18px, color Black #0D0D0D at 64% opacity, reading
“Build. Distribute. Work.”. Bottom-right corner: a primary CTA pill, Black #0D0D0D fill,
White #FFFFFF text “Start building →” in Geist Medium 14px, 1.5px stroke composed of the
three glow colors blended (cyan→violet→rose, 33% each, no banding), 999px corner radius,
14px vertical padding, 22px horizontal padding. No drop shadows, no glassmorphism, no
beveling, no specular highlights. Render at 16:9, 1600×900, white-point true, output PNG.
```

---

### P02 — Cover, Black + Saturated Glow

**File:** `02-cover-black-glow.png` · **Aspect:** 16:9 (1600×900) · **Glow mode:** Saturated (vibrant, mid-opacity)

```
Brand: Boids — Precision Mono + Ambient Glow (v1.2), inverted-night variant. Pure Black
#0D0D0D canvas, full-bleed, no charcoal/navy/dark-gray drift. Three vibrant radial Ambient
Glow blooms BEHIND the content layer: Cyan #06B6D4 bloom anchored top-right, Violet
#8B5CF6 bloom anchored bottom-center, Rose #EC4899 bloom anchored top-left. Each bloom
36–44% canvas-width radius, opacity 38–52%, soft Gaussian falloff, no stripe, no linear
gradient, no scanlines. Glow blooms must remain three discrete sources — never merge into
a uniform wash. Center the headline “Build expert agents. Bring them everywhere.” in PP
Editorial New Regular Italic, 96px, color White #FFFFFF, tracking -0.01em, two lines,
line-height 1.05. Eyebrow tag above in Cabinet Grotesk Medium, 10px, uppercase, +0.2em,
color White #FFFFFF at 64% opacity, reading “BOIDS // V1.2 — NIGHT MODE”. Subhead below
in Geist Regular, 18px, White #FFFFFF at 64% opacity, reading “Build. Distribute. Work.”.
Bottom-right primary CTA pill: White #FFFFFF fill, Black #0D0D0D text “Start building →”
in Geist Medium 14px, 1.5px stroke of cyan→violet→rose blended evenly, 999px radius. No
drop shadows, no glassmorphism, no neon outer-glow on text. Render 16:9, 1600×900, PNG.
```

---

### P03 — Asymmetric Bento, Two Product Lines

**File:** `03-bento-asymmetric.png` · **Aspect:** 3:2 (1500×1000) · **Layout:** Asymmetric Bento

```
Brand: Boids — Precision Mono + Ambient Glow (v1.2). Pure White #FFFFFF canvas, 64px outer
margin. A single ambient Cyan #06B6D4 + Violet #8B5CF6 + Rose #EC4899 three-color radial
glow at 8–12% opacity sits diffuse in the background, anchored bottom-right. Asymmetric
Bento grid, 12 columns × 6 rows, 24px gutter, NO equal-height card row. Card layout:

  • Card A — large primary card, columns 1–7, rows 1–4. Double-Bezel surface: outer fill
    Gray-50 #F4F4F5, 24px corner radius, inner panel White #FFFFFF inset 8px, 18px corner
    radius, 1px hairline Black #0D0D0D at 6% opacity around inner panel. Eyebrow “PRODUCT
    // BOIDS PRODUCT” Cabinet Grotesk 10px uppercase. Headline “Talk to your team’s
    expert agents in Slack and Telegram.” PP Editorial New Italic 36px, two lines.
    Subhead Geist Regular 14px, 64% Black: “Bring expert intelligence into the chat your
    team already lives in.” One small inline CTA pill bottom-left.
  • Card B — tall card, columns 8–12, rows 1–6. Double-Bezel as above. Eyebrow “PRODUCT
    // BOIDS API & CLI”. Headline “Compose expert agents into your workflows.” PP
    Editorial New Italic 32px. A monospaced code block in JetBrains Mono Regular 13px on
    Black #0D0D0D fill White #FFFFFF text inner panel, showing literally:
        $ boids deploy --agent finance-analyst
        ✓ deployed → https://boids.dev/a/fa
    No syntax highlighting beyond Black/White; a 1px three-color glow underline beneath
    the success line.
  • Card C — wide card, columns 1–7, rows 5–6. Single-line eyebrow “PROOF // EARNINGS”
    plus a JetBrains Mono tabular figure “$48,210.27” at 28px, Black #0D0D0D, with a
    small Geist Regular 12px caption “Distributed to 412 builders this week.”

Typography stack only: PP Editorial New (italic display), Cabinet Grotesk (eyebrow),
Geist (UI), JetBrains Mono (code/figures). NO Inter, Roboto, Open Sans, Helvetica, Space
Grotesk. No drop shadows, no gradients on cards, no glassmorphism, no faux-3D. Render
3:2, 1500×1000, PNG.
```

---

### P04 — Double-Bezel Card Close-Up

**File:** `04-double-bezel-card.png` · **Aspect:** 4:3 (1280×960) · **Layout:** Component-scale spec sheet

```
Brand: Boids — Precision Mono + Ambient Glow (v1.2). Pure White #FFFFFF canvas. A single
Double-Bezel surface centered, occupying 70% of canvas width. Construction, exact specs:

  • Outer panel: fill Gray-50 #F4F4F5, corner radius 24px, no border, no shadow.
  • Inner panel: inset 8px on all four sides from outer, fill White #FFFFFF, corner
    radius 18px, hairline 1px Black #0D0D0D at 6% opacity around the inner edge only.
  • Inner panel inset highlight: a 1px White #FFFFFF top-edge stroke at 90% opacity, 0px
    on the other three edges, simulating a printed-card top bevel.

Inside the inner panel, a minimal spec card: eyebrow tag Cabinet Grotesk Medium 10px
uppercase +0.2em “COMPONENT // SURFACE.DOUBLE-BEZEL”, headline PP Editorial New Italic
32px Black #0D0D0D “The card is two cards.”, body Geist Regular 14px Black 72% “Outer
Gray-50, 24px radius. Inner White, 18px radius, inset 8px. The bezel band makes the
content feel mounted, not pasted.”

Around the surface, four annotation callouts in Geist Regular 11px Black 64%, connected
by 1px hairlines at Black 16%, labeling:
  ① Outer fill Gray-50 #F4F4F5
  ② Outer radius 24px
  ③ Inner radius 18px
  ④ Inset 8px (the bezel band)

A faint three-color radial Ambient Glow at 6% opacity sits in the canvas background only,
NEVER on the card. No shadows on the card, no gradient on the bezel, no metallic effect.
Render 4:3, 1280×960, PNG.
```

---

### P05 — Primary CTA Pill, Component Scale

**File:** `05-cta-glow-stroke.png` · **Aspect:** 4:3 (1280×960) · **Layout:** Component spec sheet

```
Brand: Boids — Precision Mono + Ambient Glow (v1.2). Pure White #FFFFFF canvas. Centered,
a single primary CTA pill at 4× scale for legibility:

  • Pill body: Black #0D0D0D fill, 999px corner radius, no shadow, no gradient.
  • Pill stroke: 1.5px outer stroke, gradient stops Cyan #06B6D4 → Violet #8B5CF6 → Rose
    #EC4899, distributed evenly along the pill perimeter (each color ≈33% of the path),
    no banding, smooth interpolation.
  • Label: Geist Medium 14px, color White #FFFFFF, kerning -0.005em, reading literally
    “Start building”.
  • Trailing arrow circle: 24px diameter, fill White #FFFFFF, centered arrow “→”
    JetBrains Mono Bold 12px Black #0D0D0D, 8px right margin from the label.
  • Padding: 14px vertical, 22px horizontal (label edge to pill edge).

Surrounding spec annotations in Geist Regular 11px Black 64%, hairlines Black 16%:
  ① 1.5px stroke / cyan→violet→rose
  ② 999px radius
  ③ 14px vertical padding
  ④ Trailing arrow circle, 24px

Background: Pure White only — NO ambient glow on this card (component spec sheets stay
neutral so the stroke colors read true). No drop shadows, no inner glow, no neon. Render
4:3, 1280×960, PNG.
```

---

### P06 — Eyebrow Tag, Component Scale

**File:** `06-eyebrow-tag.png` · **Aspect:** 4:3 (1280×960) · **Layout:** Component spec sheet

```
Brand: Boids — Precision Mono + Ambient Glow (v1.2). Pure White #FFFFFF canvas with a
single three-color radial Ambient Glow at 10% opacity diffuse in the background, anchored
top-center. Centered, an eyebrow tag at 4× scale:

  • Text: Cabinet Grotesk Medium, 10px (rendered at 4× = 40px on canvas), uppercase,
    tracking +0.2em, color Black #0D0D0D, reading literally “BOIDS // EXPERT AGENT
    PLATFORM”.
  • Leading marker: a 6px × 6px square in solid Black #0D0D0D, 8px to the left of the
    text baseline, vertical-aligned to cap height.
  • No background pill, no underline, no border. The eyebrow sits on the canvas as raw
    text + marker.

Below the eyebrow, in PP Editorial New Italic 24px Black #0D0D0D, the line “The
agent-line for any context.” as a usage example.

Surrounding spec annotations in Geist Regular 11px Black 64%, hairlines Black 16%:
  ① Cabinet Grotesk Medium 10px
  ② Uppercase + 0.2em tracking
  ③ 6px square marker, 8px lead
  ④ Color: Black #0D0D0D (light theme) / White #FFFFFF (dark theme)

No drop shadows, no glow on the text itself, no italic on the eyebrow. Render 4:3,
1280×960, PNG.
```

---

### P07 — Data Table, JetBrains Mono Tabular

**File:** `07-data-table-jbm.png` · **Aspect:** 3:2 (1500×1000) · **Layout:** Editorial data table

```
Brand: Boids — Precision Mono + Ambient Glow (v1.2). Pure White #FFFFFF canvas, 64px
outer margin. A single Double-Bezel surface holding an agent credit ledger table. Outer
Gray-50 #F4F4F5, 24px radius. Inner White, 18px radius, inset 8px.

Inside the inner panel:
  • Header row: eyebrow Cabinet Grotesk Medium 10px uppercase +0.2em Black #0D0D0D,
    “LEDGER // AGENT EARNINGS — WEEK 21”.
  • Title: PP Editorial New Italic 28px Black #0D0D0D, “Earnings, line by line.”
  • Table, 6 columns × 8 rows + header. Typography:
      – Column headers: Geist Medium 12px Black #0D0D0D, uppercase, +0.05em tracking.
      – Cell text: JetBrains Mono Regular 13px Black #0D0D0D, tabular-nums on, all
        figures right-aligned.
  • Columns: AGENT | OWNER | RUNS | UNIT $ | GROSS | NET (after platform fee).
  • Sample rows (use exactly these values, do NOT invent new data):
      finance-analyst    nevamind    1,204    0.42    $505.68    $480.40
      contract-redliner  acme-legal     872    0.65    $566.80    $538.46
      sql-explainer      data-co      2,011    0.18    $361.98    $343.88
      cohort-cutter      growth-lab     463    0.95    $439.85    $417.86
      a11y-auditor       freelance      318    1.10    $349.80    $332.31
      brand-checker      boids-core     902    0.30    $270.60    $257.07
      pr-summarizer      lab-22         617    0.25    $154.25    $146.54
      onboarding-coach   ops-team       240    1.40    $336.00    $319.20
  • Hairlines between rows: 1px Black #0D0D0D at 5% opacity, no full borders, no
    alternating-row fill.
  • Footer row: Geist Medium 13px Black 100%, totals across NET only: “TOTAL · $2,835.72
    · 412 BUILDERS PAID”.

Outside the surface, a faint three-color radial Ambient Glow at 6% opacity in the canvas
background only. No drop shadows on the table, no gradient cells, no chart-style color
fills inside cells. Render 3:2, 1500×1000, PNG.
```

---

### P08 — Editorial Split, Narrative Landing

**File:** `08-editorial-split.png` · **Aspect:** 16:9 (1600×900) · **Layout:** Editorial Split

```
Brand: Boids — Precision Mono + Ambient Glow (v1.2). Pure White #FFFFFF canvas, 64px
outer margin. Three-color radial Ambient Glow at 10% opacity in the background only,
anchored bottom-right. Two-column editorial split, 6 + 6 of 12 columns, 32px gutter.

Left column — display statement:
  • Eyebrow Cabinet Grotesk Medium 10px uppercase +0.2em Black #0D0D0D, “NARRATIVE //
    SIX BEATS”.
  • Headline PP Editorial New Regular Italic 88px Black #0D0D0D, three lines, tracking
    -0.015em, line-height 1.02:
        Build expert agents.
        Distribute them everywhere.
        Get paid when they work.
  • Below the headline, a Geist Regular 14px Black 64% paragraph, max-width 36ch:
    “Boids turns prompts and tools into expert agents you can ship to Slack, Telegram,
    your CLI, and your customers’ apps. Earnings flow back to the builder, line by
    line.”

Right column — narrative-arc card stack, 6 stacked Double-Bezel mini-cards (outer
Gray-50, inner White, 16px radius / 11px radius, inset 5px). Each card is one beat:
  ① PAIN — “Hiring an expert is slow.”
  ② PROBLEM — “Generic LLMs don’t know your domain.”
  ③ REVEAL — “Expert agents you can build, deploy, and call.”
  ④ PROOF — “412 builders paid this week.”
  ⑤ OUTCOME — “Workflows that compound, not just chats that end.”
  ⑥ CTA — “Start building →” (this card uses Black #0D0D0D fill, White text, three-
       color glow stroke 1.5px, 999px corner radius — the only inverted card).

Card typography: Cabinet Grotesk Medium 10px uppercase eyebrow (the beat name); Geist
Regular 14px Black #0D0D0D body. No icons. No shadows. No glow on the cards themselves.

Typography stack only: PP Editorial New, Cabinet Grotesk, Geist. NO Inter, Roboto, Open
Sans, Helvetica, Space Grotesk. Render 16:9, 1600×900, PNG.
```

---

### N01 — Stripe Gradient (banned)

**File:** `donts/01-stripe-gradient.png` · **Aspect:** 16:9 (1600×900) · **Mode:** Negative exemplar

```
Brand: Boids — Precision Mono + Ambient Glow (v1.2). NEGATIVE EXEMPLAR — DO NOT IMITATE.

Render a banned cover: Pure White #FFFFFF canvas with a horizontal LINEAR STRIPE gradient
spanning the full canvas width — Cyan #06B6D4 on the left edge, Violet #8B5CF6 in the
middle, Rose #EC4899 on the right edge — opacity 100%, hard banding visible. This is the
exact thing v1.2 forbids: glow must be RADIAL, never a stripe; must live BEHIND content,
never as a full-bleed wash.

Overlay headline “Build expert agents.” in PP Editorial New Italic 88px Black #0D0D0D,
centered.

A heavy diagonal red strike-through line, 6px wide, color #DC2626, runs corner to corner
top-left to bottom-right, with a callout label in Geist Medium 14px Black #0D0D0D in the
top-right corner reading literally:
    BANNED — STRIPE GRADIENT
    Use radial Ambient Glow instead. See gpt-image2-preamble.md §3.

Render 16:9, 1600×900, PNG. The image is intentionally wrong.
```

---

### N02 — Single-Color Glow Pull (banned)

**File:** `donts/02-single-color-pull.png` · **Aspect:** 16:9 (1600×900) · **Mode:** Negative exemplar

```
Brand: Boids — Precision Mono + Ambient Glow (v1.2). NEGATIVE EXEMPLAR — DO NOT IMITATE.

Render a banned cover: Pure White #FFFFFF canvas with a single Cyan #06B6D4 radial glow
filling 80% of canvas width at 60% opacity, anchored center, NO Violet, NO Rose. This
violates v1.2: all three glow colors must coexist in any composition where the Ambient
Glow is used; pulling a single color is reserved for product chrome and never for hero
covers.

Overlay headline “Build expert agents.” in PP Editorial New Italic 88px Black #0D0D0D,
centered.

A heavy diagonal red strike-through line, 6px wide, color #DC2626, corner to corner. Top-
right callout in Geist Medium 14px Black #0D0D0D reading literally:
    BANNED — SINGLE-COLOR GLOW PULL
    All three colors (cyan/violet/rose) must coexist on hero surfaces.

Render 16:9, 1600×900, PNG. The image is intentionally wrong.
```

---

### N03 — Cool Gray Background (banned)

**File:** `donts/03-cool-gray-bg.png` · **Aspect:** 16:9 (1600×900) · **Mode:** Negative exemplar

```
Brand: Boids — Precision Mono + Ambient Glow (v1.2). NEGATIVE EXEMPLAR — DO NOT IMITATE.

Render a banned cover: Cool Gray #F5F5F5 canvas (NOT White, NOT Black, NOT Gray-50
#F4F4F5 — this is the wrong gray). No glow at all. Overlay headline “Build expert
agents.” in PP Editorial New Italic 88px Black #0D0D0D, centered. The flat cool gray
makes the surface feel like a generic SaaS template — exactly what v1.2 rules out: only
Pure White or Pure Black are valid hero backgrounds, with Gray-50 reserved as the OUTER
bezel of Double-Bezel cards.

A heavy diagonal red strike-through line, 6px wide, color #DC2626, corner to corner. Top-
right callout in Geist Medium 14px Black #0D0D0D reading literally:
    BANNED — COOL GRAY BACKGROUND
    Hero canvases are White #FFFFFF or Black #0D0D0D only.

Render 16:9, 1600×900, PNG. The image is intentionally wrong.
```

---

### N04 — Glow as Full Background Fill (banned)

**File:** `donts/04-glow-full-fill.png` · **Aspect:** 16:9 (1600×900) · **Mode:** Negative exemplar

```
Brand: Boids — Precision Mono + Ambient Glow (v1.2). NEGATIVE EXEMPLAR — DO NOT IMITATE.

Render a banned cover: full-bleed solid Violet #8B5CF6 fill, 100% opacity, no White, no
Black, no radial falloff — the glow color used as the entire background. This violates
v1.2 rule #3: Ambient Glow is a soft radial bloom on a White or Black canvas, NEVER a
flat color fill.

Overlay headline “Build expert agents.” in PP Editorial New Italic 88px White #FFFFFF,
centered.

A heavy diagonal red strike-through line, 6px wide, color #DC2626, corner to corner. Top-
right callout in Geist Medium 14px White #FFFFFF reading literally:
    BANNED — GLOW AS FULL FILL
    Glow is a radial bloom on White/Black. Never a solid background.

Render 16:9, 1600×900, PNG. The image is intentionally wrong.
```

---

### N05 — Banned Display Font (banned)

**File:** `donts/05-banned-font.png` · **Aspect:** 3:2 (1500×1000) · **Mode:** Negative exemplar / split comparison

```
Brand: Boids — Precision Mono + Ambient Glow (v1.2). NEGATIVE EXEMPLAR — DO NOT IMITATE.

Render a split comparison on Pure White #FFFFFF canvas, two columns 50/50, 32px gutter.

LEFT column — labelled “BANNED” in Cabinet Grotesk Medium 10px uppercase Red #DC2626 at
the top:
  • Headline “Build expert agents.” in HELVETICA NEUE BOLD 72px Black #0D0D0D.
  • Below it, three more banned options stacked, each at 28px:
      – “Build expert agents.” in Inter Bold.
      – “Build expert agents.” in Roboto Bold.
      – “Build expert agents.” in Space Grotesk Bold.
  • A heavy diagonal red strike-through, 6px #DC2626, across the entire left column.
  • Footnote Geist Regular 11px Black 64%: “Inter / Roboto / Open Sans / Helvetica /
    Space Grotesk are banned in display.”

RIGHT column — labelled “CORRECT” in Cabinet Grotesk Medium 10px uppercase Black at the
top:
  • Headline “Build expert agents.” in PP EDITORIAL NEW REGULAR ITALIC 72px Black
    #0D0D0D, tracking -0.01em.
  • Below it, three correct sub-styles, each at 28px:
      – Eyebrow “EYEBROW SAMPLE” in Cabinet Grotesk Medium uppercase +0.2em.
      – Body “The agent-line for any context.” in Geist Regular.
      – Code “$ boids deploy --agent finance-analyst” in JetBrains Mono Regular.
  • Footnote Geist Regular 11px Black 64%: “PP Editorial New + Cabinet Grotesk + Geist +
    JetBrains Mono — the only approved Builder Stack.”

No glow on this exemplar. Render 3:2, 1500×1000, PNG. The left half is intentionally
wrong; the right half is the correct reference.
```

---

### N06 — Equal-Height 3-Card Row (banned)

**File:** `donts/06-equal-three-card.png` · **Aspect:** 3:2 (1500×1000) · **Mode:** Negative exemplar / split comparison

```
Brand: Boids — Precision Mono + Ambient Glow (v1.2). NEGATIVE EXEMPLAR — DO NOT IMITATE.

Render a split comparison on Pure White #FFFFFF canvas, two stacked rows, 32px gutter.

TOP row — labelled “BANNED” in Cabinet Grotesk Medium 10px uppercase Red #DC2626:
  • Three IDENTICAL cards in a 3-column equal-height grid, each 33%, 24px gutter, no
    Double-Bezel, single flat White panel with 1px Black 12% border. Each card has the
    same icon placeholder square 40×40 Black 8% top-left, the same headline “Feature
    one.” / “Feature two.” / “Feature three.” in Inter Bold 18px, the same lorem body
    in Inter Regular 13px Black 64%. This is the generic SaaS feature-row pattern v1.2
    bans.
  • A heavy diagonal red strike-through, 6px #DC2626, across the entire top row.
  • Footnote Geist Regular 11px Black 64%: “Equal-height 3-card rows are banned —
    they read as generic SaaS template.”

BOTTOM row — labelled “CORRECT” in Cabinet Grotesk Medium 10px uppercase Black:
  • Asymmetric Bento, same canvas region: one large Double-Bezel card 7/12 wide, one
    tall card 5/12 wide spanning full height, one wide card 7/12 underneath. Outer
    Gray-50 #F4F4F5 24px radius, inner White #FFFFFF 18px radius, inset 8px. Headlines
    in PP Editorial New Italic, eyebrows in Cabinet Grotesk, body in Geist. One card
    contains a JetBrains Mono code block, one contains a tabular figure “$2,835.72”,
    one contains a primary CTA pill with three-color glow stroke.
  • Footnote Geist Regular 11px Black 64%: “Asymmetric Bento with Double-Bezel surfaces
    is the v1.2 default for feature stories.”

Render 3:2, 1500×1000, PNG. The top row is intentionally wrong; the bottom row is the
correct reference.
```

---

## Row template (copy this when adding a new exemplar)

```
| NN | `NN-<slug>.png` | <one-sentence intent> | [§ PNN](#pnn--<anchor>) | YYYY-MM-DD | YYYY-MM-DD | <reviewer note> |
```

## Replacement convention

When the exemplar cap is reached (12 positive / 6 negative) or a brandbook version bump invalidates an exemplar:

1. Strike through the old row: wrap the row's cells in `~~...~~`.
2. Add the new row below with a fresh sequence number.
3. Delete the old PNG file in the same commit.
4. Note the replacement reason in the new row's **Notes** column.
