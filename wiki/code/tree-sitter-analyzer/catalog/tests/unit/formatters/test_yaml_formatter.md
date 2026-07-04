---
title: 'Module: tests/unit/formatters/test_yaml_formatter.py'
type: catalog
provenance: extracted
module: tests/unit/formatters/test_yaml_formatter.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.formatters.test_yaml_formatter`/
symbols:
  TestYAMLFormatterInit.test_yaml_formatter_init: TestYAMLFormatterInit#test_yaml_formatter_init().
  TestYAMLFormatterFormatSummary.test_format_summary_empty_elements: TestYAMLFormatterFormatSummary#test_format_summary_empty_elements().
  TestYAMLFormatterFormatSummary.test_format_summary_with_documents: TestYAMLFormatterFormatSummary#test_format_summary_with_documents().
  TestYAMLFormatterFormatSummary.test_format_summary_with_mappings: TestYAMLFormatterFormatSummary#test_format_summary_with_mappings().
  TestYAMLFormatterFormatSummary.test_format_summary_with_sequences: TestYAMLFormatterFormatSummary#test_format_summary_with_sequences().
  TestYAMLFormatterFormatSummary.test_format_summary_with_anchors: TestYAMLFormatterFormatSummary#test_format_summary_with_anchors().
  TestYAMLFormatterFormatSummary.test_format_summary_with_aliases: TestYAMLFormatterFormatSummary#test_format_summary_with_aliases().
  TestYAMLFormatterFormatStructure.test_format_structure_empty: TestYAMLFormatterFormatStructure#test_format_structure_empty().
  TestYAMLFormatterFormatStructure.test_format_structure_with_documents: TestYAMLFormatterFormatStructure#test_format_structure_with_documents().
  TestYAMLFormatterFormatStructure.test_format_structure_with_mappings: TestYAMLFormatterFormatStructure#test_format_structure_with_mappings().
  TestYAMLFormatterFormatStructure.test_format_structure_with_sequences: TestYAMLFormatterFormatStructure#test_format_structure_with_sequences().
  TestYAMLFormatterFormatAdvanced.test_format_basic: TestYAMLFormatterFormatAdvanced#test_format_basic().
  TestYAMLFormatterFormatAdvanced.test_format_with_nesting: TestYAMLFormatterFormatAdvanced#test_format_with_nesting().
  TestYAMLFormatterFormatAdvanced.test_format_text_output: TestYAMLFormatterFormatAdvanced#test_format_text_output().
  TestYAMLFormatterFormatAdvanced.test_format_json_output: TestYAMLFormatterFormatAdvanced#test_format_json_output().
  TestYAMLFormatterFormatTable.test_format_table_full: TestYAMLFormatterFormatTable#test_format_table_full().
  TestYAMLFormatterFormatTable.test_format_table_compact: TestYAMLFormatterFormatTable#test_format_table_compact().
  TestYAMLFormatterFormatTable.test_format_table_csv: TestYAMLFormatterFormatTable#test_format_table_csv().
  TestYAMLFormatterEdgeCases.test_format_empty_result: TestYAMLFormatterEdgeCases#test_format_empty_result().
  TestYAMLFormatterEdgeCases.test_format_with_special_characters: TestYAMLFormatterEdgeCases#test_format_with_special_characters().
  TestYAMLFormatterEdgeCases.test_format_with_long_content: TestYAMLFormatterEdgeCases#test_format_with_long_content().
  TestYAMLFormatterFullTable.test_full_table_with_documents: TestYAMLFormatterFullTable#test_full_table_with_documents().
  TestYAMLFormatterFullTable.test_full_table_with_sequences: TestYAMLFormatterFullTable#test_full_table_with_sequences().
  TestYAMLFormatterFullTable.test_full_table_with_anchors: TestYAMLFormatterFullTable#test_full_table_with_anchors().
  TestYAMLFormatterFullTable.test_full_table_with_aliases: TestYAMLFormatterFullTable#test_full_table_with_aliases().
  TestYAMLFormatterFullTable.test_full_table_many_mappings_truncation: TestYAMLFormatterFullTable#test_full_table_many_mappings_truncation().
  TestYAMLFormatterCompact.test_compact_top_level_mappings: TestYAMLFormatterCompact#test_compact_top_level_mappings().
  TestYAMLFormatterCompact.test_compact_with_anchors_and_aliases: TestYAMLFormatterCompact#test_compact_with_anchors_and_aliases().
  TestYAMLFormatterComplexity.test_complexity_simple: TestYAMLFormatterComplexity#test_complexity_simple().
  TestYAMLFormatterComplexity.test_complexity_moderate: TestYAMLFormatterComplexity#test_complexity_moderate().
  TestYAMLFormatterComplexity.test_complexity_complex: TestYAMLFormatterComplexity#test_complexity_complex().
  TestYAMLFormatterComplexity.test_complexity_very_complex: TestYAMLFormatterComplexity#test_complexity_very_complex().
  TestYAMLFormatterFormatAnalysisResult.test_format_analysis_result: TestYAMLFormatterFormatAnalysisResult#test_format_analysis_result().
  TestYAMLFormatterValueTypes.test_advanced_value_type_distribution: TestYAMLFormatterValueTypes#test_advanced_value_type_distribution().
  TestYAMLFormatterValueTypes.test_advanced_multi_document: TestYAMLFormatterValueTypes#test_advanced_multi_document().
  TestYAMLFormatterValueTypes.test_advanced_content_analysis_flags: TestYAMLFormatterValueTypes#test_advanced_content_analysis_flags().
  yaml_formatter: yaml_formatter().
  TestYAMLFormatterInit: TestYAMLFormatterInit#
  TestYAMLFormatterFormatSummary: TestYAMLFormatterFormatSummary#
  TestYAMLFormatterFormatStructure: TestYAMLFormatterFormatStructure#
  TestYAMLFormatterFormatAdvanced: TestYAMLFormatterFormatAdvanced#
  TestYAMLFormatterFormatTable: TestYAMLFormatterFormatTable#
  TestYAMLFormatterEdgeCases: TestYAMLFormatterEdgeCases#
  TestYAMLFormatterFullTable: TestYAMLFormatterFullTable#
  TestYAMLFormatterCompact: TestYAMLFormatterCompact#
  TestYAMLFormatterComplexity: TestYAMLFormatterComplexity#
  TestYAMLFormatterFormatAnalysisResult: TestYAMLFormatterFormatAnalysisResult#
  TestYAMLFormatterValueTypes: TestYAMLFormatterValueTypes#
---
# Module: [`tests/unit/formatters/test_yaml_formatter.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_yaml_formatter.py)

