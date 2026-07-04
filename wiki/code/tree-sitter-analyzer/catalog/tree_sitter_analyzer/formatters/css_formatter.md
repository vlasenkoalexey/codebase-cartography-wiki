---
title: 'Module: tree_sitter_analyzer/formatters/css_formatter.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/formatters/css_formatter.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.formatters.css_formatter`/CSSFormatter#
symbols:
  CSSFormatter.format_structure: format_structure().
  CSSFormatter._format_full: _format_full().
  CSSFormatter.format_advanced: format_advanced().
  CSSFormatter._format_csv: _format_csv().
  CSSFormatter._format_compact: _format_compact().
  CSSFormatter._get_selector: _get_selector().
  CSSFormatter.format_summary: format_summary().
  CSSFormatter: ''
  CSSFormatter.format_table: format_table().
  CSSFormatter._get_properties: _get_properties().
  CSSFormatter._get_name: _get_name().
  CSSFormatter._get_start_line: _get_start_line().
  CSSFormatter.format_analysis_result: format_analysis_result().
  CSSFormatter._is_rule: _is_rule().
  CSSFormatter._is_at_rule: _is_at_rule().
  CSSFormatter._get_end_line: _get_end_line().
  CSSFormatter._calculate_complexity: _calculate_complexity().
  CSSFormatter._format_json_output: _format_json_output().
  CSSFormatter._get_element_class: _get_element_class().
  CSSFormatter._convert_analysis_result_to_format: _convert_analysis_result_to_format().
  CSSFormatter._format_advanced_text: _format_advanced_text().
  CSSFormatter._get_element_type: _get_element_type().
  CSSFormatter.__init__: __init__().
  CSSFormatter.language: language.
---
# Module: [`tree_sitter_analyzer/formatters/css_formatter.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/css_formatter.py)

## Classes
### `CSSFormatter`  ·  implements/extends BaseFormatter
- def: [`tree_sitter_analyzer/formatters/css_formatter.py:14`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/css_formatter.py#L14)
- doc: Formatter specialized for CSS documents.
- signature: `class CSSFormatter(BaseFormatter):`
- members:
  - `__init__(self)` — [`L17`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/css_formatter.py#L17) — Initialize the CSS formatter.
  - `_calculate_complexity(self, rules: list, at_rules: list)` — [`L335`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/css_formatter.py#L335) — Calculate CSS complexity based on structure.
  - `_convert_analysis_result_to_format(self, analysis_result: Any)` — [`L160`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/css_formatter.py#L160) — Convert AnalysisResult to format expected by format_table.
  - `_format_advanced_text(self, data: dict[str, Any])` — [`L354`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/css_formatter.py#L354) — Format advanced analysis in text format.
  - `_format_compact(self, analysis_result: dict[str, Any])` — [`L266`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/css_formatter.py#L266) — Format compact table output for CSS files.
  - `_format_csv(self, analysis_result: dict[str, Any])` — [`L316`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/css_formatter.py#L316) — Format CSV output for CSS files.
  - `_format_full(self, analysis_result: dict[str, Any])` — [`L198`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/css_formatter.py#L198) — Format full table output for CSS files.
  - `_format_json_output(self, title: str, data: dict[str, Any])` — [`L375`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/css_formatter.py#L375) — Format JSON output with title.
  - `_get_element_class(self, element: Any)` — [`L450`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/css_formatter.py#L450) — Extract element class safely
  - `_get_element_type(self, element: Any)` — [`L427`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/css_formatter.py#L427) — Extract element type safely
  - `_get_end_line(self, element: Any)` — [`L465`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/css_formatter.py#L465) — Extract end line safely
  - `_get_name(self, element: Any)` — [`L421`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/css_formatter.py#L421) — Extract name safely
  - `_get_properties(self, element: Any)` — [`L439`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/css_formatter.py#L439) — Extract properties safely
  - `_get_selector(self, element: Any)` — [`L433`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/css_formatter.py#L433) — Extract selector safely
  - `_get_start_line(self, element: Any)` — [`L456`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/css_formatter.py#L456) — Extract start line safely
  - `_is_at_rule(self, element: Any)` — [`L412`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/css_formatter.py#L412) — Check if element is an at-rule.
  - `_is_rule(self, element: Any)` — [`L384`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/css_formatter.py#L384) — Check if element is a CSS rule.
  - `format_advanced(self, analysis_result: dict[str, Any], output_format: str = "json")` — [`L95`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/css_formatter.py#L95) — Format advanced analysis for CSS files.
  - `format_analysis_result(self, analysis_result: Any, table_type: str = "full")` — [`L153`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/css_formatter.py#L153) — Format AnalysisResult directly for CSS files.
  - `format_structure(self, analysis_result: dict[str, Any])` — [`L49`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/css_formatter.py#L49) — Format structure analysis for CSS files.
  - `format_summary(self, analysis_result: dict[str, Any])` — [`L21`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/css_formatter.py#L21) — Format summary for CSS files.
  - `format_table(self, analysis_result: dict[str, Any], table_type: str = "full")` — [`L188`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/css_formatter.py#L188) — Format table output for CSS files.
  - `language` — [`L19`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/css_formatter.py#L19)
- uses (calls/refs, reference-scoped): [`BaseFormatter`](base_formatter.md#BaseFormatter)
- used by: [`BaseFormatter`](base_formatter.md#BaseFormatter), [`_register_language_formatters_safe`](formatter_registry.md#_register_language_formatters_safe), [`_formatters`](language_formatter_factory.md#LanguageFormatterFactory._formatters), [`format_structure`](base_formatter.md#BaseFormatter.format_structure), [`format_advanced`](base_formatter.md#BaseFormatter.format_advanced), [`format_summary`](base_formatter.md#BaseFormatter.format_summary), [`format_table`](base_formatter.md#BaseFormatter.format_table)  (1 test-only)

