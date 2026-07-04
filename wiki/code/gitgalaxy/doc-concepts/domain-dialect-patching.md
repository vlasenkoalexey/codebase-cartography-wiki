---
title: The Domain Dialect Pre-Flight Patch — per-project regex overrides at boot
type: doc-concept
provenance: doc
source: docs/wiki/02-02-optical-orchestration.md
updated: 2026-07-04
status: fresh
---
# The Domain Dialect Pre-Flight Patch — per-project regex overrides at boot

## Definition
`02-02-optical-orchestration.md` describes a boot-time recalibration step: "Before ignition, the
chassis checks for 'Project Overrides' in the scanning configuration. If a project name matches a
registered Dialect (e.g., `cpython`, `ansible`), the engine live-patches the language regex geometry
(updating both extensions and structural rules)... without breaking the global standard." The doc
frames this as letting the otherwise-generic heuristic engine "recalibrate its 'Spectral Focus' to
match the local reality of a specific project."

## In gitgalaxy (grounded)
This is a real, narrowly-scoped mechanism inside [`main`](../catalog/gitgalaxy/galaxyscope.md#main),
not a general plugin system. Before constructing the `Orchestrator`, `main` deep-copies the global
[`LANGUAGE_DEFINITIONS`](../catalog/gitgalaxy/standards/language_standards.md#LANGUAGE_DEFINITIONS)
and `APERTURE_CONFIG` tables, then checks whether the scan target's directory name is a key in
[`PROJECT_OVERRIDES`](../catalog/gitgalaxy/standards/language_standards.md#PROJECT_OVERRIDES) — a
module-level dict in `gitgalaxy/standards/language_standards.py` keyed by known project names. If it
matches, `main` walks the matched dialect's per-language override dict and merges it into the copied
tables: a special `"_shield_"` key can extend `APERTURE_CONFIG`'s `IGNORED_DIRECTORIES` and
`CONTRABAND_PATTERNS` (patching the [Aperture Filter](../concepts/gitgalaxy-core-aperture.md)'s own
exclusion sets for that one project), while other keys patch that language's structural rule geometry
in the copied `LANGUAGE_DEFINITIONS`. The merge happens on **copies**, so the global tables used for
every other target are never mutated — the doc's "without breaking the global standard" claim is
accurate to the code: `copy.deepcopy` is exactly the mechanism that guarantees it.

## Why it matters / when it applies
This is the one place gitgalaxy admits its heuristic tables need project-specific tuning to stay
accurate — an implicit concession to the same brittleness the doc's own [AST vs. heuristic
tradeoffs](ast-vs-heuristic-tradeoffs.md) page names more directly elsewhere: a single global regex
grammar cannot perfectly fit every real-world codebase's local conventions (a project's own build
scripts, generated-file naming, or embedded-DSL usage). Rather than asking a user to hand-edit the
global [Language standards](../concepts/gitgalaxy-standards-language_standards.md) tables, the tool
ships a small number of pre-baked, name-keyed overrides for large, well-known ecosystems and merges
them in only for a scan whose target directory name matches — a targeted patch, not a general
extensibility mechanism (there is no config flag to register a *new* dialect at scan time; the match is
purely against the hardcoded `PROJECT_OVERRIDES` dict).

## Connections
- Code concepts: [The Aperture Filter](../concepts/gitgalaxy-core-aperture.md) — the `"_shield_"`
  override key patches this filter's ignored-directory/contraband-pattern sets; [Language standards](../concepts/gitgalaxy-standards-language_standards.md) —
  the table being patched; [GalaxyScope orchestrator](../concepts/gitgalaxy-galaxyscope.md) — `main` is
  this mechanism's sole entry point, called before the `Orchestrator` is even constructed.
- Module catalogs: [galaxyscope](../catalog/gitgalaxy/galaxyscope.md), [language_standards](../catalog/gitgalaxy/standards/language_standards.md).
- Related doc-concepts: [optical-pipeline-metaphor](optical-pipeline-metaphor.md), [ast-vs-heuristic-tradeoffs](ast-vs-heuristic-tradeoffs.md).

## Source
Extracted from `docs/wiki/02-02-optical-orchestration.md`, kept in place.
