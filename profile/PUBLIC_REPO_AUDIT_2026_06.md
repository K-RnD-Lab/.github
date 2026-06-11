# K R&D Lab Public Repo Audit - 2026-06

## Purpose

This file tracks the public-facing readiness of K R&D Lab repositories and keeps GitHub, Hugging Face, and sphere-level research structure aligned.

## Public GitHub repositories

| Repository | Role | Current status | Next polish |
|---|---|---|---|
| `.github` | Organization profile and public landing layer | Active | Keep overview, sphere links, and public disclaimers current |
| `SPHERE-FRONTIER` | Front-door interface for the SET ecosystem | Active | Keep live app link and cross-sphere positioning current |
| `SPHERE-I-SCIENCE` | Science research workspace | Active | Keep S1-S7 lanes, active studies, and Hugging Face links synchronized |
| `SPHERE-II-ENTREPRENEURSHIP` | Venture, market, ecosystem, and public-case research | Active starter repo | Add more public cases and link back to S/E/T registry |
| `SPHERE-III-TECHNOLOGY` | Tools, dashboards, scoring, reproducibility, infrastructure | Active starter repo | Keep registry automation and dashboard links current |

## Active public layers

- Science: `SPHERE-I-SCIENCE`
- Entrepreneurship: `SPHERE-II-ENTREPRENEURSHIP`
- Technology: `SPHERE-III-TECHNOLOGY`
- Cross-sphere front door: `SPHERE-FRONTIER`
- Organization profile: `.github/profile/README.md`
- Interactive delivery: Hugging Face Spaces under `K-RnD-Lab`

## Current active research and interface anchors

- `S1`: biomedical and oncology research packs plus Hugging Face biomedical demos
- `S2`: plant science and phytochemistry research staging
- `S6`: K-EcoLOGIC environmental platform and research packs
- `S7-I`: Master Prep Analytics
- `S7-K`: Partner Pool Assumption Simulator
- `S7-D`: Investment Systems & Paper Trading scaffold
- `E1-E4`: starter entrepreneurship studies and public cases
- `T1-T3`: reusable tooling, readiness scoring, and study registry dashboard

## Placeholder audit

Actionable placeholder text found so far:

- `SPHERE-I-SCIENCE / S7-I / R1 - Master Prep Analytics / README.md`
  - Previous `REPLACE_ME` public links were converted to private/planned status labels.

Non-actionable placeholder language:

- simulated biomedical benchmark notes in `S1`
  - These are methodological caveats and should remain visible unless the studies are replaced with real validation data.
- `TBD` values in evidence schemas
  - These are staging markers for evidence extraction, not public broken links.

## Public-safety rules

Do not commit:

- service-account JSON
- OAuth client secrets
- Telegram tokens or chat IDs
- exchange keys
- VM SSH material
- private UID files
- runtime state with private identifiers

## Sync rule

GitHub keeps structure, reports, source maps, and public-safe scaffolds.

Hugging Face keeps interactive spaces and demo runtimes.

Private VM/Firebase systems can be represented in GitHub only through sanitized architecture, schema, and research notes.
