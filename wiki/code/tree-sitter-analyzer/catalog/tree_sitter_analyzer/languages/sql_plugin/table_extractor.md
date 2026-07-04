---
title: 'Module: tree_sitter_analyzer/languages/sql_plugin/table_extractor.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/sql_plugin/table_extractor.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.sql_plugin.table_extractor`/
symbols:
  fill_missing_sql_tables_from_regex: fill_missing_sql_tables_from_regex().
  extract_sql_tables: extract_sql_tables().
  _parse_column_definition: _parse_column_definition().
  _process_column_node: _process_column_node().
  extract_table_columns: extract_table_columns().
  _parse_columns_from_raw_text: _parse_columns_from_raw_text().
  _is_in_sql_comment: _is_in_sql_comment().
  _split_column_definitions: _split_column_definitions().
  _CREATE_TABLE_RE: _CREATE_TABLE_RE.
  _find_table_name: _find_table_name().
  _last_valid_identifier: _last_valid_identifier().
  _QUOTED_OR_BARE: _QUOTED_OR_BARE.
  _strip_sql_delimiters: _strip_sql_delimiters().
  _find_statement_end_line: _find_statement_end_line().
  _extract_statement_text: _extract_statement_text().
---
# Module: [`tree_sitter_analyzer/languages/sql_plugin/table_extractor.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/table_extractor.py)

## Functions
- `_extract_statement_text(source: str, start: int)` — [`L279`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/table_extractor.py#L279) — Return the full CREATE TABLE statement text starting at ``start``.
- `_find_statement_end_line(source: str, start: int)` — [`L265`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/table_extractor.py#L265) — Return the 1-based line number of the closing ``;`` for the statement at ``start``.
- `_find_table_name(create_table_node: tree_sitter.Node, get_node_text: Callable[..., str])` — [`L74`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/table_extractor.py#L74) — Walk a ``create_table`` AST node and return (table_name, schema_name).
- `_is_in_sql_comment(source: str, pos: int)` — [`L181`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/table_extractor.py#L181) — Return True if ``pos`` falls inside a SQL line (``--``) or block (``/* */``) comment.
- `_last_valid_identifier(object_reference: tree_sitter.Node, get_node_text: Callable[..., str])` — [`L96`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/table_extractor.py#L96) — Return (table_name, schema_name) from an ``object_reference`` node.
- `_parse_column_definition(col_def: str)` — [`L348`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/table_extractor.py#L348) — Parse a single column definition string.
- `_parse_columns_from_raw_text(raw_text: str)` — [`L293`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/table_extractor.py#L293) — Extract SQLColumn list from a CREATE TABLE raw text string (#880).
- `_process_column_node(node: Any, columns: list[SQLColumn], get_node_text: Callable[..., str])` — [`L119`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/table_extractor.py#L119) — Process one tree-sitter ``column_definition`` node into *columns*.
- `_split_column_definitions(content: str)` — [`L322`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/table_extractor.py#L322) — Split column definitions by commas, handling nested parentheses.
- `_strip_sql_delimiters(name: str)` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/table_extractor.py#L30) — Strip ANSI/MySQL/SQL Server identifier delimiters from a quoted name.
- `extract_sql_tables(root_node: tree_sitter.Node, traverse_nodes: Callable[..., Iterator[Any]], get_node_text: Callable[..., str], sql_elements: list[Any])` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/table_extractor.py#L37) — Extract CREATE TABLE statements with enhanced metadata.
- `extract_table_columns(table_node: tree_sitter.Node, columns: list[SQLColumn], constraints: list[SQLConstraint], traverse_nodes: Callable[..., Iterator[Any]], get_node_text: Callable[..., str])` — [`L152`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/table_extractor.py#L152) — Extract column definitions from CREATE TABLE statement.
- `fill_missing_sql_tables_from_regex(source_code: str, sql_elements: list[Any])` — [`L196`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/table_extractor.py#L196) — Regex fallback: add CREATE TABLE statements absorbed by ERROR nodes (#808). — documented in [tree_sitter_analyzer-models-sql_models](../../../../concepts/tree_sitter_analyzer-models-sql_models.md)

## Module values
- `_CREATE_TABLE_RE` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/table_extractor.py#L22)
- `_QUOTED_OR_BARE` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/table_extractor.py#L21)

