# Boids Brand — Application Playbooks

> Scenario-specific application rules covering the full GTM surface of an AI-infra / AI-agent company on a $1B trajectory.
> Pick **one playbook per artifact**. Always read [`brand-quick-reference.md`](./brand-quick-reference.md) for tokens before applying any playbook below.
> Confidentiality watermark text (e.g. `Privileged&Confidential`) appears below only as an optional governance overlay — apply it solely when the deliverable's distribution context requires it. Public, OSS, and developer-facing surfaces almost never carry it.

---

## Application Surface Matrix

| # | Surface | Funnel Stage | Primary Audience | Format / Channel |
|---|---|---|---|---|
| 1 | Pitch / Sales Deck | Conversion / IR | Investor, Buyer | 1920×1080 PDF / Keynote |
| 2 | One-Pager / Solution Brief | Conversion | Buyer, Champion | A4 / Letter PDF |
| 3 | Customer Case Study | Conversion / Advocacy | Buyer, Press | Web + PDF |
| 4 | RFP / Procurement / Trust Pack | Conversion | Procurement, Security | PDF set |
| 5 | Investor Update / Board Deck | IR | Investor, Board | 1920×1080 PDF + email |
| 6 | Single Marketing Image | Acquisition | Builder, Operator | LinkedIn / X / blog |
| 7 | Performance Ad / Paid Social | Acquisition | Builder, Operator | Static + 9:16 / 1:1 video |
| 8 | Out-of-Home / Billboard | Awareness | All | Billboard, transit, airport |
| 9 | Long-form Social / Thread | Awareness / Education | Builder, Press | LinkedIn, X, blog |
| 10 | Email System | Activation / Retention | All inbound | Transactional + nurture |
| 11 | Press Release / Media Kit | Press | Press, Analyst | PR wire + media room |
| 12 | Podcast / Video Episode Lockup | Awareness | Builder, Press | Podcast, YouTube, X Spaces |
| 13 | Conference / Event Booth | Awareness / Acquisition | Builder, Buyer | NeurIPS, GTC, re:Invent, KubeCon |
| 14 | Web / Landing Page | Acquisition | All | boids.so |
| 15 | Documentation Site & API Reference | Activation | Builder, Developer | docs.boids.so |
| 16 | In-Product UI System | Activation / Retention | Builder, Operator | App UI |
| 17 | Status Page & Trust Center | Retention / Trust | All | status / trust subdomains |
| 18 | App Store / Play Store Listing | Acquisition | Builder | iOS / Android stores |
| 19 | GitHub Org Profile & OSS README | Awareness / Adoption | Developer | github.com/boids-* |
| 20 | Changelog / Release Notes | Retention | Builder, Operator | Web + RSS |
| 21 | CLI / Terminal Output | Activation | Developer, Builder | `boids` CLI |
| 22 | Voiceover / Narration Script | Awareness | All | Brand video TTS |
| 23 | Careers Page & Recruiting Deck | Talent | Candidates | careers.boids.so |
| 24 | Incident / Postmortem / Security Advisory | Trust / Governance | All | Web + email |
| 25 | Co-Marketing / Partner Lockup | Ecosystem | Partners | Joint assets |
| 26 | Swag / Merch System | Advocacy | Community | Apparel, stickers, hardware |

---

# A. Sales & Conversion

### 1. Pitch / Sales Deck (1920×1080)

**When:** Investor pitch, sales deck, category leadership deck.

**Layout:** Document Bento. 55/45 left-right column split. Header band full-width above columns. ≥ 40% whitespace.

**Visual spec:**
- Builder Ink palette: Bone background, Ink text, Phosphor single accent flat
- Eyebrow pill above every H1/H2: Cabinet Grotesk 10px, Phosphor @ 18%, uppercase tracking 0.2em
- All cards: Double-Bezel (Bone-200 outer, Bone inner, 24/18px concentric radii)
- Display: PP Editorial New italic Ultralight, -0.03em tracking
- Data: JetBrains Mono, tabular-nums
- 3% grain overlay mandatory
- 5% top-left blank zone (no logo drawn)
- `Privileged&Confidential` bottom-right (optional, internal/NDA decks only), 10px JetBrains Mono, Ink @ 35%
- Page number top-right, JetBrains Mono, Stone

**Content rules:**
- One core insight per slide
- Footer source citation on data slides: 9px JetBrains Mono, Stone, left-aligned
- No two H1s on one slide

**Default flow:** cover → positioning → category map → product → credit loop → ICP tiers → competitive set → traction → ask / CTA.

---

### 2. One-Pager / Solution Brief (A4 / US Letter)

**When:** AE-led sales conversation, executive briefing, partner intro, leave-behind after a meeting.

**Layout:** Single-page Document Bento. Header band (logo zone + headline) + 2-column body + footer strip. Print-safe margins (15mm).

