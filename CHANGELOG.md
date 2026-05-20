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
- `release/2026-05-20-builder-ink-rebuild` — initial public Builder Ink release
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
| `release/2026-05-20-builder-ink-rebuild` | Initial public release. Builder Ink palette (Ink + Bone + Phosphor), Builder Stack typography, Double-Bezel surface system, L2-1 positioning (AI agent orchestration platform). |

For changes between commits without an annotated tag, refer to `git log` directly.
