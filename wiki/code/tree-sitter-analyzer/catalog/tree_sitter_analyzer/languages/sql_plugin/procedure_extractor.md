---
title: 'Module: tree_sitter_analyzer/languages/sql_plugin/procedure_extractor.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/sql_plugin/procedure_extractor.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.sql_plugin.procedure_extractor`/
symbols:
  extract_procedure_parameters: extract_procedure_parameters().
  _append_legacy_procedure_match: _append_legacy_procedure_match().
  extract_sql_procedures: extract_sql_procedures().
  _append_legacy_procedures_from_error_node: _append_legacy_procedures_from_error_node().
  extract_legacy_procedures: extract_legacy_procedures().
  _extract_procedure_dependencies: _extract_procedure_dependencies().
  _extract_parameter_section: _extract_parameter_section().
  _split_parameter_definitions: _split_parameter_definitions().
  _has_create_keyword: _has_create_keyword().
---
# Module: [`tree_sitter_analyzer/languages/sql_plugin/procedure_extractor.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/procedure_extractor.py)

## Functions
- `_append_legacy_procedure_match(node: tree_sitter.Node, node_text: str, match: re.Match[str], functions: list[Function])` — [`L187`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/procedure_extractor.py#L187) — Append one legacy procedure Function from a regex match.
- `_append_legacy_procedures_from_error_node(node: tree_sitter.Node, functions: list[Function], get_node_text: Callable[..., str])` — [`L160`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/procedure_extractor.py#L160) — Append legacy Function procedure elements from one ERROR node.
- `_extract_parameter_section(proc_text: str)` — [`L88`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/procedure_extractor.py#L88) — Return the balanced parameter section for a procedure/function.
- `_extract_procedure_dependencies(proc_node: tree_sitter.Node, dependencies: list[str], traverse_nodes: Callable[..., Iterator[Any]], get_node_text: Callable[..., str])` — [`L214`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/procedure_extractor.py#L214) — Extract table dependencies from procedure body.
- `_has_create_keyword(node: tree_sitter.Node)` — [`L179`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/procedure_extractor.py#L179) — Return whether an ERROR node carries a CREATE keyword child.
- `_split_parameter_definitions(param_section: str)` — [`L116`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/procedure_extractor.py#L116) — Split parameter definitions while preserving datatype parentheses.
- `extract_legacy_procedures(root_node: tree_sitter.Node, functions: list[Function], traverse_nodes: Callable[..., Iterator[Any]], get_node_text: Callable[..., str])` — [`L143`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/procedure_extractor.py#L143) — Extract CREATE PROCEDURE statements as generic Function elements.
- `extract_procedure_parameters(proc_text: str, parameters: list[SQLParameter])` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/procedure_extractor.py#L39) — Extract parameters from procedure/function definition.
- `extract_sql_procedures(root_node: tree_sitter.Node, traverse_nodes: Callable[..., Iterator[Any]], get_node_text: Callable[..., str], source_code: str, sql_elements: list[Any])` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/procedure_extractor.py#L19) — Extract CREATE PROCEDURE statements with enhanced metadata.

