---
title: 'Module: scripts/generate_corpus_expected.py'
type: catalog
provenance: extracted
module: scripts/generate_corpus_expected.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `scripts.generate_corpus_expected`/
symbols:
  generate_expected_json: generate_expected_json().
  count_node_types: count_node_types().
  count_node_types.count_nodes: count_node_types().count_nodes().
  main: main().
  get_language_config: get_language_config().
  filter_critical_types: filter_critical_types().
---
# Module: [`scripts/generate_corpus_expected.py`](../../../../../raw/code/tree-sitter-analyzer/scripts/generate_corpus_expected.py)

## Functions
- `count_node_types(corpus_path: Path, language: str)` — [`L90`](../../../../../raw/code/tree-sitter-analyzer/scripts/generate_corpus_expected.py#L90) — Count node types in corpus file using tree-sitter.
- `count_nodes(node: tree_sitter.Node)` — [`L122`](../../../../../raw/code/tree-sitter-analyzer/scripts/generate_corpus_expected.py#L122)
- `filter_critical_types(all_counts: dict[str, int], critical_types: list[str])` — [`L134`](../../../../../raw/code/tree-sitter-analyzer/scripts/generate_corpus_expected.py#L134) — Filter node counts to only include critical types.
- `generate_expected_json(language: str)` — [`L154`](../../../../../raw/code/tree-sitter-analyzer/scripts/generate_corpus_expected.py#L154) — Generate expected.json for a language's corpus file.
- `get_language_config(language: str)` — [`L24`](../../../../../raw/code/tree-sitter-analyzer/scripts/generate_corpus_expected.py#L24) — Get language configuration (module name and critical node types).
- `main()` — [`L201`](../../../../../raw/code/tree-sitter-analyzer/scripts/generate_corpus_expected.py#L201) — Main entry point.

