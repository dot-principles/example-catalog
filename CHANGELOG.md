# Changelog

All notable changes to the `example-catalog` will be documented here.

The format follows [Keep a Changelog](https://keepachangelog.com/).

---

## [Unreleased]

### Added

- **PTAC-NAVIGABLE-DIRS DRY rule** — README.md and INDEX.md now have explicit, non-overlapping roles: README = prose purpose only; INDEX = structured file list only. Violation added to `.context-audit.md` and `ptac.instructions.md`.
- **README.md + INDEX.md** added to `groups/`, `principles/`, `principles/ptac/`, `.github/instructions/` per `PTAC-NAVIGABLE-DIRS`.

---

## [v0.11.0] — 2026-04-22

### Added

- Initial release of the `example-catalog` — demonstrates how to build a custom extra-catalog for the [dot-principles](https://github.com/dot-principles/dot-principles) system using the `ptac` (Plain-Text-as-Code) namespace.
- Five PTAC principles: `PTAC-PLAIN-TEXT-FIRST`, `PTAC-COMPOSABLE-FILES`, `PTAC-LEAN-CONTENT`, `PTAC-NAVIGABLE-DIRS`, `PTAC-NO-GENERATED-BLOBS`.
- `@ptac` group for activating all PTAC principles at once.
- LLM context files: `.context-prime.md`, `.context-audit.md`, `.context-inspect.md`, `.context-scout.md`.
- `AGENTS.md`, `.principles`, and Copilot Code Review instruction files.
