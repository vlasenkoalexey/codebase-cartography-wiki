---
title: 'Module: tests/unit/test_codegraph_status_tool.py'
type: catalog
provenance: extracted
module: tests/unit/test_codegraph_status_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_codegraph_status_tool`/
symbols:
  tool: tool().
  tool_with_root: tool_with_root().
  TestToolDefinition: TestToolDefinition#
  TestToolDefinition.test_tool_name: TestToolDefinition#test_tool_name().
  TestToolDefinition.test_description_starts_with_index_health: TestToolDefinition#test_description_starts_with_index_health().
  TestToolDefinition.test_annotations_all_four_hints: TestToolDefinition#test_annotations_all_four_hints().
  TestToolDefinition.test_schema_strict_no_additional_properties: TestToolDefinition#test_schema_strict_no_additional_properties().
  TestToolDefinition.test_schema_output_format_default_is_toon: TestToolDefinition#test_schema_output_format_default_is_toon().
  TestToolDefinition.test_schema_include_lag_default_true: TestToolDefinition#test_schema_include_lag_default_true().
  TestValidateArguments: TestValidateArguments#
  TestValidateArguments.test_empty_args_accepted: TestValidateArguments#test_empty_args_accepted().
  TestValidateArguments.test_include_lag_must_be_bool: TestValidateArguments#test_include_lag_must_be_bool().
  TestExecuteNoProjectRoot: TestExecuteNoProjectRoot#
  TestExecuteNoProjectRoot.test_no_project_root_returns_not_found: TestExecuteNoProjectRoot#test_no_project_root_returns_not_found().
  TestExecuteNoCache: TestExecuteNoCache#
  TestExecuteNoCache.test_project_set_but_no_cache_returns_warn: TestExecuteNoCache#test_project_set_but_no_cache_returns_warn().
  TestExecuteWithIndex: TestExecuteWithIndex#
  TestExecuteWithIndex.test_indexed_returns_info_verdict: TestExecuteWithIndex#test_indexed_returns_info_verdict().
  TestExecuteWithIndex.test_storage_counters_are_surfaced: TestExecuteWithIndex#test_storage_counters_are_surfaced().
  TestExecuteWithIndex.test_total_edges_reported_for_graph_density: TestExecuteWithIndex#test_total_edges_reported_for_graph_density().
  TestExecuteWithIndex.test_total_edges_zero_when_edges_absent: TestExecuteWithIndex#test_total_edges_zero_when_edges_absent().
  TestExecuteWithIndex.test_indexed_with_lag_computes_seconds: TestExecuteWithIndex#test_indexed_with_lag_computes_seconds().
  TestExecuteWithIndex.test_cache_exists_but_empty_returns_warn: TestExecuteWithIndex#test_cache_exists_but_empty_returns_warn().
  TestExecuteOutputFormat: TestExecuteOutputFormat#
  TestExecuteOutputFormat.test_toon_format_default: TestExecuteOutputFormat#test_toon_format_default().
  TestExecuteOutputFormat.test_json_format_no_toon_blob: TestExecuteOutputFormat#test_json_format_no_toon_blob().
  TestEmptyIndexHint: TestEmptyIndexHint#
  TestEmptyIndexHint.test_hint_uses_facade_phrasing: TestEmptyIndexHint#test_hint_uses_facade_phrasing().
  TestEmptyIndexHint.test_hint_has_no_codegraph_prefix: TestEmptyIndexHint#test_hint_has_no_codegraph_prefix().
---
# Module: [`tests/unit/test_codegraph_status_tool.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_status_tool.py)

