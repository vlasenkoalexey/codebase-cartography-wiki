---
title: 'Module: tests/unit/test_node_text_perf_contract.py'
type: catalog
provenance: extracted
module: tests/unit/test_node_text_perf_contract.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_node_text_perf_contract`/
symbols:
  test_node_text_throughput_is_O1_per_call: test_node_text_throughput_is_O1_per_call().
  test_node_text_does_not_encode_twice: test_node_text_does_not_encode_twice().
  test_node_text_throughput_is_O1_per_call.collect: test_node_text_throughput_is_O1_per_call().collect().
  _node_text_files: _node_text_files().
  _REPO_ROOT: _REPO_ROOT.
  _extract_function: _extract_function().
---
# Module: [`tests/unit/test_node_text_perf_contract.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_node_text_perf_contract.py)

## Functions
- `_extract_function(text: str, name: str)` — [`L54`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_node_text_perf_contract.py#L54) — Return the source of a top-level function ``name`` from a module.
- `_node_text_files()` — [`L40`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_node_text_perf_contract.py#L40) — All modules under tree_sitter_analyzer/ defining a ``_node_text``.
- `collect(node)` — [`L129`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_node_text_perf_contract.py#L129)
- `test_node_text_does_not_encode_twice()` — [`L72`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_node_text_perf_contract.py#L72) — No ``_node_text`` implementation may contain two encode() calls.
- `test_node_text_throughput_is_O1_per_call()` — [`L108`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_node_text_perf_contract.py#L108) — Micro-bench: 5k calls on a small ASCII source must finish quickly.

## Module values
- `_REPO_ROOT` — [`L37`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_node_text_perf_contract.py#L37)