**Visual spec:**
- Bone background; one Phosphor accent only on a single CTA chip or KPI block
- Double-Bezel for the headline card and the proof-points card
- PP Editorial New italic for the headline; Cabinet Grotesk for section labels; Geist body
- Body type 10–11pt; line-height 1.45; 65ch column max
- 3% grain overlay; print colour profile FOGRA39

**Content rules (5 blocks, top-to-bottom):**
1. Eyebrow + headline (canonical hero line or audience variant)
2. The job to be done — one sentence in builder voice
3. How it works — three L2-1 verbs (build · run · publish) with one line each
4. Proof — 2–3 metrics in JetBrains Mono tabular-nums (named source under each)
5. CTA — single Phosphor chip with URL + sales contact

**Forbidden:** stock icons, three-feature equal-card row, gradient backgrounds, photography of people.

---

### 3. Customer Case Study

**When:** Public customer story for boids.so/customers, sales enablement, analyst evidence.

**Layout:** Editorial Split. Hero band (customer logo lockup + outcome metric) → narrative body → results card → quote card → CTA.

**Visual spec:**
- Bone canvas; alternating Bone / Onyx section bands for rhythm
- Customer logo rendered Ink-on-Bone or Bone-on-Onyx — never coloured
- Phosphor only on the outcome metric and the final CTA
- Double-Bezel for the results card and the pull-quote card
- Headshot policy: monochrome Ink duotone only, no full-colour stock-style photography

**Content rules (Stripe / Vercel pattern):**
- Hero: customer name + one-line outcome ("Reduced agent build time from 3 weeks to 2 days")
- Context: 2–3 sentences in Stone-coloured small caps eyebrow ("INDUSTRY · TEAM SIZE · USE CASE")
- Narrative: Pain → Problem → Reveal → Proof → Outcome → CTA (six-beat arc)
- Results card: 3 KPIs in JetBrains Mono tabular-nums with named source line
- Quote: PP Editorial New italic, ≤ 18 words, attributed with role + company
- Approval line in footer: "Reviewed by [Customer Name], [Date]"

**Forbidden:** unsourced metrics, generic adjectives ("transformative", "game-changer"), stock-photo office scenes.

---

### 4. RFP / Procurement / Trust Pack

**When:** Enterprise RFP response, security questionnaire reply, procurement-driven sales motion. Cover sheets and section dividers for SOC 2 / ISO 27001 / DPA / MSA documents.

**Layout:** Document Bento, formal register. Cover page + table of contents + section dividers + answer pages.

**Visual spec:**
- Cover: Ink full-bleed background with Bone wordmark; Phosphor single hairline rule under wordmark
- Section dividers: Bone canvas; Cabinet Grotesk Extrabold section title in Ink; eyebrow tag in Stone
- Answer pages: Bone canvas, Geist body 10pt, JetBrains Mono for IDs / control codes / hashes
- All compliance frameworks listed in a JetBrains Mono table (e.g. `SOC2-TYPE-II`, `ISO-27001`, `GDPR`)
- Page numbers and document ID in footer (`BOIDS-RFP-YYYYMMDD-NNN`)

**Content rules:**
- Plain-English answers first; technical detail in collapsible appendix references
- Every control answer cites a primary source (policy doc, audit report) with date
- No marketing copy in the body of a control response
- Confidentiality watermark `Privileged&Confidential` is **on by default** for this surface

**Forbidden:** sales taglines on cover, Phosphor used decoratively, unsourced compliance claims.

---

### 5. Investor Update / Board Deck

**When:** Monthly / quarterly investor update; board meeting deck; LP letter cover.

**Layout:** Document Bento. Single-column narrative for the email body; 1920×1080 deck for the appendix.

**Visual spec (deck):**
- Bone canvas; Ink text; Phosphor used only on the headline KPI of the period
- Cover: PP Editorial New italic period label ("Q2 2026") + one-line theme
- Section dividers: KPIs · Wins · Misses · Asks · Roadmap
- All metrics in JetBrains Mono tabular-nums with prior-period delta in Stone
- 5% top-left blank logo zone; page number top-right; `Privileged&Confidential` mandatory bottom-right

**Content rules:**
- Lead with the headline KPI and its delta
- KPI table covers ARR, NRR, gross margin, burn, runway, headcount — every line cites the source system
- Wins / misses balanced (no spin); misses include root cause and the change in plan
- Asks block: 1–3 specific, named asks (intro to X, hire for Y)
- Footer: cap-table snapshot date + next update date

**Forbidden:** vanity metrics without context, hero photography, narrative without numbers.

---

# B. Marketing & Demand Generation

### 6. Single Marketing Image

**When:** LinkedIn post image, X card, ad creative, blog hero.

**Layout:** Asymmetric Bento. Dense but breathing — one primary message, one visual metaphor, one CTA.

