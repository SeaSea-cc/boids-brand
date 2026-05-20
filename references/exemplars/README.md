# Boids Brand — v1.2 Exemplars

> **Brandbook version:** v1.2 — confirmed by Nevamind / Boids founder Chen Hong.
> **Source of truth:** [`../brandbook.md`](../brandbook.md). When an exemplar conflicts with the brandbook, the brandbook wins and the exemplar must be replaced.
> **Status:** Curated visual exemplars for the Boids brand system. Not a gallery of outputs.

This directory holds the **only** images allowed to live inside the `boids-brand` skill repository. Everything else — per-deck slides, per-campaign social images, per-artifact renders — belongs in the consuming workspace under `<workspace>/brand-outputs/<artifact>/`, never here.

---

## Purpose

Exemplars exist for one reason: to give other agents and designers a **canonical visual reference** for what v1.2 *Precision Mono + Ambient Glow* actually looks like. They are the visual companion to the rules written in [`../brandbook.md`](../brandbook.md), [`../gpt-image2-preamble.md`](../gpt-image2-preamble.md), and [`../brand-quick-reference.md`](../brand-quick-reference.md).

Use them as:

- A reference set when authoring new GPT Image 2 prompts.
- A "do / don't" companion to the forbidden-visuals list.
- A visual audit baseline when reviewing third-party Boids output.

Do **not** use them as ready-made deck slides or marketing assets. They are reference exemplars, not publishable artifacts.

---

## Curation Rules (binding)

| Rule | Specification |
|---|---|
| **Max count** | ≤ 12 positive exemplars + ≤ 6 negative exemplars (`donts/`). Exceeding the cap triggers replacement, not addition. |
| **Format** | PNG only. JPEG, WebP, AVIF, GIF, SVG, PDF are rejected. |
| **Long edge** | ≤ 1600 px. 1920×1080 production masters live in `<workspace>/brand-outputs/`, never here. |
| **File size** | ≤ 600 KB per image. Use `pngquant --quality=70-85` or equivalent to compress. |
| **Naming** | `NN-<slug>.png` (e.g. `01-cover-white-glow.png`). Two-digit sequence number, kebab-case slug. Negative exemplars under `donts/` follow the same convention. |
| **Metadata** | Every exemplar requires an entry in [`prompt.md`](./prompt.md) with: GPT Image 2 prompt used, generation date, intended teaching point, brand-owner sign-off date. |
| **Brand sign-off** | Every exemplar must be approved by the brand owner (`brand@nevamind.ai`) before commit. Approval is recorded in `prompt.md`. |
| **Versioning** | Exemplars are refreshed on each major brandbook version bump and tagged alongside the release (`release/YYYY-MM-DD-<slug>`). |
| **Git LFS** | If aggregate exemplar size exceeds 5 MB, enable Git LFS in the skill repository's `.gitattributes` and migrate before next commit. |

---

## Recommended Set (v1.2)

The first canonical exemplar batch under v1.2. File names below are **placeholders** until the brand owner approves the actual renders.

### Positive exemplars (`./`)

| # | File | Teaches |
|---|---|---|
| 01 | `01-cover-white-glow.png` | White `#FFFFFF` canvas with desaturated three-color radial Ambient Glow as background light source — universal hero cover |
| 02 | `02-cover-black-glow.png` | Black `#0D0D0D` canvas with vibrant saturated three-color radial Ambient Glow — inverted-night hero cover |
| 03 | `03-bento-asymmetric.png` | Asymmetric Bento layout, Double-Bezel cards, single ambient-glow CTA accent |
| 04 | `04-double-bezel-card.png` | Single Double-Bezel card close-up: Gray-50 outer / White inner, 24/18 px concentric radii, inset highlight |
| 05 | `05-cta-glow-stroke.png` | Primary CTA pill button: Black fill, White text, 1.5 px three-color glow stroke, trailing arrow circle |
| 06 | `06-eyebrow-tag.png` | Cabinet Grotesk eyebrow tag at 10 px / +0.2 em uppercase, glow @ 10% background |
| 07 | `07-data-table-jbm.png` | JetBrains Mono tabular-nums data table on White, hairlines at Black @ 5% |
| 08 | `08-editorial-split.png` | Editorial Split layout: PP Editorial New italic display left + scrollable interactive right |

### Negative exemplars (`./donts/`)

| # | File | Anti-pattern |
|---|---|---|
| 01 | `donts/01-stripe-gradient.png` | Banned: stripe gradient across the surface (must be radial) |
| 02 | `donts/02-single-color-pull.png` | Banned: single-color glow pull (all three colors must coexist) |
| 03 | `donts/03-cool-gray-bg.png` | Banned: cool gray background `#FAFAFA` / `#F5F5F5` / `#E5E5E5` |
| 04 | `donts/04-glow-full-fill.png` | Banned: glow color used as full background fill |
| 05 | `donts/05-banned-font.png` | Banned: Inter / Roboto / Open Sans / Helvetica / Space Grotesk in display |
| 06 | `donts/06-equal-three-card.png` | Banned: equal-height three-card feature row |

---

## How to Add a New Exemplar

1. Generate the image using the canonical preamble in [`../gpt-image2-preamble.md`](../gpt-image2-preamble.md).
2. Compress to ≤ 600 KB long-edge ≤ 1600 px PNG.
3. Place under `references/exemplars/` (or `references/exemplars/donts/` for anti-patterns).
4. Add a row to [`prompt.md`](./prompt.md) with prompt + intent + date.
5. Open a PR; tag the brand owner (`brand@nevamind.ai`) for sign-off.
6. After approval, ensure aggregate size is < 5 MB (enable Git LFS otherwise).
7. On merge that ships with a brandbook version bump, ensure the next `release/YYYY-MM-DD-<slug>` tag is moved to include the new exemplar.

---

## What Does Not Belong Here

- Per-deck slide renders → `<workspace>/decks/<deck-name>/`
- Per-campaign marketing images → `<workspace>/brand-outputs/<artifact>/`
- 1920×1080 production masters → `<workspace>/brand-outputs/`
- Customer / partner co-branded outputs → owned by the producing organization, not the skill
- Logo files in any format → handled separately under brand-asset distribution governed by [`../../TRADEMARKS.md`](../../TRADEMARKS.md)

If in doubt, the rule is: **the skill repository ships rules, not output**. An exemplar earns its place only when it teaches a rule that words alone cannot convey.
