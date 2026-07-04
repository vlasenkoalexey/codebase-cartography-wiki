---
title: Output-language detection & localization
type: doc-concept
provenance: doc
source: docs/superpowers/specs/2026-06-03-language-auto-detection-design.md
updated: 2026-07-04
status: fresh
---
# Output-language detection & localization

## Definition
All LLM-authored content (node summaries, tags, layer names, tours, language
notes) is generated in one output language. That language is resolved by a
priority chain: an explicit `--language` flag → a stored `outputLanguage` in
`.understand-anything/config.json` → (new) **first-run detection of the
conversation language**, gated so it only surfaces a confirmation when the
detected language is non-English. English users see zero behavior change; a
Chinese/Japanese/etc. conversation gets a one-time "generate in this language?"
gate before the analysis budget is spent, and the choice is persisted.

## In understand-anything (grounded)
This spec is deliberately a **prompt-logic change with no code changes** — the
resolution chain lives in `skills/understand/SKILL.md` (markdown, not indexed as
a code symbol), and it relies on data structures that already exist. The persisted
setting is [`ProjectConfig.outputLanguage`](../catalog/understand-anything-plugin/packages/core/src/types.ts.md#ProjectConfig.outputLanguage)
on [`ProjectConfig`](../catalog/understand-anything-plugin/packages/core/src/types.ts.md#ProjectConfig);
it is read and written through
[`loadConfig`](../catalog/understand-anything-plugin/packages/core/src/persistence/index.ts.md#loadConfig)
/ [`saveConfig`](../catalog/understand-anything-plugin/packages/core/src/persistence/index.ts.md#saveConfig)
(with [`DEFAULT_CONFIG`](../catalog/understand-anything-plugin/packages/core/src/persistence/index.ts.md#DEFAULT_CONFIG),
[`CONFIG_FILE`](../catalog/understand-anything-plugin/packages/core/src/persistence/index.ts.md#CONFIG_FILE)),
so the gate fires at most once per project. The friendly-name normalization and
per-language content directives are the language-lesson layer
([`getLanguageDisplayName`](../catalog/understand-anything-plugin/packages/core/src/analyzer/language-lesson.ts.md#getLanguageDisplayName)).

On the dashboard side, localized UI labels are served by the i18n context
(the `en/zh/zh-TW/ja/ko/ru` locale bundles) — the runtime string layer that the
generated `outputLanguage` content sits alongside.

> [!inferred]
> The spec notes the detection step itself is interpreted by the model at
> runtime from `SKILL.md`; there is no TypeScript function to cite for it. The
> only code touchpoint is the pre-existing `outputLanguage` field — grounded
> above — so this page documents the *mechanism and its config anchor*, not a new
> code path.

## Why it matters / when it applies
The failure this fixes is silent and expensive: a non-English user paid for a
full analysis run and got an English graph, discovering the mismatch only
afterward. The gate is first-run-only, non-English-only, and degrades gracefully
in non-interactive/CI contexts (falls back to the detected language with a
notice, never blocks). It is scoped to `/understand`; the other content skills
(`understand-domain`, `understand-knowledge`, `understand-explain`) still ignore
`outputLanguage` — a known, deferred gap.

## Connections
- Code concepts: [core types](../concepts/understand-anything-plugin-packages-core-src-types.ts.md), [persistence](../concepts/understand-anything-plugin-packages-core-src-persistence-index.ts.md), [I18n context (dashboard localization)](../concepts/understand-anything-plugin-packages-dashboard-src-contexts-I18nContext.tsx.md)
- Module catalogs: [types.ts](../catalog/understand-anything-plugin/packages/core/src/types.ts.md), [persistence/index.ts](../catalog/understand-anything-plugin/packages/core/src/persistence/index.ts.md), [analyzer/language-lesson.ts](../catalog/understand-anything-plugin/packages/core/src/analyzer/language-lesson.ts.md)
- Related doc-concepts: [language-agnostic-extraction](language-agnostic-extraction.md), [multi-agent-pipeline](multi-agent-pipeline.md)

## Source
Extracted from `docs/superpowers/specs/2026-06-03-language-auto-detection-design.md`
(kept in place).
