# Contributing to `boids-brand`

Thanks for your interest in improving the Boids brand skill. This document describes how to propose changes.

## Scope

This skill encodes the **canonical Boids brand system** — positioning, messaging, visual identity, GPT Image 2 preamble, and application playbooks. Contributions are welcome in these areas:

- **Bug fixes** — broken links, typos, factual inaccuracies, internal contradictions in the brand rules.
- **Playbook additions** — new application scenarios (e.g., podcast cover, conference booth, email template) that follow existing brand rules.
- **Reference improvements** — clearer phrasing, better tables, additional examples that don't change brand meaning.
- **Tooling** — scripts in `scripts/` that help authors apply the brand system (e.g., color-token validators, prompt linters).

Contributions are **not** welcome in these areas (these require Nevamind-AI brand-governance review):

- **Positioning changes** — category labels, what Boids is / is not, layer relationships.
- **Visual identity changes** — palette colors, typography stack, Double-Bezel construction.
- **Messaging changes** — hero lines, narrative arc, taglines, forbidden phrasings.

If you have a proposal in the second list, open an issue first to discuss with the brand owner before opening a PR.

## How to Contribute

1. **Fork** the repository.
2. **Branch** from `main` using a descriptive name: `feat/<area>`, `fix/<area>`, or `docs/<area>`.
3. **Edit** the relevant files. Keep changes focused — one logical change per PR.
4. **Self-review** your change against the relevant reference file. Run the Pre-flight Self-check in `SKILL.md` if your change touches authoring rules.
5. **Commit** with a clear message:
   - `feat:` for new content
   - `fix:` for corrections
   - `docs:` for documentation-only changes
   - `chore:` for tooling, license, or repository housekeeping
6. **Open a PR** against `main`. Include:
   - What changed and why
   - Which sections / files are affected
   - Any rendered samples or screenshots if visual rules are touched

## Versioning

This repository uses **Git-native versioning** — there are no version numbers in filenames. Significant brand-system releases are marked with annotated Git tags following the pattern `release/YYYY-MM-DD-<slug>` (see `CHANGELOG.md`). PRs that introduce a significant release should propose the tag name in the PR description.

## Code of Conduct

Be professional. Be specific. Disagree with the artifact, not the contributor. No personal attacks, no off-topic discussion.

## License of Contributions

By submitting a contribution to this repository, you agree that your contribution is licensed under the [Apache License 2.0](./LICENSE), the same license as the rest of the work.

## Questions

For brand-governance questions: `brand@nevamind.ai`.
For repository / technical questions: open a GitHub issue.