## Classes
### `TestEmptyIndexHint`
- def: [`tests/unit/test_codegraph_status_tool.py:299`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_status_tool.py#L299)
- doc: D3 — empty-index hint must reference the facade phrasing, not v1.x names.
- signature: `class TestEmptyIndexHint:`
- members:
  - `test_hint_has_no_codegraph_prefix(self, tool_with_root)` — [`L312`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_status_tool.py#L312) — Hint must NOT reference deprecated codegraph_autoindex name.
  - `test_hint_uses_facade_phrasing(self, tool_with_root)` — [`L303`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_status_tool.py#L303) — Hint must say 'index' tool with action=auto (current facade).

### `TestExecuteNoCache`
- def: [`tests/unit/test_codegraph_status_tool.py:77`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_status_tool.py#L77)
- signature: `class TestExecuteNoCache:`
- members:
  - `test_project_set_but_no_cache_returns_warn(self, tool_with_root)` — [`L79`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_status_tool.py#L79)

### `TestExecuteNoProjectRoot`
- def: [`tests/unit/test_codegraph_status_tool.py:64`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_status_tool.py#L64)
- signature: `class TestExecuteNoProjectRoot:`
- members:
  - `test_no_project_root_returns_not_found(self, tool)` — [`L66`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_status_tool.py#L66)

### `TestExecuteOutputFormat`
- def: [`tests/unit/test_codegraph_status_tool.py:285`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_status_tool.py#L285)
- signature: `class TestExecuteOutputFormat:`
- members:
  - `test_json_format_no_toon_blob(self, tool)` — [`L293`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_status_tool.py#L293)
  - `test_toon_format_default(self, tool)` — [`L287`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_status_tool.py#L287)

### `TestExecuteWithIndex`
- def: [`tests/unit/test_codegraph_status_tool.py:89`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_status_tool.py#L89)
- signature: `class TestExecuteWithIndex:`
- members:
  - `test_cache_exists_but_empty_returns_warn(self, tool_with_root, tmp_path)` — [`L260`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_status_tool.py#L260)
  - `test_indexed_returns_info_verdict(self, tool_with_root, tmp_path)` — [`L91`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_status_tool.py#L91)
  - `test_indexed_with_lag_computes_seconds(self, tool_with_root, tmp_path)` — [`L226`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_status_tool.py#L226)
  - `test_storage_counters_are_surfaced(self, tool_with_root, tmp_path)` — [`L124`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_status_tool.py#L124)
  - `test_total_edges_reported_for_graph_density(self, tool_with_root, tmp_path)` — [`L159`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_status_tool.py#L159) — total_edges must be present — README 'ahead' claim vs CodeGraph.
  - `test_total_edges_zero_when_edges_absent(self, tool_with_root, tmp_path)` — [`L198`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_status_tool.py#L198) — total_edges defaults to 0 when get_stats omits it (no edges table).

### `TestToolDefinition`
- def: [`tests/unit/test_codegraph_status_tool.py:25`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_status_tool.py#L25)
- signature: `class TestToolDefinition:`
- members:
  - `test_annotations_all_four_hints(self, tool)` — [`L34`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_status_tool.py#L34)
  - `test_description_starts_with_index_health(self, tool)` — [`L30`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_status_tool.py#L30)
  - `test_schema_include_lag_default_true(self, tool)` — [`L50`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_status_tool.py#L50)
  - `test_schema_output_format_default_is_toon(self, tool)` — [`L46`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_status_tool.py#L46)
  - `test_schema_strict_no_additional_properties(self, tool)` — [`L42`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_status_tool.py#L42)
  - `test_tool_name(self, tool)` — [`L26`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_status_tool.py#L26)

### `TestValidateArguments`
- def: [`tests/unit/test_codegraph_status_tool.py:55`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_status_tool.py#L55)
- signature: `class TestValidateArguments:`
- members:
  - `test_empty_args_accepted(self, tool)` — [`L56`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_status_tool.py#L56)
  - `test_include_lag_must_be_bool(self, tool)` — [`L59`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_status_tool.py#L59)

## Functions
- `tool()` — [`L16`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_status_tool.py#L16)
- `tool_with_root(tmp_path)` — [`L21`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_status_tool.py#L21)