**Visual spec:**
- Builder Ink palette
- One Phosphor accent element only (CTA button, key metric, or active workflow node)
- Double-Bezel card for the core message block
- PP Editorial New italic for the headline
- No more than 3 colours in play (Bone, Ink, Phosphor)
- 3% grain overlay
- No photography, no icons-as-decoration, no gradients

**Content rules:**
- One headline (canonical hero line or variant)
- One support line
- One visual metaphor (abstract: workflow graph, permission node, builder tool)
- One CTA

---

### 7. Performance Ad / Paid Social

**When:** Paid social on LinkedIn, X, Reddit, Meta; YouTube pre-roll; programmatic display.

**Required formats:**
| Format | Aspect | Use |
|---|---|---|
| Static feed | 1:1, 4:5 | LinkedIn, X, IG feed |
| Story / Reel | 9:16 | LinkedIn Stories, TikTok, IG Reels, Shorts |
| Wide display | 16:9 | YouTube, programmatic |
| Square video | 1:1 | LinkedIn, X timeline |

**Visual spec:**
- Bone canvas (or Onyx for inverted-night variant only)
- Phosphor reserved for the CTA chip and one KPI; never for body type
- Headline ≥ 56pt at 1080px output; auto-fail if headline cannot be read at 200px tall thumbnail
- Logo lockup bottom-left in Ink wordmark; 8% safe-zone all sides
- Motion (video formats): single Phosphor sweep across the build → run → publish line, max 2.5s; no kinetic typography flourishes; no purple-blue gradient backgrounds

**Content rules:**
- Headline = 1 audience-specific hero line variant (≤ 9 words)
- Support line = 1 sentence with a number ("11.5k stars · 92% Locomo")
- CTA = single L2-1 verb chip ("Build →" / "Run →" / "Publish →")
- A/B variants tag in metadata only, never on the creative surface

**Forbidden:** "Click here", "Learn more" CTAs, before/after split-screens, AI-generated stock people, urgency gimmicks ("Limited time"), all-caps body.

---

### 8. Out-of-Home / Billboard

**When:** US-101 / SF Bay billboard, NYC subway / OOH, airport (SFO, JFK, SJC), conference-adjacent transit takeover.

**Layout:** Single thought, single accent, no body copy. Ratio variants:
- Highway billboard: 14:48 (US standard) — readable at 600ft / 4 seconds
- Transit / subway: 1:1 or 4:1 vertical/horizontal — readable at 6ft / 6 seconds
- Airport panel: 16:9 backlit — readable at 30ft / 4 seconds

**Visual spec:**
- Bone canvas OR Ink full-bleed (no third option)
- ONE word or ONE short clause in PP Editorial New italic at maximum size — vertical clearance ≥ 70% of canvas
- Wordmark only in lower-right corner at 8% canvas height
- Phosphor used as 1px hairline rule under the headline OR as a single underline under one word
- No grain overlay (print degrades grain)
- No body copy, no URL, no QR code (a strong OOH does not need one)

**Content rules:**
- Maximum 7 words on the surface
- Drawn from canonical hero set or a permitted audience variant
- Co-located placements within 10mi: distinct headlines, identical lockup
- Approved one-word stamps: *Build.* · *Run.* · *Publish.* · *Persistent.* · *Orchestrated.*

**Forbidden:** product screenshots, photography, multiple accent colours, gradient skies, "scan to learn more".

---

### 9. Long-form Social Post / Thread

**When:** LinkedIn article, X / Twitter thread, blog post, newsletter.

**Layout:** Editorial Split or single-column narrative. Max 65ch body width.

**Content rules:**
- Hero line as title (canonical or audience variant)
- Six-beat narrative arc (Pain → Problem → Reveal → Proof → Outcome → CTA)
- Layer-verb discipline throughout: L2-1 verbs only
- ICP-voice matched per audience tier
- No forbidden phrasings
- Systems-thinking framing: loops, layers, connections
- Measurable ambition: back every claim with named modules or benchmark data

---

### 10. Email System (Transactional + Marketing)

**When:** All outbound + system-generated email. Three sub-templates: **transactional**, **lifecycle nurture**, **broadcast newsletter**.

**Layout:** Single-column 600px body. Header band + content + footer band. No floating images.