## Classes
### `TestYAMLFormatterCompact`
- def: [`tests/unit/formatters/test_yaml_formatter.py:465`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_yaml_formatter.py#L465)
- doc: Tests for _format_compact covering top-level keys and references.
- signature: `class TestYAMLFormatterCompact:`
- members:
  - `test_compact_top_level_mappings(self, yaml_formatter: YAMLFormatter)` — [`L468`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_yaml_formatter.py#L468)
  - `test_compact_with_anchors_and_aliases(self, yaml_formatter: YAMLFormatter)` — [`L493`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_yaml_formatter.py#L493)
- uses (calls/refs, reference-scoped): [`YAMLFormatter`](../../../tree_sitter_analyzer/formatters/yaml_formatter.md#YAMLFormatter), [`format_table`](../../../tree_sitter_analyzer/formatters/yaml_formatter.md#YAMLFormatter.format_table)

### `TestYAMLFormatterComplexity`
- def: [`tests/unit/formatters/test_yaml_formatter.py:518`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_yaml_formatter.py#L518)
- doc: Tests for _calculate_complexity covering all branches.
- signature: `class TestYAMLFormatterComplexity:`
- members:
  - `test_complexity_complex(self, yaml_formatter: YAMLFormatter)` — [`L553`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_yaml_formatter.py#L553)
  - `test_complexity_moderate(self, yaml_formatter: YAMLFormatter)` — [`L538`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_yaml_formatter.py#L538)
  - `test_complexity_simple(self, yaml_formatter: YAMLFormatter)` — [`L521`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_yaml_formatter.py#L521)
  - `test_complexity_very_complex(self, yaml_formatter: YAMLFormatter)` — [`L568`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_yaml_formatter.py#L568)
- uses (calls/refs, reference-scoped): [`YAMLFormatter`](../../../tree_sitter_analyzer/formatters/yaml_formatter.md#YAMLFormatter), [`format_advanced`](../../../tree_sitter_analyzer/formatters/yaml_formatter.md#YAMLFormatter.format_advanced)

### `TestYAMLFormatterEdgeCases`
- def: [`tests/unit/formatters/test_yaml_formatter.py:326`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_yaml_formatter.py#L326)
- doc: Tests for edge cases.
- signature: `class TestYAMLFormatterEdgeCases:`
- members:
  - `test_format_empty_result(self, yaml_formatter: YAMLFormatter)` — [`L329`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_yaml_formatter.py#L329) — Test formatting empty result.
  - `test_format_with_long_content(self, yaml_formatter: YAMLFormatter)` — [`L356`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_yaml_formatter.py#L356) — Test formatting with long content.
  - `test_format_with_special_characters(self, yaml_formatter: YAMLFormatter)` — [`L335`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_yaml_formatter.py#L335) — Test formatting with special characters in keys.
- uses (calls/refs, reference-scoped): [`YAMLFormatter`](../../../tree_sitter_analyzer/formatters/yaml_formatter.md#YAMLFormatter), [`format_table`](../../../tree_sitter_analyzer/formatters/yaml_formatter.md#YAMLFormatter.format_table)

### `TestYAMLFormatterFormatAdvanced`
- def: [`tests/unit/formatters/test_yaml_formatter.py:200`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_yaml_formatter.py#L200)
- doc: Tests for YAMLFormatter.format_advanced method.
- signature: `class TestYAMLFormatterFormatAdvanced:`
- members:
  - `test_format_basic(self, yaml_formatter: YAMLFormatter)` — [`L203`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_yaml_formatter.py#L203) — Test basic advanced formatting.
  - `test_format_json_output(self, yaml_formatter: YAMLFormatter)` — [`L251`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_yaml_formatter.py#L251) — Test JSON output format.
  - `test_format_text_output(self, yaml_formatter: YAMLFormatter)` — [`L241`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_yaml_formatter.py#L241) — Test text output format.
  - `test_format_with_nesting(self, yaml_formatter: YAMLFormatter)` — [`L222`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_yaml_formatter.py#L222) — Test formatting with nested mappings.
- uses (calls/refs, reference-scoped): [`YAMLFormatter`](../../../tree_sitter_analyzer/formatters/yaml_formatter.md#YAMLFormatter), [`format_advanced`](../../../tree_sitter_analyzer/formatters/yaml_formatter.md#YAMLFormatter.format_advanced)

### `TestYAMLFormatterFormatAnalysisResult`
- def: [`tests/unit/formatters/test_yaml_formatter.py:584`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_yaml_formatter.py#L584)
- doc: Tests for format_analysis_result / _convert_analysis_result_to_format.
- signature: `class TestYAMLFormatterFormatAnalysisResult:`
- members:
  - `test_format_analysis_result(self, yaml_formatter: YAMLFormatter)` — [`L587`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_yaml_formatter.py#L587)
- uses (calls/refs, reference-scoped): [`YAMLFormatter`](../../../tree_sitter_analyzer/formatters/yaml_formatter.md#YAMLFormatter), [`format_analysis_result`](../../../tree_sitter_analyzer/formatters/yaml_formatter.md#YAMLFormatter.format_analysis_result)

### `TestYAMLFormatterFormatStructure`
- def: [`tests/unit/formatters/test_yaml_formatter.py:123`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_yaml_formatter.py#L123)
- doc: Tests for YAMLFormatter.format_structure method.
- signature: `class TestYAMLFormatterFormatStructure:`
- members:
  - `test_format_structure_empty(self, yaml_formatter: YAMLFormatter)` — [`L126`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_yaml_formatter.py#L126) — Test formatting structure with empty elements.
  - `test_format_structure_with_documents(self, yaml_formatter: YAMLFormatter)` — [`L138`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_yaml_formatter.py#L138) — Test formatting structure with documents.
  - `test_format_structure_with_mappings(self, yaml_formatter: YAMLFormatter)` — [`L158`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_yaml_formatter.py#L158) — Test formatting structure with mappings.
  - `test_format_structure_with_sequences(self, yaml_formatter: YAMLFormatter)` — [`L179`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_yaml_formatter.py#L179) — Test formatting structure with sequences.
- uses (calls/refs, reference-scoped): [`YAMLFormatter`](../../../tree_sitter_analyzer/formatters/yaml_formatter.md#YAMLFormatter), [`format_structure`](../../../tree_sitter_analyzer/formatters/yaml_formatter.md#YAMLFormatter.format_structure)

### `TestYAMLFormatterFormatSummary`
- def: [`tests/unit/formatters/test_yaml_formatter.py:22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_yaml_formatter.py#L22)
- doc: Tests for YAMLFormatter.format_summary method.
- signature: `class TestYAMLFormatterFormatSummary:`
- members:
  - `test_format_summary_empty_elements(self, yaml_formatter: YAMLFormatter)` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_yaml_formatter.py#L25) — Test formatting summary with empty elements.
  - `test_format_summary_with_aliases(self, yaml_formatter: YAMLFormatter)` — [`L105`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_yaml_formatter.py#L105) — Test formatting summary with aliases.
  - `test_format_summary_with_anchors(self, yaml_formatter: YAMLFormatter)` — [`L88`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_yaml_formatter.py#L88) — Test formatting summary with anchors.
  - `test_format_summary_with_documents(self, yaml_formatter: YAMLFormatter)` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_yaml_formatter.py#L37) — Test formatting summary with documents.
  - `test_format_summary_with_mappings(self, yaml_formatter: YAMLFormatter)` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_yaml_formatter.py#L53) — Test formatting summary with mappings.
  - `test_format_summary_with_sequences(self, yaml_formatter: YAMLFormatter)` — [`L71`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_yaml_formatter.py#L71) — Test formatting summary with sequences.
- uses (calls/refs, reference-scoped): [`YAMLFormatter`](../../../tree_sitter_analyzer/formatters/yaml_formatter.md#YAMLFormatter), [`format_summary`](../../../tree_sitter_analyzer/formatters/yaml_formatter.md#YAMLFormatter.format_summary)

### `TestYAMLFormatterFormatTable`
- def: [`tests/unit/formatters/test_yaml_formatter.py:262`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_yaml_formatter.py#L262)
- doc: Tests for YAMLFormatter.format_table method.
- signature: `class TestYAMLFormatterFormatTable:`
- members:
  - `test_format_table_compact(self, yaml_formatter: YAMLFormatter)` — [`L285`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_yaml_formatter.py#L285) — Test formatting compact table.
  - `test_format_table_csv(self, yaml_formatter: YAMLFormatter)` — [`L305`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_yaml_formatter.py#L305) — Test formatting CSV table.
  - `test_format_table_full(self, yaml_formatter: YAMLFormatter)` — [`L265`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_yaml_formatter.py#L265) — Test formatting full table.
- uses (calls/refs, reference-scoped): [`YAMLFormatter`](../../../tree_sitter_analyzer/formatters/yaml_formatter.md#YAMLFormatter), [`format_table`](../../../tree_sitter_analyzer/formatters/yaml_formatter.md#YAMLFormatter.format_table)

### `TestYAMLFormatterFullTable`
- def: [`tests/unit/formatters/test_yaml_formatter.py:374`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_yaml_formatter.py#L374)
- doc: Tests for _format_full covering all element sections.
- signature: `class TestYAMLFormatterFullTable:`
- members:
  - `test_full_table_many_mappings_truncation(self, yaml_formatter: YAMLFormatter)` — [`L443`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_yaml_formatter.py#L443)
  - `test_full_table_with_aliases(self, yaml_formatter: YAMLFormatter)` — [`L427`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_yaml_formatter.py#L427)
  - `test_full_table_with_anchors(self, yaml_formatter: YAMLFormatter)` — [`L411`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_yaml_formatter.py#L411)
  - `test_full_table_with_documents(self, yaml_formatter: YAMLFormatter)` — [`L377`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_yaml_formatter.py#L377)
  - `test_full_table_with_sequences(self, yaml_formatter: YAMLFormatter)` — [`L395`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_yaml_formatter.py#L395)
- uses (calls/refs, reference-scoped): [`YAMLFormatter`](../../../tree_sitter_analyzer/formatters/yaml_formatter.md#YAMLFormatter), [`format_table`](../../../tree_sitter_analyzer/formatters/yaml_formatter.md#YAMLFormatter.format_table)

### `TestYAMLFormatterInit`
- def: [`tests/unit/formatters/test_yaml_formatter.py:13`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_yaml_formatter.py#L13)
- doc: Tests for YAMLFormatter initialization.
- signature: `class TestYAMLFormatterInit:`
- members:
  - `test_yaml_formatter_init(self)` — [`L16`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_yaml_formatter.py#L16) — Test YAMLFormatter initialization.
- uses (calls/refs, reference-scoped): [`YAMLFormatter`](../../../tree_sitter_analyzer/formatters/yaml_formatter.md#YAMLFormatter), [`language`](../../../tree_sitter_analyzer/formatters/yaml_formatter.md#YAMLFormatter.language)

### `TestYAMLFormatterValueTypes`
- def: [`tests/unit/formatters/test_yaml_formatter.py:615`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_yaml_formatter.py#L615)
- doc: Test advanced formatting with various value types.
- signature: `class TestYAMLFormatterValueTypes:`
- members:
  - `test_advanced_content_analysis_flags(self, yaml_formatter: YAMLFormatter)` — [`L676`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_yaml_formatter.py#L676)
  - `test_advanced_multi_document(self, yaml_formatter: YAMLFormatter)` — [`L652`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_yaml_formatter.py#L652)
  - `test_advanced_value_type_distribution(self, yaml_formatter: YAMLFormatter)` — [`L618`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_yaml_formatter.py#L618)
- uses (calls/refs, reference-scoped): [`YAMLFormatter`](../../../tree_sitter_analyzer/formatters/yaml_formatter.md#YAMLFormatter), [`format_advanced`](../../../tree_sitter_analyzer/formatters/yaml_formatter.md#YAMLFormatter.format_advanced)

## Functions
- `yaml_formatter()` — [`L696`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_yaml_formatter.py#L696) — Create a YAMLFormatter instance for testing.

