---
title: 'Module: tree_sitter_analyzer/cli/commands/table_command_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/cli/commands/table_command_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.cli.commands.table_command_helpers`/
symbols:
  _append_structure_element: _append_structure_element().
  _append_toon_element: _append_toon_element().
  _process_single_parameter: _process_single_parameter().
  process_parameters: process_parameters().
  STRUCTURE_SQL_ELEMENT_TYPES: STRUCTURE_SQL_ELEMENT_TYPES.
  _toon_package_info: _toon_package_info().
  convert_to_toon_format: convert_to_toon_format().
  collect_structure_elements: collect_structure_elements().
  get_default_package_name: get_default_package_name().
  resolve_structure_package_name: resolve_structure_package_name().
  StructureConverters: StructureConverters#
  _line_range_tuple: _line_range_tuple().
  _process_type_prefix_parameter: _process_type_prefix_parameter().
  _toon_class: _toon_class().
  _toon_method: _toon_method().
  _toon_field: _toon_field().
  TYPE_SUFFIX_LANGUAGES: TYPE_SUFFIX_LANGUAGES.
  StructureConverters.class_element: StructureConverters#class_element.
  StructureConverters.function_element: StructureConverters#function_element.
  StructureConverters.variable_element: StructureConverters#variable_element.
  StructureConverters.import_element: StructureConverters#import_element.
  StructureConverters.sql_element: StructureConverters#sql_element.
  build_structure_format: build_structure_format().
  GO_LANGUAGES: GO_LANGUAGES.
  PACKAGED_LANGUAGES: PACKAGED_LANGUAGES.
  _toon_import: _toon_import().
  _process_string_parameters: _process_string_parameters().
  _process_go_parameter: _process_go_parameter().
  _process_type_suffix_parameter: _process_type_suffix_parameter().
---
# Module: [`tree_sitter_analyzer/cli/commands/table_command_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/table_command_helpers.py)

## Classes
### `StructureConverters`
- def: [`tree_sitter_analyzer/cli/commands/table_command_helpers.py:58`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/table_command_helpers.py#L58)
- doc: Callable adapters used to preserve TableCommand conversion behavior.
- signature: `class StructureConverters:`
- members:
  - `class_element` — [`L61`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/table_command_helpers.py#L61)
  - `function_element` — [`L62`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/table_command_helpers.py#L62)
  - `import_element` — [`L64`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/table_command_helpers.py#L64)
  - `sql_element` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/table_command_helpers.py#L65)
  - `variable_element` — [`L63`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/table_command_helpers.py#L63)
- used by: [`_convert_to_structure_format`](table_command.md#TableCommand._convert_to_structure_format), [`_append_structure_element`](table_command_helpers.md#_append_structure_element), [`collect_structure_elements`](table_command_helpers.md#collect_structure_elements)

## Functions
- `_append_structure_element(element: Any, index: int, language: str, package_name: str, converters: StructureConverters, classes: list[dict[str, Any]], methods: list[dict[str, Any]], fields: list[dict[str, Any]], imports: list[dict[str, Any]])` — [`L202`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/table_command_helpers.py#L202) — Append one parsed element to the matching table structure collection.
- `_append_toon_element(element: Any, classes: list[dict[str, Any]], methods: list[dict[str, Any]], fields: list[dict[str, Any]], imports: list[dict[str, Any]])` — [`L183`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/table_command_helpers.py#L183) — Append one element to the matching TOON collection.
- `_line_range_tuple(element: Any)` — [`L300`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/table_command_helpers.py#L300) — Return tuple line range used by TOON output.
- `_process_go_parameter(param: str)` — [`L332`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/table_command_helpers.py#L332) — Process a Go parameter string: name-before-type, space-separated.
- `_process_single_parameter(param: Any, language: str)` — [`L316`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/table_command_helpers.py#L316) — Process one parameter item from parser output.
- `_process_string_parameters(params: str)` — [`L308`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/table_command_helpers.py#L308) — Split comma-delimited parameter text into Any-typed names.
- `_process_type_prefix_parameter(param: str)` — [`L365`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/table_command_helpers.py#L365) — Process type-first parameter syntax, such as Java.
- `_process_type_suffix_parameter(param: str)` — [`L350`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/table_command_helpers.py#L350) — Process name-first parameter syntax, such as Python or TypeScript.
- `_toon_class(element: Any)` — [`L230`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/table_command_helpers.py#L230) — Convert a class element to TOON shape.
- `_toon_field(element: Any)` — [`L248`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/table_command_helpers.py#L248) — Convert a variable element to TOON shape.
- `_toon_import(element: Any)` — [`L257`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/table_command_helpers.py#L257) — Convert an import element to TOON shape.
- `_toon_method(element: Any)` — [`L239`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/table_command_helpers.py#L239) — Convert a function element to TOON shape.
- `_toon_package_info(elements: list[Any])` — [`L288`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/table_command_helpers.py#L288) — Return the first package element in TOON shape.
- `build_structure_format(analysis_result: Any, package_name: str, classes: list[dict[str, Any]], methods: list[dict[str, Any]], fields: list[dict[str, Any]], imports: list[dict[str, Any]])` — [`L147`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/table_command_helpers.py#L147) — Build the final table formatter structure payload.
- `collect_structure_elements(analysis_result: Any, language: str, package_name: str, converters: StructureConverters, report_error: Callable[[str], None])` — [`L109`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/table_command_helpers.py#L109) — Collect classes, methods, fields, and imports for table structure output.
- `convert_to_toon_format(analysis_result: Any)` — [`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/table_command_helpers.py#L68) — Convert AnalysisResult to TOON-friendly format with position info.
- `get_default_package_name(language: str)` — [`L96`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/table_command_helpers.py#L96) — Return the default package name for language-specific table output.
- `process_parameters(params: Any, language: str)` — [`L174`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/table_command_helpers.py#L174) — Process parameters based on language syntax.
- `resolve_structure_package_name(analysis_result: Any, language: str)` — [`L101`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/table_command_helpers.py#L101) — Resolve the package name for table formatter structure output.

## Module values
- `GO_LANGUAGES` — [`L44`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/table_command_helpers.py#L44)
- `PACKAGED_LANGUAGES` — [`L46`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/table_command_helpers.py#L46)
- `STRUCTURE_SQL_ELEMENT_TYPES` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/table_command_helpers.py#L47)
- `TYPE_SUFFIX_LANGUAGES` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/table_command_helpers.py#L24)

