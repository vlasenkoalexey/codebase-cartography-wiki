---
title: 'Module: tests/unit/languages/test_kotlin_properties.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_kotlin_properties.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_kotlin_properties`/
symbols:
  TestKotlinProperties.test_property_9_kotlin_terminology: TestKotlinProperties#test_property_9_kotlin_terminology().
  TestKotlinProperties.test_property_3_kotlin_class_extraction_completeness: TestKotlinProperties#test_property_3_kotlin_class_extraction_completeness().
  TestKotlinProperties.test_property_3_kotlin_function_extraction_completeness: TestKotlinProperties#test_property_3_kotlin_function_extraction_completeness().
  kotlin_function_nodes: kotlin_function_nodes().
  kotlin_class_nodes: kotlin_class_nodes().
  kotlin_visibilities: kotlin_visibilities().
  TestKotlinProperties.mock_get_text: TestKotlinProperties#mock_get_text().
  kotlin_function_nodes.get_child_by_field: kotlin_function_nodes().get_child_by_field().
  kotlin_class_nodes.get_child_by_field: kotlin_class_nodes().get_child_by_field().
  kotlin_types: kotlin_types().
  TestKotlinProperties: TestKotlinProperties#
---
# Module: [`tests/unit/languages/test_kotlin_properties.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_properties.py)

## Classes
### `TestKotlinProperties`
- def: [`tests/unit/languages/test_kotlin_properties.py:191`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_properties.py#L191)
- signature: `class TestKotlinProperties:`
- members:
  - `mock_get_text(n)` — [`L203`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_properties.py#L203)
  - `test_property_3_kotlin_class_extraction_completeness(self, data)` — [`L221`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_properties.py#L221) — Property 3: Kotlin Element Extraction Completeness (Classes)
  - `test_property_3_kotlin_function_extraction_completeness(self, data)` — [`L194`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_properties.py#L194) — Property 3: Kotlin Element Extraction Completeness (Functions)
  - `test_property_9_kotlin_terminology(self, funcs, classes)` — [`L274`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_properties.py#L274) — Property 9: Kotlin-Specific Terminology
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`language`](../../../tree_sitter_analyzer/models/base.md#CodeElement.language), [`AnalysisResult`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult), [`Function`](../../../tree_sitter_analyzer/models/base.md#Function), [`Class`](../../../tree_sitter_analyzer/models/base.md#Class), [`elements`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.elements), [`language`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.language), [`file_path`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.file_path), [`line_count`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.line_count), [`class_type`](../../../tree_sitter_analyzer/models/base.md#Class.class_type), [`visibility`](../../../tree_sitter_analyzer/models/base.md#Function.visibility), [`KotlinElementExtractor`](../../../tree_sitter_analyzer/languages/kotlin_plugin.md#KotlinElementExtractor), [`KotlinTableFormatter`](../../../tree_sitter_analyzer/formatters/kotlin_formatter.md#KotlinTableFormatter), [`to_dict`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.to_dict), [`visibility`](../../../tree_sitter_analyzer/models/base.md#Class.visibility), [`_extract_class_or_object`](../../../tree_sitter_analyzer/languages/kotlin_plugin.md#KotlinElementExtractor._extract_class_or_object), [`_extract_function`](../../../tree_sitter_analyzer/languages/kotlin_plugin.md#KotlinElementExtractor._extract_function), [`format_table`](../../../tree_sitter_analyzer/formatters/kotlin_formatter.md#KotlinTableFormatter.format_table), [`format_summary`](../../../tree_sitter_analyzer/formatters/kotlin_formatter.md#KotlinTableFormatter.format_summary)  (2 test-only)

## Functions
- `get_child_by_field(field)` — [`L92`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_properties.py#L92)
- `get_child_by_field(field)` — [`L174`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_properties.py#L174)
- `kotlin_class_nodes(draw)` — [`L112`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_properties.py#L112) — Generates a mock tree-sitter node representing a Kotlin class.
- `kotlin_function_nodes(draw)` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_properties.py#L39) — Generates a mock tree-sitter node representing a Kotlin function.
- `kotlin_types(draw)` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_properties.py#L29) — Generates simple Kotlin types.
- `kotlin_visibilities(draw)` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_properties.py#L23) — Generates Kotlin visibility modifiers.

