# boids-brand

> An Agent Skill that encodes the canonical **Boids** brand system — positioning, voice, Builder Ink visual identity, messaging library, GPT Image 2 prompt preamble, and application playbooks.

[![License: Apache 2.0](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](./LICENSE)
[![Brand](https://img.shields.io/badge/Brand-Boids-0F0F0E?labelColor=F2EDE4)](https://boids.so)

---

## What This Is

`boids-brand` is an **Agent Skill** — a self-contained markdown package that teaches an AI coding agent (Qoder, Claude Code, Cursor, Windsurf, Codex, Trae, etc.) how to produce on-brand Boids artifacts: decks, landing pages, social posts, GPT Image 2 prompts, voiceover scripts, and any other Boids-branded output.

It is the **single source of truth** for the Boids brand system. When this skill is installed, an agent can:

- Apply the canonical positioning (Boids = L2-1 AI agent orchestration platform).
- Use the Builder Ink color palette (Ink `#0F0F0E` + Bone `#F2EDE4` + Phosphor `#C7FF4A`).
- Apply the Builder Stack typography (PP Editorial New + Cabinet Grotesk + Geist + JetBrains Mono).
- Use the Double-Bezel surface system for cards / panels / containers.
- Emit the canonical GPT Image 2 preamble for 1920×1080 deck-grade visuals.
- Author copy from the canonical messaging library (hero lines, narrative arc, taglines).
- Pick the correct playbook for the scenario (pitch deck, single image, social, voiceover, web).
- Self-check output against forbidden positioning, visual, and verb registers before delivery.

## Who This Is For

- **Boids customers and partners** authoring co-branded or Boids-referencing materials.
- **Agencies, contractors, and freelancers** producing Boids assets for Nevamind-AI.
- **Boids internal teams** maintaining brand consistency across decks, web, and social.
- **Open-source community** referencing the brand-as-code methodology.

## Repository Layout

```
boids-brand/
├── SKILL.md                            # Skill entry point
├── references/
│   ├── brand-quick-reference.md        # Positioning + visual identity
│   ├── gpt-image2-preamble.md          # Canonical GPT Image 2 preamble
│   ├── messaging-library.md            # Hero, narrative arc, taglines
│   └── application-playbooks.md        # Five application scenarios
├── scripts/                            # Optional tooling (linters, validators)
├── LICENSE                             # Apache License 2.0
├── NOTICE                              # Attribution + third-party typeface notes
├── TRADEMARKS.md                       # Trademark usage policy
├── CONTRIBUTING.md                     # Contribution guide
├── CHANGELOG.md                        # Git-native versioning guide
├── .gitignore
└── README.md
```

## Installation

`boids-brand` is a flat markdown skill. Install it in the agent skills directory of your IDE / agent:

### As a Git submodule (recommended for teams)

```bash
# From the root of your project repository
git submodule add https://github.com/SeaSea-cc/boids-brand.git .agents/skills/boids-brand
git submodule update --init --recursive
```

### As a clone (lightweight, single-user)

```bash
git clone https://github.com/SeaSea-cc/boids-brand.git .agents/skills/boids-brand
```

### Agent-specific paths

Most agent runtimes will autodiscover skills in one of these directories:

| Agent | Path |
|---|---|
| Qoder | `.agents/skills/boids-brand/` |
| Claude Code | `.claude/skills/boids-brand/` |
| Cursor | `.cursor/skills/boids-brand/` |
| Windsurf | `.windsurf/skills/boids-brand/` |
| Trae | `.trae/skills/boids-brand/` |

If your runtime uses a different convention, symlink or copy the directory accordingly.

## Quick Start

After installation, invoke the skill by asking your agent to perform any Boids-branded authoring task:

- "Draft a Boids investor deck cover slide."
- "Write a LinkedIn post launching Boids credit-loop."
- "Generate a GPT Image 2 prompt for the Boids product map page."
- "Apply the Boids brand to this draft."

The agent will read `SKILL.md`, pick the relevant playbook, and produce output aligned with the canonical positioning, visual identity, and messaging library.

## Versioning

This repository uses **Git-native versioning**. There are no version numbers in filenames. Significant brand-system releases are marked with annotated Git tags following the pattern `release/YYYY-MM-DD-<slug>`.

```bash
git log --oneline                      # Full commit history
git tag -l "release/*"                 # All release tags
git show release/2026-05-20-builder-ink-rebuild
```

See [CHANGELOG.md](./CHANGELOG.md) for details.

## License

The skill content — `SKILL.md`, `references/`, and any tooling under `scripts/` — is licensed under the [Apache License 2.0](./LICENSE).

This is a **permissive** license. You may use, modify, redistribute, and integrate the skill into commercial and non-commercial work, subject to the terms in `LICENSE` and the attribution notices in `NOTICE`.

## Trademarks

The Apache License does **not** grant rights to the **Boids** name, logo, or visual identity — these are trademarks of Nevamind-AI. See [TRADEMARKS.md](./TRADEMARKS.md) for the trademark usage policy.

Short version:

- ✅ You may say "Compatible with Boids", "Built for Boids", etc.
- ✅ You may link to boids.so.
- ✅ You may use this skill to produce Boids-branded output if you are authorized.
- ❌ You may not register a domain or business name containing "Boids".
- ❌ You may not modify the Boids logo.
- ❌ You may not suggest endorsement that doesn't exist.

For approvals: **`brand@nevamind.ai`** (5 business days standard).

## Third-Party Typefaces

The Builder Stack typography references four typefaces. These are **not distributed** with this skill — users must obtain licenses from the respective foundries. See [NOTICE](./NOTICE) for the list and links.

## Contributing

Bug fixes, playbook additions, and tooling contributions are welcome. Positioning, visual identity, and messaging changes require brand-governance review. See [CONTRIBUTING.md](./CONTRIBUTING.md).

## Maintainers

- **Brand owner**: Nevamind-AI — `brand@nevamind.ai`
- **Skill author**: Seasea Brand OS — [seasea.cc](https://seasea.cc)
- **Issues**: [GitHub issues](https://github.com/SeaSea-cc/boids-brand/issues)

---

*Build. Run. Publish.*
