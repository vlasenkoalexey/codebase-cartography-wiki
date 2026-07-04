---
title: 'Module: tree_sitter_analyzer/formatters/yaml_formatter.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/formatters/yaml_formatter.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.formatters.yaml_formatter`/
symbols:
  YAMLFormatter: YAMLFormatter#
  YAMLFormatter.format_table: YAMLFormatter#format_table().
  YAMLFormatter.format_advanced: YAMLFormatter#format_advanced().
  YAMLFormatter._format_full: YAMLFormatter#_format_full().
  YAMLFormatter.format_summary: YAMLFormatter#format_summary().
  YAMLFormatter.format_structure: YAMLFormatter#format_structure().
  YAMLFormatter.format_analysis_result: YAMLFormatter#format_analysis_result().
  _yaml_filter: _yaml_filter().
  YAMLFormatter._format_json_output: YAMLFormatter#_format_json_output().
  YAMLFormatter._convert_analysis_result_to_format: YAMLFormatter#_convert_analysis_result_to_format().
  YAMLFormatter.language: YAMLFormatter#language.
  YAMLFormatter._format_compact: YAMLFormatter#_format_compact().
  YAMLFormatter._format_csv: YAMLFormatter#_format_csv().
  YAMLFormatter._calculate_complexity: YAMLFormatter#_calculate_complexity().
  YAMLFormatter._format_advanced_text: YAMLFormatter#_format_advanced_text().
  _strip_yaml_extension: _strip_yaml_extension().
  _yaml_section_overview: _yaml_section_overview().
  _yaml_section_documents: _yaml_section_documents().
  _yaml_section_mappings: _yaml_section_mappings().
  _yaml_section_sequences: _yaml_section_sequences().
  _yaml_section_anchors: _yaml_section_anchors().
  _yaml_section_aliases: _yaml_section_aliases().
  _yaml_section_comments: _yaml_section_comments().
  YAMLFormatter.__init__: YAMLFormatter#__init__().
---
# Module: [`tree_sitter_analyzer/formatters/yaml_formatter.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/yaml_formatter.py)

## Classes
### `YAMLFormatter`  ·  implements/extends BaseFormatter
- def: [`tree_sitter_analyzer/formatters/yaml_formatter.py:14`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/yaml_formatter.py#L14)
- doc: Formatter specialized for YAML documents.
- signature: `class YAMLFormatter(BaseFormatter):`
- members:
  - `__init__(self)` — [`L17`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/yaml_formatter.py#L17) — Initialize the YAML formatter.
  - `_calculate_complexity(self, mappings: list[dict], sequences: list[dict], max_nesting: int)` — [`L342`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/yaml_formatter.py#L342) — Calculate document complexity based on structure.
  - `_convert_analysis_result_to_format(self, analysis_result: Any)` — [`L195`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/yaml_formatter.py#L195) — Convert AnalysisResult to format expected by format_table.
  - `_format_advanced_text(self, data: dict[str, Any])` — [`L361`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/yaml_formatter.py#L361) — Format advanced analysis in text format.
  - `_format_compact(self, analysis_result: dict[str, Any])` — [`L261`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/yaml_formatter.py#L261) — Format compact table output for YAML files.
  - `_format_csv(self, analysis_result: dict[str, Any])` — [`L325`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/yaml_formatter.py#L325) — Format CSV output for YAML files.
  - `_format_full(self, analysis_result: dict[str, Any])` — [`L239`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/yaml_formatter.py#L239) — Format full table output for YAML files.
  - `_format_json_output(self, title: str, data: dict[str, Any])` — [`L387`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/yaml_formatter.py#L387) — Format JSON output with title.
  - `format_advanced(self, analysis_result: dict[str, Any], output_format: str = "json")` — [`L126`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/yaml_formatter.py#L126) — Format advanced analysis for YAML files.
  - `format_analysis_result(self, analysis_result: Any, table_type: str = "full")` — [`L188`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/yaml_formatter.py#L188) — Format AnalysisResult directly for YAML files.
  - `format_structure(self, analysis_result: dict[str, Any])` — [`L47`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/yaml_formatter.py#L47) — Format structure analysis for YAML files.
  - `format_summary(self, analysis_result: dict[str, Any])` — [`L21`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/yaml_formatter.py#L21) — Format summary for YAML files.
  - `format_table(self, analysis_result: dict[str, Any], table_type: str = "full")` — [`L228`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/yaml_formatter.py#L228) — Format table output for YAML files.
  - `language` — [`L19`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/yaml_formatter.py#L19)
- uses (calls/refs, reference-scoped): [`BaseFormatter`](base_formatter.md#BaseFormatter), [`_yaml_filter`](yaml_formatter.md#_yaml_filter), [`_strip_yaml_extension`](yaml_formatter.md#_strip_yaml_extension), [`_yaml_section_aliases`](yaml_formatter.md#_yaml_section_aliases), [`_yaml_section_anchors`](yaml_formatter.md#_yaml_section_anchors), [`_yaml_section_comments`](yaml_formatter.md#_yaml_section_comments), [`_yaml_section_documents`](yaml_formatter.md#_yaml_section_documents), [`_yaml_section_mappings`](yaml_formatter.md#_yaml_section_mappings), [`_yaml_section_overview`](yaml_formatter.md#_yaml_section_overview), [`_yaml_section_sequences`](yaml_formatter.md#_yaml_section_sequences)
- used by: [`BaseFormatter`](base_formatter.md#BaseFormatter), [`_register_language_formatters_safe`](formatter_registry.md#_register_language_formatters_safe), [`_formatters`](language_formatter_factory.md#LanguageFormatterFactory._formatters), [`format_structure`](base_formatter.md#BaseFormatter.format_structure), [`format_advanced`](base_formatter.md#BaseFormatter.format_advanced), [`format_summary`](base_formatter.md#BaseFormatter.format_summary), [`format_table`](base_formatter.md#BaseFormatter.format_table)  (43 test-only)

## Functions
- `_strip_yaml_extension(file_path: str)` — [`L401`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/yaml_formatter.py#L401) — Return the filename without its ``.yaml`` / ``.yml`` extension.
- `_yaml_filter(elements: list[dict[str, Any]], element_type: str)` — [`L409`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/yaml_formatter.py#L409) — Return elements whose ``element_type`` field equals ``element_type``.
- `_yaml_section_aliases(output: list[str], aliases: list[dict[str, Any]])` — [`L496`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/yaml_formatter.py#L496) — Aliases table — ``*target`` + line number.
- `_yaml_section_anchors(output: list[str], anchors: list[dict[str, Any]])` — [`L482`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/yaml_formatter.py#L482) — Anchors table — ``&name`` + line number.
- `_yaml_section_comments(output: list[str], comments: list[dict[str, Any]])` — [`L510`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/yaml_formatter.py#L510) — Comments table — first 50 chars of content + line number.
- `_yaml_section_documents(output: list[str], documents: list[dict[str, Any]])` — [`L433`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/yaml_formatter.py#L433) — Documents table — index + line span + children count.
- `_yaml_section_mappings(output: list[str], mappings: list[dict[str, Any]])` — [`L449`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/yaml_formatter.py#L449) — Mappings table — first 50 key entries, with a ``... (N more)`` tail.
- `_yaml_section_overview(output: list[str], file_path: str, analysis_result: dict[str, Any], element_count: int)` — [`L416`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/yaml_formatter.py#L416) — Document Overview — file path, language, line + element counts.
- `_yaml_section_sequences(output: list[str], sequences: list[dict[str, Any]])` — [`L467`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/yaml_formatter.py#L467) — Sequences table — child count + nesting level.

