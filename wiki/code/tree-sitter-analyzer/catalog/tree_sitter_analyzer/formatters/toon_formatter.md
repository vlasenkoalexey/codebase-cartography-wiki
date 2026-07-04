---
title: 'Module: tree_sitter_analyzer/formatters/toon_formatter.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/formatters/toon_formatter.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.formatters.toon_formatter`/
symbols:
  ToonFormatter: ToonFormatter#
  ToonFormatter.format_analysis_result: ToonFormatter#format_analysis_result().
  ToonFormatter.format: ToonFormatter#format().
  ToonFormatter._format_internal: ToonFormatter#_format_internal().
  ToonFormatter.is_toon_content: ToonFormatter#is_toon_content().
  ToonFormatter.encoder: ToonFormatter#encoder.
  ToonFormatter._emit_method_lines: ToonFormatter#_emit_method_lines().
  ToonFormatter.format_structure: ToonFormatter#format_structure().
  ToonFormatter.format_summary: ToonFormatter#format_summary().
  ToonFormatter.format_advanced: ToonFormatter#format_advanced().
  ToonFormatter.format_table: ToonFormatter#format_table().
  ToonFormatter._is_mcp_response: ToonFormatter#_is_mcp_response().
  ToonFormatter.format_mcp_response: ToonFormatter#format_mcp_response().
  logger: logger.
  ToonFormatter._method_to_dict: ToonFormatter#_method_to_dict().
  ToonFormatter.use_tabs: ToonFormatter#use_tabs.
  ToonFormatter.compact_arrays: ToonFormatter#compact_arrays.
  ToonFormatter.include_metadata: ToonFormatter#include_metadata.
  ToonFormatter.fallback_to_json: ToonFormatter#fallback_to_json.
  ToonFormatter._emit_class_lines: ToonFormatter#_emit_class_lines().
  ToonFormatter._emit_function_lines: ToonFormatter#_emit_function_lines().
  ToonFormatter.__init__: ToonFormatter#__init__().
  ToonFormatter.normalize_paths: ToonFormatter#normalize_paths.
---
# Module: [`tree_sitter_analyzer/formatters/toon_formatter.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_formatter.py)

