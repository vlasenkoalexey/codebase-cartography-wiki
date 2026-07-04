---
title: 'Module: tree_sitter_analyzer/cli/commands/table_command.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/cli/commands/table_command.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.cli.commands.table_command`/
symbols:
  TableCommand._convert_to_structure_format: TableCommand#_convert_to_structure_format().
  TableCommand: TableCommand#
  TableCommand._render_table_output: TableCommand#_render_table_output().
  TableCommand.execute_async: TableCommand#execute_async().
  TableCommand._format_as_toon: TableCommand#_format_as_toon().
  TableCommand._convert_function_element: TableCommand#_convert_function_element().
  _attach_table_envelope: _attach_table_envelope().
  TableCommand._render_table_json: TableCommand#_render_table_json().
  TableCommand._convert_variable_element: TableCommand#_convert_variable_element().
  TableCommand._convert_sql_element: TableCommand#_convert_sql_element().
  TableCommand._resolve_table_type: TableCommand#_resolve_table_type().
  TableCommand._convert_to_toon_format: TableCommand#_convert_to_toon_format().
  TableCommand._process_parameters: TableCommand#_process_parameters().
  TableCommand.__init__: TableCommand#__init__().
  TableCommand._convert_to_formatter_format: TableCommand#_convert_to_formatter_format().
  TableCommand._get_default_package_name: TableCommand#_get_default_package_name().
  TableCommand._get_element_visibility: TableCommand#_get_element_visibility().
  TableCommand._convert_class_element: TableCommand#_convert_class_element().
  TableCommand._convert_import_element: TableCommand#_convert_import_element().
  TableCommand._process_sql_parameters: TableCommand#_process_sql_parameters().
  TableCommand._output_table: TableCommand#_output_table().
---
# Module: [`tree_sitter_analyzer/cli/commands/table_command.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/table_command.py)

## Classes
### `TableCommand`  ·  implements/extends BaseCommand
- def: [`tree_sitter_analyzer/cli/commands/table_command.py:61`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/table_command.py#L61)
- doc: Command for generating table format output.
- signature: `class TableCommand(BaseCommand):`
- members:
  - `__init__(self, args: Any)` — [`L64`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/table_command.py#L64) — Initialize the table command.
  - `_convert_class_element(self, element: Any, index: int, language: str)` — [`L316`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/table_command.py#L316) — Convert class element to table format.
  - `_convert_function_element(self, element: Any, language: str)` — [`L342`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/table_command.py#L342) — Convert function element to table format.
  - `_convert_import_element(self, element: Any)` — [`L418`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/table_command.py#L418) — Convert import element to table format.
  - `_convert_sql_element(self, element: Any, language: str)` — [`L457`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/table_command.py#L457) — Convert SQL element to table format.
  - `_convert_to_formatter_format(self, analysis_result: Any)` — [`L239`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/table_command.py#L239) — Convert AnalysisResult to format expected by formatters.
  - `_convert_to_structure_format(self, analysis_result: Any, language: str)` — [`L292`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/table_command.py#L292) — Convert AnalysisResult to the format expected by table formatter.
  - `_convert_to_toon_format(self, analysis_result: Any)` — [`L234`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/table_command.py#L234) — Convert AnalysisResult to TOON-friendly format with position info.
  - `_convert_variable_element(self, element: Any, language: str)` — [`L378`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/table_command.py#L378) — Convert variable element to table format.
  - `_format_as_toon(self, analysis_result: Any, effective_table: str | None = None, requested_table: str | None = None)` — [`L207`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/table_command.py#L207) — Format analysis result as TOON.
  - `_get_default_package_name(self, language: str)` — [`L276`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/table_command.py#L276) — Get default package name for language.
  - `_get_element_visibility(self, element: Any)` — [`L513`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/table_command.py#L513) — Get element visibility.
  - `_output_table(self, table_output: str)` — [`L522`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/table_command.py#L522) — Output the table with proper encoding.
  - `_process_parameters(self, params: Any, language: str)` — [`L509`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/table_command.py#L509) — Process parameters based on language syntax.
  - `_process_sql_parameters(self, params: Any)` — [`L491`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/table_command.py#L491) — Process SQL parameters.
  - `_render_table_json(self, analysis_result: Any, language: str, table_type: str, user_table_request: str, table_was_user_specified: bool)` — [`L178`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/table_command.py#L178) — Build the JSON envelope with K11 metadata + r37ab canonical envelope.
  - `_render_table_output(self, analysis_result: Any, language: str, table_type: str, user_table_request: str, table_was_user_specified: bool)` — [`L137`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/table_command.py#L137) — Render the table output string per ``table_type`` (json/toon/text).
  - `_resolve_table_type(self)` — [`L98`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/table_command.py#L98) — Pick the effective table view, honouring ``--format`` overrides.
  - `execute_async(self, language: str)` — [`L69`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/table_command.py#L69) — Execute table format generation.
- uses (calls/refs, reference-scoped): [`FormatterRegistry`](../../formatters/formatter_registry.md#FormatterRegistry), [`ToonFormatter`](../../formatters/toon_formatter.md#ToonFormatter), [`args`](base_command.md#BaseCommand.args), [`output_error`](../../output_manager.md#output_error), [`get_formatter_for_language`](../../formatters/formatter_registry.md#FormatterRegistry.get_formatter_for_language), [`BaseCommand`](base_command.md#BaseCommand), [`format`](../../formatters/toon_formatter.md#ToonFormatter.format), [`analyze_file`](base_command.md#BaseCommand.analyze_file), [`get_element_type`](../../constants.md#get_element_type), [`process_parameters`](table_command_helpers.md#process_parameters), [`_attach_table_envelope`](table_command.md#_attach_table_envelope), [`collect_structure_elements`](table_command_helpers.md#collect_structure_elements), [`convert_to_toon_format`](table_command_helpers.md#convert_to_toon_format), [`get_default_package_name`](table_command_helpers.md#get_default_package_name), [`resolve_structure_package_name`](table_command_helpers.md#resolve_structure_package_name), [`StructureConverters`](table_command_helpers.md#StructureConverters), [`__init__`](base_command.md#BaseCommand.__init__), [`build_structure_format`](table_command_helpers.md#build_structure_format), [`class_element`](table_command_helpers.md#StructureConverters.class_element), [`function_element`](table_command_helpers.md#StructureConverters.function_element), [`import_element`](table_command_helpers.md#StructureConverters.import_element), [`sql_element`](table_command_helpers.md#StructureConverters.sql_element), [`variable_element`](table_command_helpers.md#StructureConverters.variable_element)
- used by: [`BaseCommand`](base_command.md#BaseCommand), [`execute_async`](base_command.md#BaseCommand.execute_async), [`_create_file_command`](../../cli_main.md#_create_file_command)  (8 test-only)

## Functions
- `_attach_table_envelope(data: dict[str, Any], analysis_result: Any)` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/table_command.py#L27) — Attach canonical envelope keys to a ``--table json`` response.

