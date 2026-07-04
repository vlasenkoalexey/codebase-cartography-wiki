---
title: Language-agnostic extraction
type: doc-concept
provenance: doc
source: docs/superpowers/specs/2026-03-21-language-agnostic-design.md
updated: 2026-07-04
status: fresh
---
# Language-agnostic extraction

## Definition
The extraction framework is language-neutral by design; the bias that made early
versions TypeScript-heavy lived in *shipped content*, not the architecture. The
fix is **config-first with a code escape hatch**: each language is a declarative
`LanguageConfig` (extensions, tree-sitter grammar package, node-type mappings for
function/class/import/export, key concepts), registered in a registry, and driven
through one generic tree-sitter plugin — with a per-language custom analyzer only
where the AST shape is unusual. Prompts get the same treatment: a base
language-neutral prompt plus per-language markdown snippets injected by detected
language.

## In understand-anything (grounded)
The config type and its Zod validation are in `packages/core/src/languages/types.ts`:
[`LanguageConfig`](../catalog/understand-anything-plugin/packages/core/src/languages/types.ts.md#LanguageConfig),
[`TreeSitterConfig`](../catalog/understand-anything-plugin/packages/core/src/languages/types.ts.md#TreeSitterConfig),
validated by [`LanguageConfigSchema`](../catalog/understand-anything-plugin/packages/core/src/languages/types.ts.md#LanguageConfigSchema)
/ [`StrictLanguageConfigSchema`](../catalog/understand-anything-plugin/packages/core/src/languages/types.ts.md#StrictLanguageConfigSchema)
(the spec's "fail fast at registration" rule). The registry is
[`LanguageRegistry`](../catalog/understand-anything-plugin/packages/core/src/languages/language-registry.ts.md#LanguageRegistry)
— [`getByExtension`](../catalog/understand-anything-plugin/packages/core/src/languages/language-registry.ts.md#LanguageRegistry.getByExtension),
[`getForFile`](../catalog/understand-anything-plugin/packages/core/src/languages/language-registry.ts.md#LanguageRegistry.getForFile),
[`createDefault`](../catalog/understand-anything-plugin/packages/core/src/languages/language-registry.ts.md#LanguageRegistry.createDefault)
(auto-registers the built-in configs). Frameworks get a parallel
[`FrameworkRegistry`](../catalog/understand-anything-plugin/packages/core/src/languages/framework-registry.ts.md#FrameworkRegistry)
([`detectFrameworks`](../catalog/understand-anything-plugin/packages/core/src/languages/framework-registry.ts.md#FrameworkRegistry.detectFrameworks)).

> [!inferred]
> The pinned code has grown well past the spec's v1 list of 12 languages — the
> `languages/configs/` directory ships ~45 configs (code languages plus config
> formats like Dockerfile, Terraform, YAML, SQL). The spec's single
> `GenericTreeSitterPlugin` also landed as the per-language
> [`LanguageExtractor`](../catalog/understand-anything-plugin/packages/core/src/plugins/extractors/types.ts.md#LanguageExtractor)
> pattern (one extractor class per language, e.g. `SwiftExtractor`,
> `DartExtractor`) sharing the `base-extractor` helpers, rather than one config-
> driven class — same idea, different factoring.

Extractors are registered on the plugin via
[`registerExtractor`](../catalog/understand-anything-plugin/packages/core/src/plugins/tree-sitter-plugin.ts.md#TreeSitterPlugin.registerExtractor)
and looked up with
[`getExtractor`](../catalog/understand-anything-plugin/packages/core/src/plugins/tree-sitter-plugin.ts.md#TreeSitterPlugin.getExtractor);
the [`PluginRegistry`](../catalog/understand-anything-plugin/packages/core/src/plugins/registry.ts.md#PluginRegistry)
holds a [`languageRegistry`](../catalog/understand-anything-plugin/packages/core/src/plugins/registry.ts.md#PluginRegistry.languageRegistry).
The spec's config-driven language lessons are
[`detectLanguageConcepts`](../catalog/understand-anything-plugin/packages/core/src/analyzer/language-lesson.ts.md#detectLanguageConcepts)
and [`getLanguageDisplayName`](../catalog/understand-anything-plugin/packages/core/src/analyzer/language-lesson.ts.md#getLanguageDisplayName)
(replacing the deleted hardcoded `LANGUAGE_DISPLAY_NAMES`).

## Why it matters / when it applies
The spec's key principle is graceful degradation: **every file always gets
analyzed.** Tree-sitter is an enhancement — an unknown extension returns `null`
structural analysis and the LLM still produces a summary, tags, and a graph node;
a missing WASM grammar degrades that one language to LLM-only without affecting
others. For a cross-tool survey this is the multi-language-extraction axis:
Understand-Anything gets broad coverage from a declarative config table plus a
uniform extractor interface, and never hard-fails on an unsupported language.

## Connections
- Code concepts: [language config types](../concepts/understand-anything-plugin-packages-core-src-languages-types.ts.md), [extractor types](../concepts/understand-anything-plugin-packages-core-src-plugins-extractors-types.ts.md), [base extractor](../concepts/understand-anything-plugin-packages-core-src-plugins-extractors-base-extractor.ts.md), [swift extractor](../concepts/understand-anything-plugin-packages-core-src-plugins-extractors-swift-extractor.ts.md), [dart extractor](../concepts/understand-anything-plugin-packages-core-src-plugins-extractors-dart-extractor.ts.md), [plugin registry](../concepts/understand-anything-plugin-packages-core-src-plugins-registry.ts.md), [tree-sitter-plugin](../concepts/understand-anything-plugin-packages-core-src-plugins-tree-sitter-plugin.ts.md)
- Module catalogs: [languages/types.ts](../catalog/understand-anything-plugin/packages/core/src/languages/types.ts.md), [languages/language-registry.ts](../catalog/understand-anything-plugin/packages/core/src/languages/language-registry.ts.md), [languages/framework-registry.ts](../catalog/understand-anything-plugin/packages/core/src/languages/framework-registry.ts.md), [plugins/extractors/types.ts](../catalog/understand-anything-plugin/packages/core/src/plugins/extractors/types.ts.md), [plugins/extractors/base-extractor.ts](../catalog/understand-anything-plugin/packages/core/src/plugins/extractors/base-extractor.ts.md), [analyzer/language-lesson.ts](../catalog/understand-anything-plugin/packages/core/src/analyzer/language-lesson.ts.md)
- Related doc-concepts: [tree-sitter-llm-hybrid](tree-sitter-llm-hybrid.md), [output-language-detection](output-language-detection.md)

## Source
Extracted from `docs/superpowers/specs/2026-03-21-language-agnostic-design.md`
(kept in place).
