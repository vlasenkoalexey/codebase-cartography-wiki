---
title: 'Module: tests/unit/languages/test_go_properties.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_go_properties.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_go_properties`/
symbols:
  TestGoTerminologyProperties.test_property_7_go_visibility_terminology: TestGoTerminologyProperties#test_property_7_go_visibility_terminology().
  TestGoElementExtractionProperties.test_property_1_go_function_extraction_completeness: TestGoElementExtractionProperties#test_property_1_go_function_extraction_completeness().
  TestGoElementExtractionProperties.test_property_1_go_struct_extraction_completeness: TestGoElementExtractionProperties#test_property_1_go_struct_extraction_completeness().
  TestGoElementExtractionProperties.test_property_1_go_interface_extraction_completeness: TestGoElementExtractionProperties#test_property_1_go_interface_extraction_completeness().
  TestGoTerminologyProperties.test_property_7_go_terminology_full_format: TestGoTerminologyProperties#test_property_7_go_terminology_full_format().
  TestGoElementExtractionProperties.test_property_1_go_method_extraction_completeness: TestGoElementExtractionProperties#test_property_1_go_method_extraction_completeness().
  TestGoTerminologyProperties.test_property_7_go_terminology_compact_format: TestGoTerminologyProperties#test_property_7_go_terminology_compact_format().
  TestGoTerminologyProperties.test_property_7_go_interface_terminology: TestGoTerminologyProperties#test_property_7_go_interface_terminology().
  go_function_nodes: go_function_nodes().
  TestGoElementExtractionProperties.mock_get_text: TestGoElementExtractionProperties#mock_get_text().
  go_method_nodes: go_method_nodes().
  go_struct_nodes: go_struct_nodes().
  go_interface_nodes: go_interface_nodes().
  go_types: go_types().
  go_function_nodes.get_child_by_field: go_function_nodes().get_child_by_field().
  go_method_nodes.get_child_by_field: go_method_nodes().get_child_by_field().
  go_struct_nodes.get_child_by_field: go_struct_nodes().get_child_by_field().
  go_interface_nodes.get_child_by_field: go_interface_nodes().get_child_by_field().
  go_visibilities: go_visibilities().
  TestGoElementExtractionProperties: TestGoElementExtractionProperties#
  TestGoTerminologyProperties: TestGoTerminologyProperties#
---
# Module: [`tests/unit/languages/test_go_properties.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_properties.py)

## Classes
### `TestGoElementExtractionProperties`
- def: [`tests/unit/languages/test_go_properties.py:327`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_properties.py#L327)
- doc: Property tests for Go element extraction completeness.
- signature: `class TestGoElementExtractionProperties:`
- members:
  - `mock_get_text(n: MagicMock)` — [`L344`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_properties.py#L344)
  - `test_property_1_go_function_extraction_completeness(self, data: dict)` — [`L332`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_properties.py#L332) — Property 1: Go Element Extraction Completeness (Functions)
  - `test_property_1_go_interface_extraction_completeness(self, data: dict)` — [`L418`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_properties.py#L418) — Property 1: Go Element Extraction Completeness (Interfaces)
  - `test_property_1_go_method_extraction_completeness(self, data: dict)` — [`L360`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_properties.py#L360) — Property 1: Go Element Extraction Completeness (Methods)
  - `test_property_1_go_struct_extraction_completeness(self, data: dict)` — [`L390`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_properties.py#L390) — Property 1: Go Element Extraction Completeness (Structs)
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`language`](../../../tree_sitter_analyzer/models/base.md#CodeElement.language), [`return_type`](../../../tree_sitter_analyzer/models/base.md#Function.return_type), [`class_type`](../../../tree_sitter_analyzer/models/base.md#Class.class_type), [`visibility`](../../../tree_sitter_analyzer/models/base.md#Function.visibility), [`GoElementExtractor`](../../../tree_sitter_analyzer/languages/go_plugin.md#GoElementExtractor), [`visibility`](../../../tree_sitter_analyzer/models/base.md#Class.visibility), [`content_lines`](../../../tree_sitter_analyzer/languages/go_plugin.md#GoElementExtractor.content_lines), [`source_code`](../../../tree_sitter_analyzer/languages/go_plugin.md#GoElementExtractor.source_code), [`_extract_function`](../../../tree_sitter_analyzer/languages/go_plugin.md#GoElementExtractor._extract_function), [`_extract_method`](../../../tree_sitter_analyzer/languages/go_plugin.md#GoElementExtractor._extract_method), [`_extract_type_spec`](../../../tree_sitter_analyzer/languages/go_plugin.md#GoElementExtractor._extract_type_spec)  (4 test-only)

### `TestGoTerminologyProperties`
- def: [`tests/unit/languages/test_go_properties.py:445`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_properties.py#L445)
- doc: Property tests for Go-specific terminology.
- signature: `class TestGoTerminologyProperties:`
- members:
  - `test_property_7_go_interface_terminology(self, interfaces: list[Class])` — [`L552`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_properties.py#L552) — Property 7: Go-Specific Terminology (Interfaces)
  - `test_property_7_go_terminology_compact_format(self, funcs: list[Function])` — [`L513`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_properties.py#L513) — Property 7: Go-Specific Terminology (Compact Format)
  - `test_property_7_go_terminology_full_format(self, funcs: list[Function], structs: list[Class])` — [`L470`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_properties.py#L470) — Property 7: Go-Specific Terminology (Full Format)
  - `test_property_7_go_visibility_terminology(self)` — [`L572`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_properties.py#L572) — Property 7: Go-Specific Terminology (Visibility)
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`AnalysisResult`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult), [`Function`](../../../tree_sitter_analyzer/models/base.md#Function), [`Class`](../../../tree_sitter_analyzer/models/base.md#Class), [`elements`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.elements), [`language`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.language), [`file_path`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.file_path), [`line_count`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.line_count), [`GoTableFormatter`](../../../tree_sitter_analyzer/formatters/go_formatter.md#GoTableFormatter), [`to_dict`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.to_dict), [`format_table`](../../../tree_sitter_analyzer/formatters/go_formatter.md#GoTableFormatter.format_table), [`format_summary`](../../../tree_sitter_analyzer/formatters/go_formatter.md#GoTableFormatter.format_summary)

## Functions
- `get_child_by_field(field: str)` — [`L107`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_properties.py#L107)
- `get_child_by_field(field: str)` — [`L180`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_properties.py#L180)
- `get_child_by_field(field: str)` — [`L248`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_properties.py#L248)
- `get_child_by_field(field: str)` — [`L310`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_properties.py#L310)
- `go_function_nodes(draw: st.DrawFn)` — [`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_properties.py#L51) — Generates a mock tree-sitter node representing a Go function.
- `go_interface_nodes(draw: st.DrawFn)` — [`L266`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_properties.py#L266) — Generates a mock tree-sitter node representing a Go interface.
- `go_method_nodes(draw: st.DrawFn)` — [`L128`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_properties.py#L128) — Generates a mock tree-sitter node representing a Go method.
- `go_struct_nodes(draw: st.DrawFn)` — [`L203`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_properties.py#L203) — Generates a mock tree-sitter node representing a Go struct.
- `go_types(draw: st.DrawFn)` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_properties.py#L30) — Generates simple Go types.
- `go_visibilities(draw: st.DrawFn)` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_properties.py#L23) — Generates Go visibility based on name capitalization.

