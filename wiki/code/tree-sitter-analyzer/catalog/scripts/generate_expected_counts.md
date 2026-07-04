---
title: 'Module: scripts/generate_expected_counts.py'
type: catalog
provenance: extracted
module: scripts/generate_expected_counts.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `scripts.generate_expected_counts`/
symbols:
  generate_expected_json: generate_expected_json().
  parse_corpus_file: parse_corpus_file().
  parse_corpus_file.count_nodes: parse_corpus_file().count_nodes().
  main: main().
  get_language_config: get_language_config().
---
# Module: [`scripts/generate_expected_counts.py`](../../../../../raw/code/tree-sitter-analyzer/scripts/generate_expected_counts.py)

## Functions
- `count_nodes(node: tree_sitter.Node)` — [`L210`](../../../../../raw/code/tree-sitter-analyzer/scripts/generate_expected_counts.py#L210)
- `generate_expected_json(language: str, golden_dir: Path)` — [`L237`](../../../../../raw/code/tree-sitter-analyzer/scripts/generate_expected_counts.py#L237) — Generate expected.json file for a language.
- `get_language_config(language: str)` — [`L23`](../../../../../raw/code/tree-sitter-analyzer/scripts/generate_expected_counts.py#L23) — Get configuration for a language.
- `main()` — [`L275`](../../../../../raw/code/tree-sitter-analyzer/scripts/generate_expected_counts.py#L275) — Main entry point.
- `parse_corpus_file(corpus_path: Path, language: str)` — [`L174`](../../../../../raw/code/tree-sitter-analyzer/scripts/generate_expected_counts.py#L174) — Parse corpus file and count node types.

