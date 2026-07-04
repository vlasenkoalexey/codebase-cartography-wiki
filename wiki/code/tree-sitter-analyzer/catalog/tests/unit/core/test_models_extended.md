---
title: 'Module: tests/unit/core/test_models_extended.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_models_extended.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_models_extended`/Test
symbols:
  TestExtendedModelsIntegration.test_element_serialization_compatibility: ExtendedModelsIntegration#test_element_serialization_compatibility().
  TestExtendedModelsIntegration.test_mixed_elements_in_analysis_result: ExtendedModelsIntegration#test_mixed_elements_in_analysis_result().
  TestExtendedModelsIntegration.test_analysis_result_with_style_elements: ExtendedModelsIntegration#test_analysis_result_with_style_elements().
  TestExtendedModelsIntegration.test_analysis_result_with_markup_elements: ExtendedModelsIntegration#test_analysis_result_with_markup_elements().
  TestMarkupElement.test_markup_element_creation: MarkupElement#test_markup_element_creation().
  TestElementTypeConstants.test_element_summary_items: ElementTypeConstants#test_element_summary_items().
  TestMarkupElement.test_markup_element_default_values: MarkupElement#test_markup_element_default_values().
  TestStyleElement.test_style_element_creation: StyleElement#test_style_element_creation().
  TestExtendedModelsIntegration.test_element_classification_system: ExtendedModelsIntegration#test_element_classification_system().
  TestElementTypeConstants.test_element_type_detection: ElementTypeConstants#test_element_type_detection().
  TestMarkupElement.test_markup_element_hierarchy: MarkupElement#test_markup_element_hierarchy().
  TestMarkupElement.test_markup_element_to_summary_item: MarkupElement#test_markup_element_to_summary_item().
  TestStyleElement.test_style_element_to_summary_item: StyleElement#test_style_element_to_summary_item().
  TestStyleElement.test_style_element_default_values: StyleElement#test_style_element_default_values().
  TestMarkupElement.test_markup_element_complex_attributes: MarkupElement#test_markup_element_complex_attributes().
  TestStyleElement.test_style_element_complex_properties: StyleElement#test_style_element_complex_properties().
  TestEdgeCases.test_markup_element_empty_attributes: EdgeCases#test_markup_element_empty_attributes().
  TestEdgeCases.test_style_element_empty_properties: EdgeCases#test_style_element_empty_properties().
  TestEdgeCases.test_circular_reference_prevention: EdgeCases#test_circular_reference_prevention().
  TestEdgeCases.test_deep_nesting_hierarchy: EdgeCases#test_deep_nesting_hierarchy().
  TestMarkupElement.test_markup_element_inheritance: MarkupElement#test_markup_element_inheritance().
  TestStyleElement.test_style_element_inheritance: StyleElement#test_style_element_inheritance().
  TestMarkupElement: MarkupElement#
  TestStyleElement: StyleElement#
  TestExtendedModelsIntegration: ExtendedModelsIntegration#
  TestElementTypeConstants: ElementTypeConstants#
  TestEdgeCases: EdgeCases#
---
# Module: [`tests/unit/core/test_models_extended.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_extended.py)

