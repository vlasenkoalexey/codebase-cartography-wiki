---
title: 'Module: tests/unit/languages/test_rust_properties.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_rust_properties.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_rust_properties`/
symbols:
  TestRustProperties.test_property_8_rust_terminology: TestRustProperties#test_property_8_rust_terminology().
  TestRustProperties.test_property_2_rust_function_extraction_completeness: TestRustProperties#test_property_2_rust_function_extraction_completeness().
  TestRustProperties.test_property_2_rust_struct_extraction_completeness: TestRustProperties#test_property_2_rust_struct_extraction_completeness().
  rust_function_nodes: rust_function_nodes().
  rust_struct_nodes: rust_struct_nodes().
  rust_visibilities: rust_visibilities().
  TestRustProperties.mock_get_text: TestRustProperties#mock_get_text().
  rust_types: rust_types().
  rust_function_nodes.get_child_by_field: rust_function_nodes().get_child_by_field().
  rust_struct_nodes.get_child_by_field: rust_struct_nodes().get_child_by_field().
  TestRustProperties: TestRustProperties#
---
# Module: [`tests/unit/languages/test_rust_properties.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_properties.py)

## Classes
### `TestRustProperties`
- def: [`tests/unit/languages/test_rust_properties.py:167`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_properties.py#L167)
- signature: `class TestRustProperties:`
- members:
  - `mock_get_text(n)` — [`L180`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_properties.py#L180)
  - `test_property_2_rust_function_extraction_completeness(self, data)` — [`L170`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_properties.py#L170) — Property 2: Rust Element Extraction Completeness (Functions)
  - `test_property_2_rust_struct_extraction_completeness(self, data)` — [`L199`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_properties.py#L199) — Property 2: Rust Element Extraction Completeness (Structs)
  - `test_property_8_rust_terminology(self, funcs, structs)` — [`L243`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_properties.py#L243) — Property 8: Rust-Specific Terminology
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`language`](../../../tree_sitter_analyzer/models/base.md#CodeElement.language), [`AnalysisResult`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult), [`Function`](../../../tree_sitter_analyzer/models/base.md#Function), [`Class`](../../../tree_sitter_analyzer/models/base.md#Class), [`elements`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.elements), [`language`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.language), [`file_path`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.file_path), [`line_count`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.line_count), [`return_type`](../../../tree_sitter_analyzer/models/base.md#Function.return_type), [`class_type`](../../../tree_sitter_analyzer/models/base.md#Class.class_type), [`visibility`](../../../tree_sitter_analyzer/models/base.md#Function.visibility), [`RustElementExtractor`](../../../tree_sitter_analyzer/languages/rust_plugin.md#RustElementExtractor), [`_extract_function`](../../../tree_sitter_analyzer/languages/rust_plugin.md#RustElementExtractor._extract_function), [`RustTableFormatter`](../../../tree_sitter_analyzer/formatters/rust_formatter.md#RustTableFormatter), [`to_dict`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.to_dict), [`visibility`](../../../tree_sitter_analyzer/models/base.md#Class.visibility), [`_extract_struct`](../../../tree_sitter_analyzer/languages/rust_plugin.md#RustElementExtractor._extract_struct), [`format_table`](../../../tree_sitter_analyzer/formatters/rust_formatter.md#RustTableFormatter.format_table), [`format_summary`](../../../tree_sitter_analyzer/formatters/rust_formatter.md#RustTableFormatter.format_summary)  (2 test-only)

## Functions
- `get_child_by_field(field)` — [`L96`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_properties.py#L96)
- `get_child_by_field(field)` — [`L151`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_properties.py#L151)
- `rust_function_nodes(draw)` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_properties.py#L37) — Generates a mock tree-sitter node representing a Rust function.
- `rust_struct_nodes(draw)` — [`L119`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_properties.py#L119) — Generates a mock tree-sitter node representing a Rust struct.
- `rust_types(draw)` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_properties.py#L29) — Generates simple Rust types.
- `rust_visibilities(draw)` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_properties.py#L23) — Generates Rust visibility modifiers.

