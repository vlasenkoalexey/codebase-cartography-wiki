---
title: 'Module: tree_sitter_analyzer/languages/typescript_plugin/import_extractor.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/typescript_plugin/import_extractor.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.typescript_plugin.import_extractor`/
symbols:
  _build_import_info: _build_import_info().
  _extract_dynamic_import: _extract_dynamic_import().
  _build_commonjs_require_import: _build_commonjs_require_import().
  extract_ts_imports: extract_ts_imports().
  _extract_commonjs_requires: _extract_commonjs_requires().
  _extract_import_child_names: _extract_import_child_names().
  _extract_import_names: _extract_import_names().
  _extract_import_info_simple: _extract_import_info_simple().
  _extract_import_statement_parts: _extract_import_statement_parts().
  _build_commonjs_require_imports: _build_commonjs_require_imports().
  _extract_identifier_names: _extract_identifier_names().
  _extract_named_import_names: _extract_named_import_names().
  _extract_namespace_import_names: _extract_namespace_import_names().
  _iter_typed_children: _iter_typed_children().
  _extract_identifier_text: _extract_identifier_text().
  _COMMONJS_REQUIRE_PATTERN: _COMMONJS_REQUIRE_PATTERN.
  _node_line_range: _node_line_range().
  _extract_node_text: _extract_node_text().
  _extract_string_literal: _extract_string_literal().
  _extract_dynamic_import_source: _extract_dynamic_import_source().
  _touch_root_text: _touch_root_text().
---
# Module: [`tree_sitter_analyzer/languages/typescript_plugin/import_extractor.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/import_extractor.py)

## Functions
- `_build_commonjs_require_import(source_code: str, match: re.Match[str])` — [`L308`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/import_extractor.py#L308)
- `_build_commonjs_require_imports(source_code: str)` — [`L299`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/import_extractor.py#L299)
- `_build_import_info(node: Any, source_code: str, get_node_text: Callable[..., str])` — [`L56`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/import_extractor.py#L56)
- `_extract_commonjs_requires(tree: Any, source_code: str, get_node_text: Callable[..., str])` — [`L279`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/import_extractor.py#L279) — Extract CommonJS require() statements (for compatibility).
- `_extract_dynamic_import(node: Any, get_node_text: Callable[..., str])` — [`L240`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/import_extractor.py#L240) — Extract dynamic import() calls.
- `_extract_dynamic_import_source(node_text: str)` — [`L266`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/import_extractor.py#L266)
- `_extract_identifier_names(node: Any, source_bytes: bytes)` — [`L187`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/import_extractor.py#L187)
- `_extract_identifier_text(node: Any, source_bytes: bytes)` — [`L227`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/import_extractor.py#L227) — Extract text from an identifier node.
- `_extract_import_child_names(child: Any, source_bytes: bytes, get_node_text: Callable[..., str])` — [`L127`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/import_extractor.py#L127)
- `_extract_import_info_simple(node: Any, source_code: str, get_node_text: Callable[..., str])` — [`L42`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/import_extractor.py#L42) — Extract import information from import_statement node.
- `_extract_import_names(import_clause_node: Any, source_code: str, get_node_text: Callable[..., str])` — [`L85`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/import_extractor.py#L85) — Extract import names from import clause.
- `_extract_import_statement_parts(node: Any, source_code: str, get_node_text: Callable[..., str])` — [`L106`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/import_extractor.py#L106)
- `_extract_named_import_names(node: Any, source_bytes: bytes, get_node_text: Callable[..., str])` — [`L199`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/import_extractor.py#L199)
- `_extract_namespace_import_names(node: Any, source_bytes: bytes)` — [`L214`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/import_extractor.py#L214)
- `_extract_node_text(node: Any, source_code: str, get_node_text: Callable[..., str])` — [`L152`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/import_extractor.py#L152)
- `_extract_string_literal(node: Any, source_code: str)` — [`L172`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/import_extractor.py#L172)
- `_iter_typed_children(node: Any)` — [`L166`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/import_extractor.py#L166)
- `_node_line_range(node: Any)` — [`L146`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/import_extractor.py#L146)
- `_touch_root_text(tree: Any, get_node_text: Callable[..., str])` — [`L294`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/import_extractor.py#L294)
- `extract_ts_imports(tree: Any, source_code: str, get_node_text: Callable[..., str])` — [`L16`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/import_extractor.py#L16) — Extract TypeScript import statements with ES6+ and type import support.

## Module values
- `_COMMONJS_REQUIRE_PATTERN` — [`L10`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/import_extractor.py#L10)

