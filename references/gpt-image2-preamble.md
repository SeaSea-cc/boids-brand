# Boids Brand — GPT Image 2 Prompt Preamble (v1.2)

> **Brandbook version:** v1.2 — confirmed by Nevamind / Boids founder Chen Hong.
> **Source of truth:** [`brandbook.md`](./brandbook.md). When this file conflicts with the brandbook, the brandbook wins.
> Paste the canonical preamble below verbatim at the start of every Boids GPT Image 2 prompt.
> Confidentiality watermark text (e.g. `Privileged&Confidential`) is optional and depends on the deliverable's distribution context — see notes after the preamble.

---

## Canonical Preamble (v1.2 — Precision Mono + Ambient Glow)

```
Create a 16:9 executive strategy slide image, 1920x1080, for Boids (boids.so).
Use a systems-thinking, builder-grade visual standard: clean information
hierarchy, professional editorial layout, scannable technical content,
crisp vector-like diagrams, monospace data labels, and no consumer-app
playfulness.

Use a strict Precision Mono base — pure White (#FFFFFF) or deep Black
(#0D0D0D) as the canvas — overlaid with a 3% film-grain texture. Black
and White carry the structure. As the decorative layer, render an
Ambient Glow built from three colors: Cyan #06B6D4, Violet #8B5CF6,
and Rose #EC4899. The glow MUST appear as soft, radial, atmospheric
washes — never as a stripe gradient, never as a flat full-surface fill,
never a single-color pull. On Black: vibrant, saturated radial glows.
On White: desaturated pastel radial washes. All three colors must
coexist on the surface.

Use no other accent colors. No teal-to-blue or purple-to-blue stripe
gradients of any kind. Neutrals are warm grays (Gray-50 #F7F7F7,
Gray-400 #9E9E9E, Gray-700 #3D3D3D) — never cool grays such as #FAFAFA,
#F5F5F5, or #E5E5E5.

Typography: PP Editorial New for any display headline (italic
permitted), Cabinet Grotesk for eyebrow tags and section titles, Geist
for body copy, JetBrains Mono for any numbers or data labels. Never
use Inter, Roboto, Arial, Open Sans, Helvetica, SF Pro, Source Sans
Pro, or Space Grotesk.

All cards, panels, and containers use a Double-Bezel nested-enclosure
architecture: an outer Gray-50 hairline-ringed shell (1px Black at 5%
opacity, 24px radius) with a slightly distinct inner White core surface
(18px radius, inset highlight at White 60%). Shadows are Black-tinted
at low opacity (around 8%), never pure rgba(0,0,0,*).

Buttons are pill-shaped with a Black fill, White text, and a thin
1.5px gradient glow stroke composed of the three glow colors.

In the upper-left corner, reserve a blank square equal to 5% of the
total image width; keep this area identical to the background, with
no border, no placeholder, no icon, no logo, and no framing. Do not
draw the Boids logo. Add the exact text "Privileged&Confidential" in
small light-gray type at the bottom-right corner. Add a small page
number at the top-right corner in JetBrains Mono.
```

---

## Confidentiality Watermark (Optional)

The preamble above includes the literal text `Privileged&Confidential` (no space) in the bottom-right corner. This is appropriate for **internal**, **NDA-protected**, or **investor-only** decks. For **public** Boids assets (marketing pages, social posts, press kits), **omit** the confidentiality watermark by removing the sentence:

> "Add the exact text 'Privileged&Confidential' in small light-gray type at the bottom-right corner."

Replace with the producing organization's own footer convention, or leave the bottom-right empty.

---

## Required Elements Checklist

Every Boids GPT Image 2 prompt must include all of these:

| Element | Required phrase |
|---|---|
| Aspect ratio | `16:9` AND `1920x1080` |
| Visual register | `systems-thinking, builder-grade visual standard` |
| Background | Pure White `#FFFFFF` OR deep Black `#0D0D0D` only |
| Texture | `3% film-grain texture` |
| Decorative layer | `Ambient Glow` using `#06B6D4`, `#8B5CF6`, `#EC4899` — radial, atmospheric, never stripe, never single-color pull, all three coexist |
| Banned colors | No teal-to-blue, no purple-to-blue stripe gradients; no flat glow-color background fills; no cool grays (`#FAFAFA`, `#F5F5F5`, `#E5E5E5`) |
| Banned fonts | Never use Inter, Roboto, Arial, Open Sans, Helvetica, SF Pro, Source Sans Pro, or Space Grotesk |
| Required fonts | `PP Editorial New` AND `Cabinet Grotesk` AND `Geist` AND `JetBrains Mono` |
| Surface system | `Double-Bezel nested-enclosure architecture` (Gray-50 outer / White inner, 24px / 18px concentric radii) |
| Shadow rule | Black-tinted at low opacity (~8%), never pure `rgba(0,0,0,*)` |
| Logo safe zone | `5% of the total image width` blank square top-left, `no logo`, `no framing` |
| Logo prohibition | `Do not draw the Boids logo` |
| Confidentiality watermark | `Privileged&Confidential` (exact spelling, no space) — optional, only when distribution context requires it |
| Page number | `small page number at the top-right corner in JetBrains Mono` |

---

## Prompt Block Structure

After the preamble, structure every prompt as:

```
### Page NN Prompt — <Title>

Slide theme: "<Page Title> — <Hook Sentence>." <One sentence on slide intent.>

Core content to show: <Specific factual content. Numbers, named modules,
named agent capabilities, named workflows. NO vague hype.>

Visual direction: <Layout description (Asymmetric Bento / Editorial Split
/ Document Bento). Ambient glow placement (radial, atmospheric, all three
colors coexisting — never stripe). Restate forbidden visuals where
relevant: no stock-photo people, no teal-blue stripe gradient, no cartoon
robots/brains, no SaaS chat mockup, no Lucide icons, no cool gray.>
```

---

## v1.2 Migration Notes

If you previously used the v1.1 "Builder Ink" preamble (Bone `#F2EDE4` + Ink `#0F0F0E` + Phosphor `#C7FF4A`), update to v1.2 by:

1. Swapping the warm Bone background for either pure White `#FFFFFF` or deep Black `#0D0D0D`.
2. Replacing the single Phosphor flat accent with the **three-color Ambient Glow** (`#06B6D4`, `#8B5CF6`, `#EC4899`) — radial only, never stripe, all three must coexist on the surface.
3. Updating the Double-Bezel surface from Bone-200 / Bone to Gray-50 / White.
4. Replacing warm-Ink-tinted shadows with Black-tinted shadows at ~8% opacity.

The Builder Stack typography, 3% film-grain texture, 5% top-left logo safe zone, and Double-Bezel architecture are unchanged from v1.1.
