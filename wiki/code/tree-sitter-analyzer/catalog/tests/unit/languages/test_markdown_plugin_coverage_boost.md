---
title: 'Module: tests/unit/languages/test_markdown_plugin_coverage_boost.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_markdown_plugin_coverage_boost.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_markdown_plugin_coverage_boost`/
symbols:
  _Node: _Node#
  test_fenced_code_block_extracts_language_and_line_count: test_fenced_code_block_extracts_language_and_line_count().
  test_atx_header_extracts_level_and_text: test_atx_header_extracts_level_and_text().
  test_fenced_code_block_without_language_uses_unknown_name_and_text_language: test_fenced_code_block_without_language_uses_unknown_name_and_text_language().
  test_fenced_code_block_extraction_swallows_single_node_failure: test_fenced_code_block_extraction_swallows_single_node_failure().
  test_list_items_classify_task_ordered_and_unordered_lists: test_list_items_classify_task_ordered_and_unordered_lists().
  test_list_item_extraction_swallows_single_node_failure: test_list_item_extraction_swallows_single_node_failure().
  test_pipe_table_extracts_row_and_column_counts: test_pipe_table_extracts_row_and_column_counts().
  plugin: plugin().
  _Node.__init__: _Node#__init__().
  _Node.raw_text: _Node#raw_text.
  _Node.children: _Node#children.
  _Node.start_point: _Node#start_point.
  _Node.end_point: _Node#end_point.
  test_markdown_plugin_basic: test_markdown_plugin_basic().
---
# Module: [`tests/unit/languages/test_markdown_plugin_coverage_boost.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_coverage_boost.py)

## Classes
### `_Node`
- def: [`tests/unit/languages/test_markdown_plugin_coverage_boost.py:11`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_coverage_boost.py#L11)
- signature: `class _Node:`
- members:
  - `children` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_coverage_boost.py#L23)
  - `end_point` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_coverage_boost.py#L25)
  - `raw_text` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_coverage_boost.py#L22)
  - `start_point` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_coverage_boost.py#L24)
- protocol/private: `__init__`[`L12`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_coverage_boost.py#L12)
- used by: (7 test-only callers)

## Functions
- `plugin()` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_coverage_boost.py#L29)
- `test_atx_header_extracts_level_and_text()` — [`L94`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_coverage_boost.py#L94)
- `test_fenced_code_block_extraction_swallows_single_node_failure()` — [`L149`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_coverage_boost.py#L149)
- `test_fenced_code_block_extracts_language_and_line_count()` — [`L63`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_coverage_boost.py#L63)
- `test_fenced_code_block_without_language_uses_unknown_name_and_text_language()` — [`L120`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_coverage_boost.py#L120)
- `test_list_item_extraction_swallows_single_node_failure()` — [`L198`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_coverage_boost.py#L198)
- `test_list_items_classify_task_ordered_and_unordered_lists()` — [`L165`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_coverage_boost.py#L165)
- `test_markdown_plugin_basic(plugin)` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_coverage_boost.py#L33)
- `test_pipe_table_extracts_row_and_column_counts()` — [`L218`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_coverage_boost.py#L218)

