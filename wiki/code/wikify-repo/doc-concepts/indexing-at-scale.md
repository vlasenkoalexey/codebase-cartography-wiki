---
title: Indexing at scale — sharding, AST fallback, and the symbol-recovery floor
type: doc-concept
provenance: doc
source: docs/implementation.md
updated: 2026-07-04
status: fresh
---
# Indexing at scale — sharding, AST fallback, and the symbol-recovery floor

## Definition
Real ingests (pytorch, jax, torch_tpu) forced mechanisms that make L1 grounding
robust to indexer limits at scale. Two failure modes had to be handled without
"give the type checker more memory": scip-python/pyright is single-process and
**OOMs** on pytorch at any heap size, and it **drops or fails** on some symbols/files
(a `RangeError`, or a file it can't type at all). The design's response is a
**symbol-recovery floor**: ingestion is robust to *partial* indexer failure, so
thousands of existing references still bind to a recovered symbol rather than
dangling.

## In wikify-repo (grounded)
- **Sharding, not heap.** [`run_indexer_sharded`](../catalog/wikify/scip_index.md#run_indexer_sharded)
  runs one `scip-python --target-only <path>` process per shard with a bounded
  working set; because monikers are global,
  [`merge_shards`](../catalog/wikify/scip_index.md#merge_shards) unions the shard
  indexes, repairing each doc's target-relative path back to repo-relative. Then
  [`build_graph`](../catalog/wikify/scip_index.md#build_graph) unions everything into
  one [`SymbolGraph`](../catalog/wikify/graph.md#SymbolGraph).
- **Orphan-synthesis.** When pyright records a definition *occurrence* but drops the
  symbol's `SymbolInformation` (RangeError), build_graph synthesizes the node from
  that occurrence via [`_synth_symbol`](../catalog/wikify/scip_index.md#_synth_symbol)
  so it stays citable/coverable (recovered `nn.Module` + ~2000 symbols).
- **AST fallback.** For files pyright crashes on entirely (e.g. `torch/_tensor.py` =
  `torch.Tensor`), [`synthesize_index`](../catalog/wikify/ast_fallback.md#synthesize_index)
  parses them with Python's own `ast` (the [`_document`](../catalog/wikify/ast_fallback.md#_document)
  visitor, [`module_path`](../catalog/wikify/ast_fallback.md#module_path)) and emits
  symbols whose monikers **match scip-python's scheme exactly**, so the thousands of
  existing references join (Tensor recovered with 4990 callers). Run automatically for
  any target file the shards didn't emit.

Any heuristic edge produced this way carries provenance so it never masquerades as a
resolved fact — the recovery floor sits *below* the grounding floor, never above it.

## Why it matters / when it applies
This is what lets the SCIP-grounding bet survive on the largest real codebases: a
type checker literally *can't* index everything, so completeness comes from
recovery, not from a bigger machine. For the survey, it is the honest counter to
"SCIP is heavier than tree-sitter" — the heaviness is bounded by sharding, and
partial failure degrades to recovery rather than dropped subsystems.

## Connections
- Code concepts: [SCIP indexing](../concepts/wikify-scip_index.md) — the indexer orchestration; [AST fallback](../concepts/wikify-ast_fallback.md) — the recovery parser; [SymbolGraph](../concepts/wikify-graph.md) — where recovered nodes land.
- Module catalogs: [scip_index](../catalog/wikify/scip_index.md), [ast_fallback](../catalog/wikify/ast_fallback.md), [graph](../catalog/wikify/graph.md).
- Related doc-concepts: [scip-vs-ast-grounding](scip-vs-ast-grounding.md), [devirtualization-dispatch-seam](devirtualization-dispatch-seam.md), [concept-driven-synthesis-and-coverage](concept-driven-synthesis-and-coverage.md).

## Source
Extracted from `docs/implementation.md` (§10.1 sharded scip-python + AST fallback;
§10.2 orphan-synthesis in `build_graph`), with the "symbol-recovery floor" and
"scale by sharding, not heap" decisions from `docs/design.md` (Decisions log). Kept
in place.
