---
title: 'Module: tree_sitter_analyzer/formatters/_go_formatter_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/formatters/_go_formatter_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.formatters._go_formatter_helpers`/
symbols:
  format_go_full_table: format_go_full_table().
  _append_type_sections: _append_type_sections().
  _append_function_sections: _append_function_sections().
  VisibilityResolver: VisibilityResolver.
  _append_structs: _append_structs().
  _append_interfaces: _append_interfaces().
  _append_variable_sections: _append_variable_sections().
  _append_variables: _append_variables().
  DocExtractor: DocExtractor.
  _append_type_aliases: _append_type_aliases().
  _append_functions: _append_functions().
  _append_methods: _append_methods().
  FunctionRowFormatter: FunctionRowFormatter.
  MethodRowFormatter: MethodRowFormatter.
  _is_go_method: _is_go_method().
  PackageNameExtractor: PackageNameExtractor.
  _append_header: _append_header().
  _append_package_info: _append_package_info().
  _append_imports: _append_imports().
---
# Module: [`tree_sitter_analyzer/formatters/_go_formatter_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_go_formatter_helpers.py)

## Functions
- `_append_function_sections(lines: list[str], functions: list[dict[str, Any]], format_func_row: FunctionRowFormatter, format_method_row: MethodRowFormatter)` — [`L170`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_go_formatter_helpers.py#L170)
- `_append_functions(lines: list[str], funcs: list[dict[str, Any]], format_func_row: FunctionRowFormatter)` — [`L187`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_go_formatter_helpers.py#L187)
- `_append_header(lines: list[str], data: dict[str, Any], package_name: str)` — [`L47`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_go_formatter_helpers.py#L47)
- `_append_imports(lines: list[str], imports: list[dict[str, Any]])` — [`L71`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_go_formatter_helpers.py#L71)
- `_append_interfaces(lines: list[str], interfaces: list[dict[str, Any]], go_visibility: VisibilityResolver, extract_doc_summary: DocExtractor)` — [`L130`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_go_formatter_helpers.py#L130)
- `_append_methods(lines: list[str], methods: list[dict[str, Any]], format_method_row: MethodRowFormatter)` — [`L203`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_go_formatter_helpers.py#L203)
- `_append_package_info(lines: list[str], data: dict[str, Any], package_name: str)` — [`L56`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_go_formatter_helpers.py#L56)
- `_append_structs(lines: list[str], structs: list[dict[str, Any]], go_visibility: VisibilityResolver, extract_doc_summary: DocExtractor)` — [`L105`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_go_formatter_helpers.py#L105)
- `_append_type_aliases(lines: list[str], type_aliases: list[dict[str, Any]], go_visibility: VisibilityResolver)` — [`L151`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_go_formatter_helpers.py#L151)
- `_append_type_sections(lines: list[str], classes: list[dict[str, Any]], go_visibility: VisibilityResolver, extract_doc_summary: DocExtractor)` — [`L90`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_go_formatter_helpers.py#L90)
- `_append_variable_sections(lines: list[str], variables: list[dict[str, Any]], go_visibility: VisibilityResolver)` — [`L219`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_go_formatter_helpers.py#L219)
- `_append_variables(lines: list[str], title: str, variables: list[dict[str, Any]], go_visibility: VisibilityResolver)` — [`L233`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_go_formatter_helpers.py#L233)
- `_is_go_method(func: dict[str, Any])` — [`L183`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_go_formatter_helpers.py#L183)
- `format_go_full_table(data: dict[str, Any], get_package_name: PackageNameExtractor, go_visibility: VisibilityResolver, extract_doc_summary: DocExtractor, format_func_row: FunctionRowFormatter, format_method_row: MethodRowFormatter)` — [`L13`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_go_formatter_helpers.py#L13) — Format full Go output while keeping section assembly isolated.

## Module values
- `DocExtractor` — [`L6`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_go_formatter_helpers.py#L6)
- `FunctionRowFormatter` — [`L7`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_go_formatter_helpers.py#L7)
- `MethodRowFormatter` — [`L8`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_go_formatter_helpers.py#L8)
- `PackageNameExtractor` — [`L9`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_go_formatter_helpers.py#L9)
- `VisibilityResolver` — [`L10`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_go_formatter_helpers.py#L10)

