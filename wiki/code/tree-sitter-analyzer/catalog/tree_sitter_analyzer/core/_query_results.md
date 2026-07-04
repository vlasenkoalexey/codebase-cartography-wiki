---
title: 'Module: tree_sitter_analyzer/core/_query_results.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/core/_query_results.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.core._query_results`/
symbols:
  process_captures: process_captures().
  _unpack_capture: _unpack_capture().
  create_result_dict: create_result_dict().
  _process_capture: _process_capture().
  create_error_result: create_error_result().
  query_statistics: query_statistics().
  logger: logger.
  TextExtractor: TextExtractor.
---
# Module: [`tree_sitter_analyzer/core/_query_results.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_query_results.py)

## Functions
- `_process_capture(capture: Any, source_code: str, create_result_dict: Callable[[Any, str, str], dict[str, Any]])` — [`L35`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_query_results.py#L35)
- `_unpack_capture(capture: Any)` — [`L54`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_query_results.py#L54)
- `create_error_result(error_message: str, query_name: str | None = None, **kwargs: Any)` — [`L87`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_query_results.py#L87) — Create an error result dictionary.
- `create_result_dict(node: Node, capture_name: str, source_code: str, get_node_text: TextExtractor)` — [`L65`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_query_results.py#L65) — Create a result dictionary from a Tree-sitter node.
- `process_captures(captures: Any, source_code: str, create_result_dict: Callable[[Any, str, str], dict[str, Any]])` — [`L16`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_query_results.py#L16) — Process query captures into standardized dictionaries.
- `query_statistics(stats: dict[str, Any])` — [`L100`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_query_results.py#L100) — Return query execution statistics with derived rates.

## Module values
- `TextExtractor` — [`L13`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_query_results.py#L13)
- `logger` — [`L11`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_query_results.py#L11)

