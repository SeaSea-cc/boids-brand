# Changelog

This repository uses **Git-native versioning**. There are no version numbers in filenames; every meaningful change is captured in a Git commit, and significant brand-system releases are marked with annotated tags.

## How to View History

### Full commit history of the skill

```bash
git log --oneline
```

### Commit history of a specific file

```bash
git log --oneline --follow SKILL.md
git log --oneline --follow references/brand-quick-reference.md
```

### All release tags

```bash
git tag -l "release/*"
```

### Diff between two tagged releases

```bash
git diff release/2026-01-01-bone-launch..release/2026-05-20-builder-ink-rebuild
```

## Release Tag Convention

Annotated tags follow the pattern:

```
release/YYYY-MM-DD-<short-slug>
```

Examples:
- `release/2026-05-20-builder-ink-rebuild` — initial public Builder Ink release (v1.1, superseded)
- `release/2026-05-20-gtm-surface-expansion` — playbook expansion to 26 scenarios
- `release/2026-05-21-v1.2-expert-agent-platform` — v1.2 brandbook (Expert Agent Platform repositioning + Precision Mono + Ambient Glow visual system)
- `release/YYYY-MM-DD-<change>` — subsequent releases

Each annotated tag carries a short release note in its tag message:

```bash
git tag -a release/YYYY-MM-DD-<slug> -m "Release notes here"
```

To read a tag's message:

```bash
git show release/2026-05-20-builder-ink-rebuild
```

## Significant Releases

The list below is a short curated index. The Git tags themselves are the authoritative record.

| Tag | Summary |
|---|---|
| `release/2026-05-21-v1.2-expert-agent-platform` | **Brandbook v1.2** (confirmed by Nevamind / Boids founder Chen Hong). Major repositioning: Boids is now the **Expert Agent Platform** with two product lines — **Boids Product** (C-end / regular users, integrating into Slack / Telegram / IM tools) and **Boids API / CLI** (developer infrastructure for building agent-powered products). Visual identity replaced: v1.1 "Builder Ink" (Bone + Ink + Phosphor) → **v1.2 "Precision Mono + Ambient Glow"** (Black `#0D0D0D` + White `#FFFFFF` base + radial three-color glow Cyan `#06B6D4` / Violet `#8B5CF6` / Rose `#EC4899`). New three-word motto: **Build. Distribute. Work.** New universal hero: *Build expert agents. Bring them everywhere.* Verb register expanded (build · distribute · publish · call · compose · deploy · ship · earn · compound · bring · integrate · run). All reference files updated; application playbooks include a v1.2 token migration table. |
| `release/2026-05-20-gtm-surface-expansion` | Expanded application playbooks from 5 to 26 scenarios across 7 categories — covers full GTM surface of an AI-infra / AI-agent company on a $1B trajectory (sales, marketing, web/product/developer, video, talent, governance, community). Added application surface matrix. |
| `release/2026-05-20-builder-ink-rebuild` | Initial public release. Builder Ink palette (Ink + Bone + Phosphor), Builder Stack typography, Double-Bezel surface system, L2-1 positioning (AI agent orchestration platform). Superseded by v1.2. |

For changes between commits without an annotated tag, refer to `git log` directly.
