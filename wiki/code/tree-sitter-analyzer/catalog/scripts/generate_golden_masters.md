---
title: 'Module: scripts/generate_golden_masters.py'
type: catalog
provenance: extracted
module: scripts/generate_golden_masters.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `scripts.generate_golden_masters`/
symbols:
  main: main().
  generate_golden_master: generate_golden_master().
  verify_golden_masters: verify_golden_masters().
  run_analyzer: run_analyzer().
  update_test_file: update_test_file().
---
# Module: [`scripts/generate_golden_masters.py`](../../../../../raw/code/tree-sitter-analyzer/scripts/generate_golden_masters.py)

## Functions
- `generate_golden_master(language: str, sample_file: str, output_base_name: str | None = None)` — [`L32`](../../../../../raw/code/tree-sitter-analyzer/scripts/generate_golden_masters.py#L32) — Generate golden master files for a language
- `main()` — [`L170`](../../../../../raw/code/tree-sitter-analyzer/scripts/generate_golden_masters.py#L170) — Main entry point
- `run_analyzer(input_file: str, table_format: str)` — [`L21`](../../../../../raw/code/tree-sitter-analyzer/scripts/generate_golden_masters.py#L21) — Run tree-sitter-analyzer and return output
- `update_test_file(language: str, sample_file: str, output_base_name: str)` — [`L140`](../../../../../raw/code/tree-sitter-analyzer/scripts/generate_golden_masters.py#L140) — Print instructions for updating test_golden_master_regression.py
- `verify_golden_masters(language: str, sample_file: str, output_base_name: str)` — [`L86`](../../../../../raw/code/tree-sitter-analyzer/scripts/generate_golden_masters.py#L86) — Verify that golden masters are consistent across multiple runs

