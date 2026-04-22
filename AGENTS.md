# AI Agent Instructions

This is the **example-catalog** repository — a concrete example of an extra-catalog
for the [dot-principles](https://github.com/dot-principles/dot-principles) system,
demonstrating how to extend the built-in catalog with custom namespaces.

The `ptac/` namespace (Plain-Text-as-Code) is the reference example here.

---

## Setup

To work with and validate this catalog locally, vendor it into a project:

```bash
cd /path/to/dot-principles
./install.sh vendor /path/to/your-project --extra-catalog /path/to/example-catalog
```

---

## Documentation — keep these files current

Every change must update the relevant documentation:

| File | When to update |
|------|----------------|
| **`README.md`** | Any change to the catalog structure, namespace content, quick-start steps, or principle IDs/summaries |
| **`CHANGELOG.md`** | Every change — follow the `## [version] - YYYY-MM-DD` format if present, otherwise add a dated entry |

---

## Before any release or significant change

Run `dot-scout` to re-analyse this catalog and refresh generated principle files:

```
/dot-scout
```

Confirm that generated files are committed before tagging a release.

---

## Before merging changes to `principles/` or `groups/`

Run `dot-audit` on the affected paths:

```
/dot-audit principles/<changed-dir>
```

All findings must be resolved or explicitly accepted before merging.

---

## Active principles

This repo has `.principles` files that define which principles govern AI-assisted
work here. Run `/dot-prime` before starting any significant change:

```
/dot-prime
```

The active set covers: documentation quality (`@docs`), schema/YAML structure
(`@schema`), and plain-text practices (`@ptac` when self-hosting this catalog).