## Classes
### `ToonFormatter`  ·  implements/extends BaseFormatter
- def: [`tree_sitter_analyzer/formatters/toon_formatter.py:19`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_formatter.py#L19) — documented in [tree_sitter_analyzer-mcp-tools-read_partial_tool](../../../concepts/tree_sitter_analyzer-mcp-tools-read_partial_tool.md)
- doc: TOON formatter for LLM-optimized output.
- signature: `class ToonFormatter(BaseFormatter):`
- members:
  - `__init__(self, use_tabs: bool = False, compact_arrays: bool = True, include_metadata: bool = True, fallback_to_json: bool = True, normalize_paths: bool = True)` — [`L30`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_formatter.py#L30) — Initialize TOON formatter.
  - `_emit_class_lines(lines: list[str], classes: list[Any])` — [`L197`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_formatter.py#L197) — Append ``classes[N]:`` header + ``- name`` lines for each class.
  - `_emit_function_lines(lines: list[str], functions: list[Any])` — [`L225`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_formatter.py#L225) — Append ``functions[N]:`` header + first-10 names.
  - `_emit_method_lines(self, lines: list[str], methods: list[Any])` — [`L205`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_formatter.py#L205) — Append ``methods[N]:`` block (compact-table or simple name list).
  - `_format_internal(self, data: Any)` — [`L91`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_formatter.py#L91) — Internal format method without error handling wrapper. — documented in [tree_sitter_analyzer-formatters-toon_encoder](../../../concepts/tree_sitter_analyzer-formatters-toon_encoder.md)
  - `_is_mcp_response(self, data: dict[str, Any])` — [`L122`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_formatter.py#L122) — Detect if data is an MCP response structure.
  - `_method_to_dict(self, method: Any)` — [`L301`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_formatter.py#L301) — Convert method element to dictionary for table encoding.
  - `format(self, data: Any)` — [`L60`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_formatter.py#L60) — Unified format method implementing the Formatter protocol.
  - `format_advanced(self, analysis_result: dict[str, Any], output_format: str = "toon")` — [`L271`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_formatter.py#L271) — Format advanced analysis output (BaseFormatter requirement).
  - `format_analysis_result(self, result: Any, table_type: str = "full")` — [`L137`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_formatter.py#L137) — Format complete analysis result as TOON. — documented in [tree_sitter_analyzer-formatters-toon_encoder](../../../concepts/tree_sitter_analyzer-formatters-toon_encoder.md)
  - `format_mcp_response(self, data: dict[str, Any])` — [`L233`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_formatter.py#L233) — Format MCP tool response as TOON.
  - `format_structure(self, analysis_result: dict[str, Any])` — [`L259`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_formatter.py#L259) — Format structure analysis output (BaseFormatter requirement).
  - `format_summary(self, analysis_result: dict[str, Any])` — [`L247`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_formatter.py#L247) — Format summary output (BaseFormatter requirement).
  - `format_table(self, analysis_result: dict[str, Any], table_type: str = "full")` — [`L286`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_formatter.py#L286) — Format table output (BaseFormatter requirement).
  - `is_toon_content(content: str)` — [`L318`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_formatter.py#L318) — Detect if content is in TOON format.
  - `compact_arrays` — [`L50`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_formatter.py#L50)
  - `encoder` — [`L54`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_formatter.py#L54)
  - `fallback_to_json` — [`L52`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_formatter.py#L52)
  - `include_metadata` — [`L51`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_formatter.py#L51)
  - `normalize_paths` — [`L53`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_formatter.py#L53)
  - `use_tabs` — [`L49`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_formatter.py#L49)
- uses (calls/refs, reference-scoped): [`AnalysisResult`](../models/result.md#AnalysisResult), [`elements`](../models/result.md#AnalysisResult.elements), [`language`](../models/result.md#AnalysisResult.language), [`ToonEncoder`](toon_encoder.md#ToonEncoder), [`file_path`](../models/result.md#AnalysisResult.file_path), [`encode`](toon_encoder.md#ToonEncoder.encode), [`element_type`](../models/base.md#CodeElement.element_type), [`BaseFormatter`](base_formatter.md#BaseFormatter), [`ToonEncodeError`](toon_encoder.md#ToonEncodeError), [`get_summary`](../models/result.md#AnalysisResult.get_summary), [`encode_array_table`](toon_encoder.md#ToonEncoder.encode_array_table), [`package`](../models/result.md#AnalysisResult.package), [`encode_dict`](toon_encoder.md#ToonEncoder.encode_dict), [`logger`](toon_formatter.md#logger), [`name`](../models/java_models.md#JavaPackage.name), [`encode_to_json`](toon_encoder.md#ToonEncoder.encode_to_json)
- used by: [`BaseFormatter`](base_formatter.md#BaseFormatter), [`_output_statistics`](../cli/commands/advanced_command.md#AdvancedCommand._output_statistics), [`_output_full_analysis`](../cli/commands/advanced_command.md#AdvancedCommand._output_full_analysis), [`format`](base_formatter.md#BaseFormatter.format), [`format_as_toon`](../mcp/utils/format_helper.md#format_as_toon), [`format_structure`](base_formatter.md#BaseFormatter.format_structure), [`format_advanced`](base_formatter.md#BaseFormatter.format_advanced), [`format_summary`](base_formatter.md#BaseFormatter.format_summary), [`format_table`](base_formatter.md#BaseFormatter.format_table), [`_output_structure_analysis`](../cli/commands/structure_command.md#StructureCommand._output_structure_analysis), [`_emit_partial_payload`](../cli/commands/partial_read_command.md#PartialReadCommand._emit_partial_payload), [`_emit_query_results`](../cli/commands/query_command.md#QueryCommand._emit_query_results), [`_emit_summary`](../cli/commands/summary_command.md#SummaryCommand._emit_summary), [`_emit_unsupported_language_envelope`](../cli/commands/base_command.md#BaseCommand._emit_unsupported_language_envelope), [`_format_as_toon`](../cli/commands/table_command.md#TableCommand._format_as_toon), [`_get_formatter_for_toon`](../mcp/utils/format_helper.md#_get_formatter_for_toon), [`_init_formatters`](../output_manager.md#OutputManager._init_formatters)  (61 test-only)

## Module values
- `logger` — [`L16`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_formatter.py#L16)

