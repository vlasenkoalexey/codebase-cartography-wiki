---
title: Tree-sitter + LLM hybrid analysis
type: doc-concept
provenance: doc
source: README.md
updated: 2026-07-04
status: fresh
---
# Tree-sitter + LLM hybrid analysis

## Definition
Understand-Anything comprehends code by splitting the work between two engines
that each do what they do best: **tree-sitter (deterministic)** parses source
into a concrete syntax tree and extracts structural facts — imports, exports,
function/class definitions, call sites, inheritance — while the **LLM
(semantic)** reads that parsed structure alongside the original source to produce
what parsers can't: plain-English summaries, tags, architectural-layer
assignments, and language-concept callouts. The split is the tool's grounding
substrate: the structural side is reproducible (same code → same edges every
run), the semantic side captures intent (what a file is *for*, not just what it
imports).

## In understand-anything (grounded)
Structural extraction is the plugin layer. Every analyzer implements the
[`AnalyzerPlugin`](../catalog/understand-anything-plugin/packages/core/src/types.ts.md#AnalyzerPlugin)
interface; the shipped one is
[`TreeSitterPlugin`](../catalog/understand-anything-plugin/packages/core/src/plugins/tree-sitter-plugin.ts.md#TreeSitterPlugin),
whose [`analyzeFile`](../catalog/understand-anything-plugin/packages/core/src/plugins/tree-sitter-plugin.ts.md#TreeSitterPlugin.analyzeFile),
[`resolveImports`](../catalog/understand-anything-plugin/packages/core/src/plugins/tree-sitter-plugin.ts.md#TreeSitterPlugin.resolveImports),
and [`extractCallGraph`](../catalog/understand-anything-plugin/packages/core/src/plugins/tree-sitter-plugin.ts.md#TreeSitterPlugin.extractCallGraph)
produce the structural spine. Per-language parsing is delegated to
[`LanguageExtractor`](../catalog/understand-anything-plugin/packages/core/src/plugins/extractors/types.ts.md#LanguageExtractor)
implementations that share the AST-walking helpers
([`traverse`](../catalog/understand-anything-plugin/packages/core/src/plugins/extractors/base-extractor.ts.md#traverse),
[`findChild`](../catalog/understand-anything-plugin/packages/core/src/plugins/extractors/base-extractor.ts.md#findChild)).
The [`PluginRegistry`](../catalog/understand-anything-plugin/packages/core/src/plugins/registry.ts.md#PluginRegistry)
routes each file to the right plugin by language.

> [!inferred]
> Note: the README says tree-sitter uses `node-tree-sitter`, but the shipped
> code uses `web-tree-sitter` (WASM) — the repo's own `CLAUDE.md` records the
> switch (native bindings fail on darwin/arm64 + Node 24).

The semantic side is the LLM analyzer. The prompt and response plumbing lives in
`analyzer/llm-analyzer.ts`:
[`buildFileAnalysisPrompt`](../catalog/understand-anything-plugin/packages/core/src/analyzer/llm-analyzer.ts.md#buildFileAnalysisPrompt)
feeds the parsed structure + source to the model and
[`parseFileAnalysisResponse`](../catalog/understand-anything-plugin/packages/core/src/analyzer/llm-analyzer.ts.md#parseFileAnalysisResponse)
turns the reply (summary, tags, complexity) back into typed data. Because
structural facts are deterministic, they also drive change detection — the
fingerprint layer ([`extractFileFingerprint`](../catalog/understand-anything-plugin/packages/core/src/fingerprint.ts.md#extractFileFingerprint))
hashes the same extracted structure.

## Why it matters / when it applies
This hybrid is the answer to "what is the grounding substrate?" — the axis that
makes this tool comparable to other code-comprehension tools. Unlike a
pure-LLM reader, structural edges are exact and repeatable; unlike a pure static
analyzer, the graph carries human-readable intent. Tree-sitter is an
*enhancement, not a gate*: an unknown language still gets an LLM summary and a
graph node (see language-agnostic-extraction), so coverage never silently drops.

## Connections
- Code concepts: [tree-sitter-plugin](../concepts/understand-anything-plugin-packages-core-src-plugins-tree-sitter-plugin.ts.md), [plugin registry](../concepts/understand-anything-plugin-packages-core-src-plugins-registry.ts.md), [base extractor](../concepts/understand-anything-plugin-packages-core-src-plugins-extractors-base-extractor.ts.md), [extractor types](../concepts/understand-anything-plugin-packages-core-src-plugins-extractors-types.ts.md), [fingerprint](../concepts/understand-anything-plugin-packages-core-src-fingerprint.ts.md), [core types](../concepts/understand-anything-plugin-packages-core-src-types.ts.md)
- Module catalogs: [tree-sitter-plugin.ts](../catalog/understand-anything-plugin/packages/core/src/plugins/tree-sitter-plugin.ts.md), [registry.ts](../catalog/understand-anything-plugin/packages/core/src/plugins/registry.ts.md), [extractors/base-extractor.ts](../catalog/understand-anything-plugin/packages/core/src/plugins/extractors/base-extractor.ts.md), [extractors/types.ts](../catalog/understand-anything-plugin/packages/core/src/plugins/extractors/types.ts.md), [analyzer/llm-analyzer.ts](../catalog/understand-anything-plugin/packages/core/src/analyzer/llm-analyzer.ts.md), [types.ts](../catalog/understand-anything-plugin/packages/core/src/types.ts.md)
- Related doc-concepts: [knowledge-graph-schema](knowledge-graph-schema.md), [multi-agent-pipeline](multi-agent-pipeline.md), [language-agnostic-extraction](language-agnostic-extraction.md), [incremental-reconcile](incremental-reconcile.md)

## Source
Extracted from `README.md` (§ Under the Hood — Tree-sitter + LLM hybrid) and
`docs/superpowers/specs/2026-03-14-understand-anything-design.md` (§ Plugin
System), both kept in place.