## Classes
### `TestEdgeCases`
- def: [`tests/unit/core/test_models_extended.py:528`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_extended.py#L528)
- doc: Test edge cases and error conditions for extended models
- signature: `class TestEdgeCases:`
- members:
  - `test_circular_reference_prevention(self)` — [`L551`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_extended.py#L551) — Test that circular references are handled properly
  - `test_deep_nesting_hierarchy(self)` — [`L568`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_extended.py#L568) — Test deeply nested element hierarchy
  - `test_markup_element_empty_attributes(self)` — [`L531`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_extended.py#L531) — Test MarkupElement with empty attributes
  - `test_style_element_empty_properties(self)` — [`L541`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_extended.py#L541) — Test StyleElement with empty properties
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`MarkupElement`](../../../tree_sitter_analyzer/models/markup_models.md#MarkupElement), [`tag_name`](../../../tree_sitter_analyzer/models/markup_models.md#MarkupElement.tag_name), [`StyleElement`](../../../tree_sitter_analyzer/models/markup_models.md#StyleElement), [`attributes`](../../../tree_sitter_analyzer/models/markup_models.md#MarkupElement.attributes), [`selector`](../../../tree_sitter_analyzer/models/markup_models.md#StyleElement.selector), [`properties`](../../../tree_sitter_analyzer/models/markup_models.md#StyleElement.properties), [`children`](../../../tree_sitter_analyzer/models/markup_models.md#MarkupElement.children), [`parent`](../../../tree_sitter_analyzer/models/markup_models.md#MarkupElement.parent), [`to_summary_item`](../../../tree_sitter_analyzer/models/markup_models.md#MarkupElement.to_summary_item), [`to_summary_item`](../../../tree_sitter_analyzer/models/markup_models.md#StyleElement.to_summary_item)

### `TestElementTypeConstants`
- def: [`tests/unit/core/test_models_extended.py:474`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_extended.py#L474)
- doc: Test element type constants and utilities
- signature: `class TestElementTypeConstants:`
- members:
  - `test_element_summary_items(self)` — [`L490`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_extended.py#L490) — Test summary item generation for new elements
  - `test_element_type_detection(self)` — [`L477`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_extended.py#L477) — Test element type detection for new models
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`MarkupElement`](../../../tree_sitter_analyzer/models/markup_models.md#MarkupElement), [`tag_name`](../../../tree_sitter_analyzer/models/markup_models.md#MarkupElement.tag_name), [`StyleElement`](../../../tree_sitter_analyzer/models/markup_models.md#StyleElement), [`element_class`](../../../tree_sitter_analyzer/models/markup_models.md#MarkupElement.element_class), [`selector`](../../../tree_sitter_analyzer/models/markup_models.md#StyleElement.selector), [`element_class`](../../../tree_sitter_analyzer/models/markup_models.md#StyleElement.element_class), [`to_summary_item`](../../../tree_sitter_analyzer/models/markup_models.md#MarkupElement.to_summary_item), [`to_summary_item`](../../../tree_sitter_analyzer/models/markup_models.md#StyleElement.to_summary_item), [`element_type`](../../../tree_sitter_analyzer/models/markup_models.md#StyleElement.element_type), [`element_type`](../../../tree_sitter_analyzer/models/markup_models.md#MarkupElement.element_type)

### `TestExtendedModelsIntegration`
- def: [`tests/unit/core/test_models_extended.py:225`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_extended.py#L225)
- doc: Test integration of extended models with existing system
- signature: `class TestExtendedModelsIntegration:`
- members:
  - `test_analysis_result_with_markup_elements(self)` — [`L228`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_extended.py#L228) — Test AnalysisResult with MarkupElement objects
  - `test_analysis_result_with_style_elements(self)` — [`L262`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_extended.py#L262) — Test AnalysisResult with StyleElement objects
  - `test_element_classification_system(self)` — [`L345`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_extended.py#L345) — Test element classification system for HTML/CSS
  - `test_element_serialization_compatibility(self)` — [`L426`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_extended.py#L426) — Test that new elements work with existing serialization methods
  - `test_mixed_elements_in_analysis_result(self)` — [`L298`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_extended.py#L298) — Test AnalysisResult with mixed element types
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`language`](../../../tree_sitter_analyzer/models/base.md#CodeElement.language), [`AnalysisResult`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult), [`Function`](../../../tree_sitter_analyzer/models/base.md#Function), [`Variable`](../../../tree_sitter_analyzer/models/base.md#Variable), [`elements`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.elements), [`language`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.language), [`file_path`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.file_path), [`success`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.success), [`MarkupElement`](../../../tree_sitter_analyzer/models/markup_models.md#MarkupElement), [`line_count`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.line_count), [`tag_name`](../../../tree_sitter_analyzer/models/markup_models.md#MarkupElement.tag_name), [`StyleElement`](../../../tree_sitter_analyzer/models/markup_models.md#StyleElement), [`element_class`](../../../tree_sitter_analyzer/models/markup_models.md#MarkupElement.element_class), [`attributes`](../../../tree_sitter_analyzer/models/markup_models.md#MarkupElement.attributes), [`source_code`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.source_code), [`node_count`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.node_count), [`selector`](../../../tree_sitter_analyzer/models/markup_models.md#StyleElement.selector), [`element_class`](../../../tree_sitter_analyzer/models/markup_models.md#StyleElement.element_class), [`properties`](../../../tree_sitter_analyzer/models/markup_models.md#StyleElement.properties), [`to_dict`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.to_dict), [`to_mcp_format`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.to_mcp_format), [`query_results`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.query_results), [`to_summary_dict`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.to_summary_dict), [`to_json`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.to_json)

### `TestMarkupElement`
- def: [`tests/unit/core/test_models_extended.py:17`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_extended.py#L17)
- doc: Test MarkupElement data model
- signature: `class TestMarkupElement:`
- members:
  - `test_markup_element_complex_attributes(self)` — [`L118`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_extended.py#L118) — Test MarkupElement with complex attributes
  - `test_markup_element_creation(self)` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_extended.py#L20) — Test basic MarkupElement creation
  - `test_markup_element_default_values(self)` — [`L107`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_extended.py#L107) — Test MarkupElement with default values
  - `test_markup_element_hierarchy(self)` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_extended.py#L48) — Test parent-child relationships
  - `test_markup_element_inheritance(self)` — [`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_extended.py#L41) — Test MarkupElement inherits from CodeElement
  - `test_markup_element_to_summary_item(self)` — [`L84`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_extended.py#L84) — Test to_summary_item method
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`language`](../../../tree_sitter_analyzer/models/base.md#CodeElement.language), [`raw_text`](../../../tree_sitter_analyzer/models/base.md#CodeElement.raw_text), [`CodeElement`](../../../tree_sitter_analyzer/models/base.md#CodeElement), [`MarkupElement`](../../../tree_sitter_analyzer/models/markup_models.md#MarkupElement), [`tag_name`](../../../tree_sitter_analyzer/models/markup_models.md#MarkupElement.tag_name), [`element_class`](../../../tree_sitter_analyzer/models/markup_models.md#MarkupElement.element_class), [`attributes`](../../../tree_sitter_analyzer/models/markup_models.md#MarkupElement.attributes), [`children`](../../../tree_sitter_analyzer/models/markup_models.md#MarkupElement.children), [`parent`](../../../tree_sitter_analyzer/models/markup_models.md#MarkupElement.parent), [`to_summary_item`](../../../tree_sitter_analyzer/models/markup_models.md#MarkupElement.to_summary_item), [`element_type`](../../../tree_sitter_analyzer/models/markup_models.md#MarkupElement.element_type)

### `TestStyleElement`
- def: [`tests/unit/core/test_models_extended.py:140`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_extended.py#L140)
- doc: Test StyleElement data model
- signature: `class TestStyleElement:`
- members:
  - `test_style_element_complex_properties(self)` — [`L201`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_extended.py#L201) — Test StyleElement with complex CSS properties
  - `test_style_element_creation(self)` — [`L143`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_extended.py#L143) — Test basic StyleElement creation
  - `test_style_element_default_values(self)` — [`L192`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_extended.py#L192) — Test StyleElement with default values
  - `test_style_element_inheritance(self)` — [`L162`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_extended.py#L162) — Test StyleElement inherits from CodeElement
  - `test_style_element_to_summary_item(self)` — [`L169`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_extended.py#L169) — Test to_summary_item method
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`language`](../../../tree_sitter_analyzer/models/base.md#CodeElement.language), [`raw_text`](../../../tree_sitter_analyzer/models/base.md#CodeElement.raw_text), [`CodeElement`](../../../tree_sitter_analyzer/models/base.md#CodeElement), [`StyleElement`](../../../tree_sitter_analyzer/models/markup_models.md#StyleElement), [`selector`](../../../tree_sitter_analyzer/models/markup_models.md#StyleElement.selector), [`element_class`](../../../tree_sitter_analyzer/models/markup_models.md#StyleElement.element_class), [`properties`](../../../tree_sitter_analyzer/models/markup_models.md#StyleElement.properties), [`to_summary_item`](../../../tree_sitter_analyzer/models/markup_models.md#StyleElement.to_summary_item), [`element_type`](../../../tree_sitter_analyzer/models/markup_models.md#StyleElement.element_type)

