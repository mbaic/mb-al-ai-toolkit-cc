# Changelog

## 1.0.0 — 2026-08-19

Claude Code plugin providing skills, slash commands, and an autonomous agent for AL development in Microsoft Dynamics 365 Business Central Per-Tenant Extensions. The repo doubles as its own marketplace (`.claude-plugin/marketplace.json`) so it installs directly from GitHub or a local clone — not published to any third-party marketplace.

- 1 specialist agent: `al-fast` (speed-optimized AL development, `model: haiku`).
- 7 skills, all invocable by description match and — for the four action skills — as slash commands:
  - `al-docs-code`, `al-review-code`, `al-refactor-code`, `al-unit-tests` — invocable as `/al-docs-code` etc. (accept an AL snippet, file path, or folder as `$ARGUMENTS`) or auto-activated when the request matches.
  - `al-best-practices` — `paths`-scoped to `**/*.al`; auto-activates inside AL source.
  - `al-general-dev` — PTE/BC general development principles.
  - `al-sortrecordref` — RecordRef sorting reference (`SKILL.md` + `REFERENCE.md`).
- Converted from the `mb-al-ai-toolkit` VS Code extension. The original VS Code `.prompt.md` files became action skills; the `.instructions.md` files became reference skills.