**Visual spec:**
- Bone email canvas (#F2EDE4); Ink text; outer email-client gutter Bone-200
- Header band: 64px tall, Ink fill, Bone wordmark left, period label right (transactional / nurture only)
- Body: Geist 16px regular for paragraphs; Cabinet Grotesk 14px for inline labels; JetBrains Mono for data lines (account ID, run ID, credit balance)
- Single Phosphor CTA chip per email — never a Phosphor wash, never two CTAs
- Footer: legal address, unsubscribe (one click), trust-center link, period release tag

**Content rules — transactional:**
- One purpose per email (run completed, credit applied, key issued)
- Subject line: noun-phrase + ID, no emoji ("Run completed · run_8af2…")
- Body: facts in JetBrains Mono table at top; plain-English paragraph below; CTA last
- Receipts include period release tag: `release/YYYY-MM-DD-<slug>`

**Content rules — nurture / broadcast:**
- Pain → Reveal → Proof → CTA in 3 short paragraphs (≤ 180 words total)
- Single hero line drawn from canonical set
- One Phosphor CTA; never a "P.S." sales tactic; never urgency gimmicks
- Quiet hours: never send between 22:00–07:00 recipient local time

**Forbidden:** image-only emails, dark-pattern unsub flows, "marked as urgent" subject prefixes, full-bleed Phosphor backgrounds.

---

### 11. Press Release / Media Kit

**When:** Funding announcement, product launch, customer milestone, leadership hire, partnership. Full media kit at `boids.so/press`.

**Press-release layout:**
- Plain Markdown / wire format with a header block: dateline city · ISO date · embargo line
- Cabinet Grotesk Extrabold headline, sentence case, ≤ 12 words
- Standfirst paragraph ≤ 50 words
- Body in inverted pyramid; quotes in PP Editorial New italic when typeset
- Boilerplate: 4 sentences max, links to nevamind.ai and boids.so

**Media kit (web) layout:**
- Editorial Split. Sections: Logos & Lockups · Brand Colours · Founder Bios & Headshots · Product Screenshots · Fact Sheet · Press Contact
- Headshots: Ink duotone only, no full-colour
- Logo downloads: SVG + PNG @ 1× / 2× / 3×, on Ink, Bone, Onyx — never on busy photography
- Fact sheet block in JetBrains Mono table

**Content rules:**
- All metrics cite source + date
- Founder titles match the canonical org chart in `references/brand-quick-reference.md`
- "About Boids" boilerplate identical across all releases for the period — bumped only on a tagged release
- Quotes ≤ 30 words; attributed with full name + role

**Forbidden:** breathless adjectives ("revolutionary", "cutting-edge"), unsourced rankings, AI-generated headshots in the kit, stock metaphor imagery (handshakes, rockets, globes).

---

### 12. Podcast / Video Episode Lockup

**When:** Hosting, sponsoring, or appearing on podcasts and video shows (Latent Space, Lex, No Priors, etc.). Includes YouTube thumbnails, X-Spaces banners, episode title cards, lower-thirds.

**Layout:**
- 16:9 episode card / YouTube thumbnail: Bone canvas, guest portrait left (Ink duotone), title block right
- 1:1 social cut-down: title only, no portrait
- Lower-third: Ink bar, Bone wordmark left, guest name + title in Cabinet Grotesk

**Visual spec:**
- Guest portrait: monochrome Ink duotone, head-and-shoulders, no background imagery
- Title: PP Editorial New italic, ≤ 7 words
- Episode number in JetBrains Mono ("EP 042") top-right, Stone colour
- Phosphor: a single hairline rule under the episode number — never on the portrait
- 3% grain overlay on Bone areas; never on the duotone portrait

**Content rules:**
- Title pattern: `[Guest first name] · [one-noun topic]` ("Andrej · Reasoning")
- No clickbait punctuation ("?!?", "🤯", "WAIT")
- Sponsor mentions land in chapter markers, not in the title card

**Forbidden:** rainbow chapter dividers, AI-generated guest faces, neon highlight outlines on portraits, drop-shadowed text.

---

### 13. Conference / Event Booth

**When:** Booth presence at NeurIPS, GTC, AWS re:Invent, KubeCon, AI Engineer Summit, Web Summit, YC demo days. Includes hosted side-events (dinners, hackathons).

**Surface set:**
| Surface | Spec |
|---|---|
| Booth back-wall | 3×3m or 3×6m printed Bone canvas; one PP Editorial New italic statement at human scale |
| Side panels | Three Double-Bezel cards: BUILD · RUN · PUBLISH, each with one demo entry-point |
| Demo station | Onyx counter, JetBrains Mono terminal display, Phosphor CTA chip on screen |
| Lanyard / badge | Bone background, Ink wordmark, JetBrains Mono attendee handle |
| Hand-out | One-Pager (see playbook 2) |
| Side-event invite | A6 card, Ink fill, Bone wordmark, Phosphor `RSVP →` chip |

**Visual spec:**
- Bone-dominant booth; Onyx accent only on the demo station
- ONE Phosphor element visible in any sightline (CTA chip on screen) — never decorative on walls
- No motion-graphic walls, no LED-strip Phosphor, no stage smoke
- Floor decals: Stone hairline rules pointing to BUILD / RUN / PUBLISH cards

**Content rules:**
- Wall statement = canonical hero line OR one-word stamp (*Build.* · *Run.* · *Publish.*)
- Demo run-time ≤ 90 seconds, ending on a published agent
- Booth team script opens with "Are you building agents?" — never "Have you heard of Boids?"
- Lead capture: badge scan + opt-in only; never auto-subscribe

**Forbidden:** logo wall of customers without permission, swag pile dominating sightlines, branded foam fingers, mascot costumes, plastic giveaways.

---

# C. Web, Product & Developer

### 14. Web / Landing Page

**When:** boids.so homepage, product page, feature page.

**Layout:** Asymmetric Bento + Editorial Split. Hero section full-bleed Bone. Sections alternate Bone / Onyx for contrast rhythm.

**Visual spec:**
- Builder Ink palette
- Double-Bezel cards for every feature block
- Phosphor only on the primary CTA button (flat fill, never gradient)
- Eyebrow tags on every section header
- Grain overlay on hero and footer only
- Typography: PP Editorial New italic display, Cabinet Grotesk titles, Geist body, JetBrains Mono data

**Content rules:**
- Hero: canonical headline + support line + one CTA
- Feature sections: ICP-specific (builder, operator, developer)
- Social proof: benchmark metrics with named source
- Credit loop explained in plain language
- Navigation: no more than 5 items

---

### 15. Documentation Site & API Reference

**When:** docs.boids.so. Stripe / Vercel-tier developer documentation: guides, API reference, recipes, SDK pages.

**Layout:** Document Bento. Three-pane: left nav (240px) · centre content (720px / 65ch body) · right TOC (200px).

**Visual spec:**
- Bone canvas in light mode; Onyx in dark mode (parity required at launch)
- Body type: Geist 16px regular, line-height 1.65
- Code blocks: Onyx fill, Bone-200 hairline border, JetBrains Mono 14px, syntax theme uses Phosphor for keywords + Stone for comments — no rainbow tokens
- Inline code: JetBrains Mono 90% size, Bone-200 background pill, no monospace stretching
- Headings: Cabinet Grotesk Extrabold; H1 size only on landing pages of each section
- Callouts: Double-Bezel cards with eyebrow tag (`NOTE` · `WARNING` · `DEPRECATED`)
- API reference: 50/50 split — prose left, request/response example right, sticky scroll
- Search: keyboard `⌘K`, JetBrains Mono input

**Content rules:**
- Every page opens with a one-sentence summary in PP Editorial New italic
- Every code sample is runnable as written (no `…` placeholders)
- Every API endpoint shows: `METHOD /path`, parameters table, request example, response example, error codes
- "Last updated" timestamp + git short-sha in footer of every page
- L2-1 verb discipline: docs verbs are *build · run · publish · deploy · authenticate · authorize · rank · credit*

**Forbidden:** generic AI-doc tropes ("Welcome! 🚀"), animated hero illustrations, autoplay videos, gated reference docs, Inter / Roboto for body, gradient code-block backgrounds.

---

### 16. In-Product UI System

**When:** Authoring inside the Boids product surface — empty states, loading states, error states, onboarding modals, success toasts, pricing & billing UI.

**Layout:** Application chrome on Onyx in dark mode (default for builders), Bone in light mode. Side-rail 64px collapsed / 240px expanded. Workbench panes use Double-Bezel.

**Visual spec:**
- Surfaces: Onyx (chrome), Ink-elevated (modals), Bone-elevated (light-mode cards) — never #000 or #FFF
- Phosphor used for: active step in BUILD → RUN → PUBLISH stepper, primary CTA, run-success state — never error, never decorative
- Error state: Terracotta hairline + JetBrains Mono error code (`ERR_AGENT_TIMEOUT`)
- Pending state: Ochre dot + JetBrains Mono progress (`Step 2 / 4`)
- Toasts: Double-Bezel pill, top-right, auto-dismiss 6s, never stack > 3
- Empty states: PP Editorial New italic line + one Phosphor CTA — never an illustration of a person / robot / brain

**Content rules:**
- Microcopy verbs are L2-1 only; never "Click here" / "Get started" / "Try it now"
- Error messages name the failed step + suggest the next action ("Step 2 / 4 timed out · Re-run from Build")
- Onboarding ends on a published agent within 5 minutes of first sign-in
- Pricing tiers labelled by capability, not by adjective ("Builder" · "Studio" · "Enterprise" — never "Pro" / "Premium" / "Unlimited")

**Forbidden:** gamification badges, confetti, dark-pattern paywalls, AI-mascot characters, gradient progress bars, modal stacking, "Are you sure?" confirmations on reversible actions.

---

### 17. Status Page & Trust Center

**When:** status.boids.so · trust.boids.so. Public uptime, incident history, security posture, compliance attestations, sub-processor list.

**Layout (status):** Single-column timeline. Top: 90-day uptime grid (90 squares); Below: incident timeline; Right rail: subscribe + RSS.

**Layout (trust):** Document Bento. Sections: Compliance · Architecture · Data Residency · Sub-processors · Vulnerability Disclosure · DPA & MSA links.

**Visual spec:**
- Bone canvas, no grain (clarity > texture on operational surfaces)
- Uptime squares: Phosphor (operational) · Ochre (degraded) · Terracotta (outage) — flat fill, no gradient
- Incident entries: JetBrains Mono timestamp, Cabinet Grotesk title, Geist body, status pills using the same colour set
- Compliance badges: Ink wordmark on Bone-200 chip — never the vendor's full-colour SOC2 / ISO logos
- Sub-processor table: JetBrains Mono, sortable, with country flag absent (text country code only)

**Content rules:**
- Real-time status reflects probe data, not marketing
- Incident posts include: detection time, customer impact, current status, next update ETA — updated every 30 minutes during an active incident
- Trust center never claims certifications not held; expired certs are removed within 24h
- Subscribe options: email, RSS, Slack webhook, Atom feed — never SMS-only

**Forbidden:** "All systems operational" green-wash when components are degraded, marketing copy on incident pages, hidden incident archives, certification badges as decoration.

---

### 18. App Store / Play Store Listing

**When:** iOS App Store, Google Play, Mac App Store listing. Includes screenshots, preview video, store description.

**Layout (screenshots):** 6 frames, each Bone or Onyx canvas with a single Cabinet Grotesk caption + one product screenshot in a Double-Bezel device frame.

**Visual spec:**
- App icon: Ink fill rounded square, Phosphor glyph centred, no gradient, no inner shadow — pixel-perfect at 1024px and 16px
- Screenshots: caption above device frame; caption ≤ 6 words, sentence case, PP Editorial New italic for one keyword
- Preview video: 15s, opens on a build → run → publish in 3 cuts, no voiceover, captions in Cabinet Grotesk
- Store description: opens with the canonical hero line, then 5 short paragraphs (Pain · Problem · Reveal · Proof · CTA)

**Content rules:**
- Keyword field uses functional terms only (`agent`, `workflow`, `automation`, `orchestration`) — never competitor names
- "What's New" notes mirror the public Changelog (playbook 20) verbatim
- Screenshots show real product UI captured at the latest period release tag — never mocks
- Privacy nutrition label: every data type declared, even if optional

**Forbidden:** "#1 AI app" claims, fake 5-star testimonials in screenshots, gradient store-art backgrounds, AI-generated mascots in the icon.

---

### 19. GitHub Org Profile & Open-Source README

**When:** `github.com/boids-*` org profile · `README.md` of any open-source repo published under the Boids name (skills, SDKs, CLIs, examples).

**Org profile layout:**
- Bone-coloured header banner (1280×640) with PP Editorial New italic statement + Phosphor hairline
- Pinned repos: 6 max, ordered by usage relevance not stars
- Profile README: short manifesto (≤ 120 words) + repo index table

**README layout (per repo):**
1. Header: shields.io badges (Apache 2.0 / version / CI / coverage) — black-on-Bone style only, no rainbow
2. Hero: project name in `# H1`, one-line summary in italic
3. Animated demo (optional): asciinema cast, ≤ 30 seconds, JetBrains Mono terminal
4. Quick start: 3 commands max, runnable
5. Documentation link to docs.boids.so
6. Contributing link to `CONTRIBUTING.md`
7. License + Trademarks section linking `LICENSE` and `TRADEMARKS.md`

**Visual spec:**
- All embedded images on Bone canvas, dark-mode variant on Onyx with `<picture>` tag
- Code blocks use the `bash` / `ts` / `py` fence honestly; no `language: ai` placeholder
- Tables minimal — never Markdown tables of features when prose works

**Content rules:**
- README opens with what the project IS (one sentence) — not why it exists
- Every quick-start command tested in CI on the period release tag
- Comparison tables to other projects: only with permission and a fair-use methodology link
- Issues / PR templates carry the same voice as docs (L2-1 verbs)

**Forbidden:** "Awesome" emoji headers, gradient banner art, "Made with ❤️ by …" footers, broken demo GIFs, vanity star-history charts as the README hero.

---

### 20. Changelog / Release Notes

**When:** Public changelog at boids.so/changelog · in-product "What's new" panel · email-broadcast monthly digest · GitHub releases entry.

**Layout:** Reverse-chronological timeline. Each entry = a Double-Bezel card with date, period release tag, and category label.

**Visual spec:**
- Bone canvas; entries stack in a single 720px column
- Date: JetBrains Mono `YYYY-MM-DD`, Stone colour
- Period release tag: JetBrains Mono pill (`release/2026-05-20-builder-ink-rebuild`)
- Category label: Cabinet Grotesk eyebrow, Phosphor on Ink chip — categories are `Added` · `Changed` · `Fixed` · `Deprecated` · `Removed` · `Security`
- Inline product visuals: short looping mp4 ≤ 4s, Bone background, no captions overlay

**Content rules:**
- Entries written in the perfect tense from the user's perspective ("You can now publish agents to private workspaces")
- Every entry credits the engineer or team in a JetBrains Mono footer line
- Breaking changes lead with a `BREAKING` Terracotta chip and a migration link
- Monthly digest email = grouped categories of the period; never marketing prose

**Forbidden:** "Various improvements and bug fixes" filler entries, marketing CTAs inside changelog entries, animated hero illustrations, emoji headers.

---

### 21. CLI / Terminal Output

**When:** `boids` CLI — `init`, `build`, `run`, `publish`, `doctor`, `whoami`, error states. Includes `npx boids …` first-run experience.

**Layout:** Onyx terminal background; Bone foreground text; Phosphor accent on success markers and the final CTA line. Width target: 80 cols; gracefully degrades to 60.

**Visual spec:**
- Banner (first-run only): ASCII wordmark in Bone, one Phosphor underline, version string in JetBrains Mono — banner ≤ 6 lines, suppressed in CI / non-TTY
- Step output: `▸ Step 1 / 4 · Build` — Phosphor caret, Cabinet Grotesk-equivalent uppercase pseudo-tracking via SMALL CAPS
- Success: `✓` in Phosphor; pending: `…` in Ochre; error: `✗` in Terracotta + error code on the next line
- Tables (e.g. `boids credits ls`): box-drawing characters U+2500 family, JetBrains Mono alignment, tabular numbers
- Colour: respects `NO_COLOR`, `--no-color`, and CI env detection — falls back to glyph-only output

**Content rules:**
- Every command exits with a meaningful code; documented in `boids help <cmd>`
- Errors name the failed step, the cause, and the next command to run (mirror in-product UI rule)
- Never auto-update silently; updates announce on `boids doctor` and require explicit `boids upgrade`
- Telemetry off by default; opt-in via `boids telemetry on` with an explicit confirmation prompt

**Forbidden:** rainbow gradients, ASCII art beyond the wordmark, emoji success markers, blocking spinners on non-TTY, banner output in scripted use.

---

# D. Video & Voice

### 22. Voiceover / Narration Script

**When:** TTS narration for a brand video, product demo, or explainer.

**Voice:** Builder confidence. Precise. Empathetic. Measured ambition. No hype.

**Register:** Professional peer — speaks to another builder, not a consumer.

**Content rules:**
- Open with the canonical hero line
- Use L2-1 verbs exclusively
- Describe the workflow: BUILD → DEPLOY → RUN → RANK → CREDIT
- Anchor to MemU: agents remember across sessions
- Close with a specific outcome (number, result, ICP signal)
- Never: magic framing, one-click language, consumer-AI tone

**TTS defaults:** English, Geist-compatible pacing (160–180 wpm), pause at each beat transition.

---

# E. Talent & Culture

### 23. Careers Page & Recruiting Deck

**When:** careers.boids.so · job-description headers · recruiting-loop deck · offer-letter cover. Talent is brand.

**Careers page layout:** Editorial Split. Manifesto block (≤ 200 words) → roles table → benefits & comp posture → "How we hire" loop → application CTA.

**Visual spec:**
- Bone canvas; one Phosphor accent on the application CTA only
- Team photos: Ink duotone group portraits, candid not posed; no glass office stock
- Role cards in Document Bento; each card: title · location · band · team · `Apply →` Phosphor chip
- "How we hire" rendered as a 5-step Double-Bezel diagram

**Recruiting deck layout (1920×1080):**
- Cover · why this company · the work · the team · comp posture · loop · ask
- Comp posture page: salary bands in JetBrains Mono tabular-nums + named geographic policy
- Loop page: each stage time-boxed; no surprise stages

**Content rules:**
- Job descriptions open with the outcome of the role, not a list of requirements
- "Required" vs "Bonus" must be true — not aspirational
- Comp ranges published in every role card (no "DOE")
- Diversity / equal-opportunity statement: factual, no boilerplate
- Offer letter cover carries the period release tag in the footer

**Forbidden:** "rockstar" / "ninja" / "10x" language, foosball / kombucha tropes, ping-pong photography, AI-generated team headshots, ranges that span > 30%.

---

# F. Governance & Crisis

### 24. Incident / Postmortem / Security Advisory

**When:** Active outage updates · public postmortem after an incident · CVE / security advisory · vendor security incident notification.

**Layout (incident update during outage):** Status-page entry (playbook 17) + email body in single column, plain Markdown.

**Layout (postmortem):** Document Bento. Sections: Summary · Customer impact · Timeline · Root cause · What we are changing · Acknowledgements.

**Layout (security advisory):** Cloudflare-style web post + CVE-format email. CVE ID and CVSS score in JetBrains Mono header.

**Visual spec:**
- Bone canvas; no Phosphor, no decorative accents — operational surfaces stay neutral
- Timestamps in JetBrains Mono, all UTC, with local time in parentheses
- Severity pill: Phosphor (resolved) · Ochre (degraded) · Terracotta (active) — same token set as status page

**Content rules:**
- Incident updates: every 30 minutes during active impact, even if "no new information"
- Postmortem published within 5 business days of resolution
- Root cause stated in plain language; no blame language; never "human error" without systemic context
- "What we are changing" lists ≥ 1 named, dated change with an owner
- Security advisory: CVE + CVSS + affected versions + fixed-in version + workaround + credit to reporter
- Confidentiality watermark NEVER applied to public incident or advisory pages

**Forbidden:** spin language ("minor inconvenience", "limited impact" without numbers), silent edits to past incident timelines, embargo extensions without reporter consent, marketing CTAs inside an advisory.

---

# G. Community & Ecosystem

### 25. Co-Marketing / Partner Lockup

**When:** Joint announcement, integration launch, co-hosted event, hyperscaler / model-provider / framework partnership.

**Lockup spec:**
- Horizontal pairing: `[Boids wordmark] × [Partner mark]` separated by a Stone-coloured `×` glyph at 60% wordmark x-height
- Vertical pairing: `[Boids wordmark]` over Stone hairline rule over `[Partner mark]`
- Clearspace: each mark gets a clearspace ≥ 1 cap-height of its own wordmark
- Backgrounds: Bone or Ink only — never the partner's brand colour
- Phosphor never used in a co-mark; partner accent colour never used either — both marks neutralised

**Visual spec:**
- Co-branded one-pager, web banner, social card all reuse the relevant single-brand playbook (2, 6, 7) with the lockup substituting for the wordmark
- Joint case study uses playbook 3 with both customer and partner logos in monochrome

**Content rules:**
- Both parties review before publication; approval line in the footer (`Reviewed by [Boids] [Partner] · [Date]`)
- Press release headline does not claim category leadership unless the partnership earns it
- Integration claims tied to a named, public release tag on both sides
- Trademark line in the footer cites both: `Boids is a trademark of Nevamind-AI. [Partner] is a trademark of [Owner].`

**Forbidden:** partner mark in Phosphor, partner-brand-colour wash on co-marketing surfaces, ghost-mark usage without permission, "powered by" claims when the integration is reciprocal.

---

### 26. Swag / Merch System

**When:** Conference giveaways, employee onboarding kit, customer-loyalty drops, hackathon prizes, holiday gifts.

**Catalogue (canonical SKUs):**
| Item | Spec |
|---|---|
| T-shirt | Bone or Ink heavyweight cotton; chest wordmark Ink-on-Bone or Bone-on-Ink; back: one verb stamp (*Build.* / *Run.* / *Publish.*) |
| Hoodie | Ink heavyweight; chest wordmark only; Phosphor inner-hood lining permitted (single accent rule honoured) |
| Cap | Bone or Ink; Cabinet Grotesk wordmark only |
| Sticker pack | 5 stickers: wordmark · *Build.* · *Run.* · *Publish.* · the brand glyph — die-cut on Bone vinyl |
| Notebook | Bone cover; Cabinet Grotesk wordmark debossed; JetBrains Mono dot-grid pages |
| Mechanical keyboard cap | Onyx caps, single Phosphor `⏎` Enter key (one-accent rule) |
| Tote | Bone canvas; Ink wordmark; reinforced strap |

**Visual spec:**
- One accent per piece — Phosphor reserved for ONE element across the entire item
- Pantone calls: Ink → Pantone Black 6 C; Bone → Pantone 7527 C; Phosphor → Pantone 2297 C
- Wordmark embroidered or screen-printed at proportion: chest mark = 8% garment width; back stamp = 35% garment width
- Care labels include period release tag for collectible drops

**Content rules:**
- Verb stamps are the only permitted back-of-shirt content — never slogans, never URLs
- Hackathon prizes: SKU lockup to event date in care label, not on the visible surface
- No partner co-branded swag without playbook 25 lockup
- Sustainable suppliers preferred; vendor list maintained internally and audited annually

**Forbidden:** rainbow Pride colourways without governance approval, full-bleed Phosphor garments, phrases like "I built X with Boids", dated event-year prints (creates landfill), emoji prints, AI-generated graphics on apparel.

---

## Visual Asset Amendment (all playbooks)

Every visual asset generated under any playbook must apply the Builder Ink rules:
- Builder Ink palette (Ink + Bone + Phosphor flat) — one accent per surface
- Builder Stack typography (PP Editorial New + Cabinet Grotesk + Geist + JetBrains Mono)
- Double-Bezel surface construction
- 3% grain overlay (omit on operational, OOH-print, and duotone-portrait surfaces)
- No teal, no navy, no azure, no purple-to-blue gradient
- No banned fonts (Inter, Roboto, Open Sans, Helvetica, SF Pro, Source Sans Pro, Space Grotesk)
- No #000 / #FFF — Ink and Bone only

When a playbook above conflicts with the quick reference, the **quick reference wins**; raise an issue rather than override silently.
