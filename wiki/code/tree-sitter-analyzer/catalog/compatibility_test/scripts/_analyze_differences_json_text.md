---
title: 'Module: compatibility_test/scripts/_analyze_differences_json_text.py'
type: catalog
provenance: extracted
module: compatibility_test/scripts/_analyze_differences_json_text.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `compatibility_test.scripts._analyze_differences_json_text`/
symbols:
  analyze_text_difference: analyze_text_difference().
  load_json_pair: load_json_pair().
  _count_diff_lines: _count_diff_lines().
  _unified_diff_lines: _unified_diff_lines().
---
# Module: [`compatibility_test/scripts/_analyze_differences_json_text.py`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/_analyze_differences_json_text.py)

## Functions
- `_count_diff_lines(diff_lines: list[str], prefix: str, excluded_prefix: str)` — [`L67`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/_analyze_differences_json_text.py#L67)
- `_unified_diff_lines(content_a: str, content_b: str, file_a: Path, file_b: Path, version_a: str, version_b: str)` — [`L49`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/_analyze_differences_json_text.py#L49)
- `analyze_text_difference(file_a: Path, file_b: Path, version_a: str, version_b: str)` — [`L9`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/_analyze_differences_json_text.py#L9) — Analyze a text file difference.
- `load_json_pair(file_a: Path, file_b: Path)` — [`L37`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/_analyze_differences_json_text.py#L37) — Load two JSON files or return the legacy error payload.

