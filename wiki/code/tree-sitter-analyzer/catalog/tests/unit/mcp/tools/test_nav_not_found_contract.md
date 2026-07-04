---
title: 'Module: tests/unit/mcp/tools/test_nav_not_found_contract.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/tools/test_nav_not_found_contract.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.tools.test_nav_not_found_contract`/
symbols:
  test_edges_without_built_marker_no_empty_index_hint: test_edges_without_built_marker_no_empty_index_hint().
  _make_built_index_with_edges: _make_built_index_with_edges().
  _run_missing: _run_missing().
  test_missing_symbol_in_populated_index_contract: test_missing_symbol_in_populated_index_contract().
  _MISSING: _MISSING.
  _TOOL_LABELS: _TOOL_LABELS.
  _FORBIDDEN_HINT_FRAGMENTS: _FORBIDDEN_HINT_FRAGMENTS.
---
# Module: [`tests/unit/mcp/tools/test_nav_not_found_contract.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_nav_not_found_contract.py)

## Functions
- `_make_built_index_with_edges(root: Any)` — [`L40`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_nav_not_found_contract.py#L40) — Index a tiny project that contains a real call edge (caller -> target).
- `_run_missing(tool_label: str, root: str)` — [`L60`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_nav_not_found_contract.py#L60) — Execute the named tool for the missing symbol; return the JSON envelope.
- `test_edges_without_built_marker_no_empty_index_hint(tmp_path: Any, tool_cls: type[CodeGraphCallersTool] | type[CodeGraphCalleesTool])` — [`L118`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_nav_not_found_contract.py#L118) — #981 defense-in-depth: edges present but the built marker is a
- `test_missing_symbol_in_populated_index_contract(tmp_path: Any, tool_label: str)` — [`L90`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_nav_not_found_contract.py#L90) — #981: missing symbol, BUILT index WITH edges.

## Module values
- `_FORBIDDEN_HINT_FRAGMENTS` — [`L37`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_nav_not_found_contract.py#L37)
- `_MISSING` — [`L35`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_nav_not_found_contract.py#L35)
- `_TOOL_LABELS` — [`L85`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_nav_not_found_contract.py#L85)

