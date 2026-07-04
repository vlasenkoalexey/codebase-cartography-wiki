---
title: 'Module: tests/unit/test_codegraph_metrics_tool.py'
type: catalog
provenance: extracted
module: tests/unit/test_codegraph_metrics_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_codegraph_metrics_tool`/
symbols:
  TestCallGraphMetricsSanity.test_dead_code_candidates_never_equals_total: TestCallGraphMetricsSanity#test_dead_code_candidates_never_equals_total().
  TestCallGraphMetricsSanity.test_files_with_functions_reflects_real_paths: TestCallGraphMetricsSanity#test_files_with_functions_reflects_real_paths().
  TestCallGraphMetricsSanity._index: TestCallGraphMetricsSanity#_index().
  tool: tool().
  tool_with_root: tool_with_root().
  TestToolDefinition: TestToolDefinition#
  TestToolDefinition.test_tool_name: TestToolDefinition#test_tool_name().
  TestToolDefinition.test_description_mentions_codegraph_parity: TestToolDefinition#test_description_mentions_codegraph_parity().
  TestToolDefinition.test_schema_has_sections_and_output_format: TestToolDefinition#test_schema_has_sections_and_output_format().
  TestToolDefinition.test_schema_sections_enum: TestToolDefinition#test_schema_sections_enum().
  TestToolDefinition.test_annotations_readonly: TestToolDefinition#test_annotations_readonly().
  TestValidation: TestValidation#
  TestValidation.test_valid_no_sections: TestValidation#test_valid_no_sections().
  TestValidation.test_valid_subset_sections: TestValidation#test_valid_subset_sections().
  TestValidation.test_rejects_unknown_section: TestValidation#test_rejects_unknown_section().
  TestExecuteNoCache: TestExecuteNoCache#
  TestExecuteNoCache.test_no_project_root_returns_info: TestExecuteNoCache#test_no_project_root_returns_info().
  TestExecuteNoCache.test_cache_empty_section_hint: TestExecuteNoCache#test_cache_empty_section_hint().
  TestExecuteNoCache.test_toon_format_default: TestExecuteNoCache#test_toon_format_default().
  TestExecuteNoCache.test_sections_included_field: TestExecuteNoCache#test_sections_included_field().
  TestExecuteWithCache: TestExecuteWithCache#
  TestExecuteWithCache.test_cache_section_populated_when_indexed: TestExecuteWithCache#test_cache_section_populated_when_indexed().
  TestCallGraphMetricsSanity: TestCallGraphMetricsSanity#
---
# Module: [`tests/unit/test_codegraph_metrics_tool.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_metrics_tool.py)

## Classes
### `TestCallGraphMetricsSanity`
- def: [`tests/unit/test_codegraph_metrics_tool.py:124`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_metrics_tool.py#L124)
- doc: F1 regression: project metrics must not degenerate to 'every function is
- signature: `class TestCallGraphMetricsSanity:`
- members:
  - `test_dead_code_candidates_never_equals_total(self, tmp_path)` — [`L146`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_metrics_tool.py#L146)
  - `test_files_with_functions_reflects_real_paths(self, tmp_path)` — [`L162`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_metrics_tool.py#L162)
- protocol/private: `_index`[`L132`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_metrics_tool.py#L132)
- uses (calls/refs, reference-scoped): [`ASTCache`](../../tree_sitter_analyzer/ast_cache.md#ASTCache), [`index_project`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.index_project), [`_collect_call_graph_metrics`](../../tree_sitter_analyzer/mcp/tools/codegraph_metrics_tool.md#CodeGraphMetricsTool._collect_call_graph_metrics), [`CodeGraphMetricsTool`](../../tree_sitter_analyzer/mcp/tools/codegraph_metrics_tool.md#CodeGraphMetricsTool)

### `TestExecuteNoCache`
- def: [`tests/unit/test_codegraph_metrics_tool.py:65`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_metrics_tool.py#L65)
- signature: `class TestExecuteNoCache:`
- members:
  - `test_cache_empty_section_hint(self, tool_with_root)` — [`L71`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_metrics_tool.py#L71)
  - `test_no_project_root_returns_info(self, tool)` — [`L66`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_metrics_tool.py#L66)
  - `test_sections_included_field(self, tool_with_root)` — [`L87`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_metrics_tool.py#L87)
  - `test_toon_format_default(self, tool)` — [`L82`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_metrics_tool.py#L82)

### `TestExecuteWithCache`
- def: [`tests/unit/test_codegraph_metrics_tool.py:99`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_metrics_tool.py#L99)
- signature: `class TestExecuteWithCache:`
- members:
  - `test_cache_section_populated_when_indexed(self, tool_with_root)` — [`L100`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_metrics_tool.py#L100)

### `TestToolDefinition`
- def: [`tests/unit/test_codegraph_metrics_tool.py:22`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_metrics_tool.py#L22)
- signature: `class TestToolDefinition:`
- members:
  - `test_annotations_readonly(self, tool)` — [`L46`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_metrics_tool.py#L46)
  - `test_description_mentions_codegraph_parity(self, tool)` — [`L26`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_metrics_tool.py#L26)
  - `test_schema_has_sections_and_output_format(self, tool)` — [`L30`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_metrics_tool.py#L30)
  - `test_schema_sections_enum(self, tool)` — [`L36`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_metrics_tool.py#L36)
  - `test_tool_name(self, tool)` — [`L23`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_metrics_tool.py#L23)

### `TestValidation`
- def: [`tests/unit/test_codegraph_metrics_tool.py:52`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_metrics_tool.py#L52)
- signature: `class TestValidation:`
- members:
  - `test_rejects_unknown_section(self, tool)` — [`L59`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_metrics_tool.py#L59)
  - `test_valid_no_sections(self, tool)` — [`L53`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_metrics_tool.py#L53)
  - `test_valid_subset_sections(self, tool)` — [`L56`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_metrics_tool.py#L56)

## Functions
- `tool()` — [`L13`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_metrics_tool.py#L13)
- `tool_with_root(tmp_path)` — [`L18`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_metrics_tool.py#L18)

