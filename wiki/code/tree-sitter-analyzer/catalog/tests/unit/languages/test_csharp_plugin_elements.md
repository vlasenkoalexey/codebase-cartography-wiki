---
title: 'Module: tests/unit/languages/test_csharp_plugin_elements.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_csharp_plugin_elements.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_csharp_plugin_elements`/
symbols:
  get_tree_for_code: get_tree_for_code().
  SIMPLE_CLASS_CODE: SIMPLE_CLASS_CODE.
  COMPLEX_CLASS_CODE: COMPLEX_CLASS_CODE.
  TestCSharpClassExtraction.test_extract_simple_class: TestCSharpClassExtraction#test_extract_simple_class().
  TestCSharpVariableExtraction.test_extract_const_field: TestCSharpVariableExtraction#test_extract_const_field().
  TestCSharpVariableExtraction.test_extract_readonly_field: TestCSharpVariableExtraction#test_extract_readonly_field().
  TestCSharpVariableExtraction.test_extract_field_type: TestCSharpVariableExtraction#test_extract_field_type().
  TestCSharpClassExtraction.test_extract_interface: TestCSharpClassExtraction#test_extract_interface().
  TestCSharpClassExtraction.test_class_attribute_names_extracted: TestCSharpClassExtraction#test_class_attribute_names_extracted().
  TestCSharpClassExtraction.test_extract_abstract_class: TestCSharpClassExtraction#test_extract_abstract_class().
  TestCSharpClassExtraction.test_extract_class_with_generics: TestCSharpClassExtraction#test_extract_class_with_generics().
  TestCSharpClassExtraction.test_class_constructor_extraction: TestCSharpClassExtraction#test_class_constructor_extraction().
  TestCSharpFunctionExtraction.test_extract_method_parameters: TestCSharpFunctionExtraction#test_extract_method_parameters().
  TestCSharpFunctionExtraction.test_extract_method_with_parameters: TestCSharpFunctionExtraction#test_extract_method_with_parameters().
  TestCSharpFunctionExtraction.test_extract_constructor: TestCSharpFunctionExtraction#test_extract_constructor().
  TestCSharpFunctionExtraction.test_extract_method_modifiers: TestCSharpFunctionExtraction#test_extract_method_modifiers().
  TestCSharpFunctionExtraction.test_extract_virtual_method: TestCSharpFunctionExtraction#test_extract_virtual_method().
  TestCSharpFunctionExtraction.test_method_complexity_calculation: TestCSharpFunctionExtraction#test_method_complexity_calculation().
  TestCSharpVariableExtraction.test_extract_event_field: TestCSharpVariableExtraction#test_extract_event_field().
  TestCSharpVariableExtraction.test_extract_static_field: TestCSharpVariableExtraction#test_extract_static_field().
  TestCSharpImportExtraction.test_extract_static_using: TestCSharpImportExtraction#test_extract_static_using().
  TestCSharpImportExtraction.test_import_line_numbers: TestCSharpImportExtraction#test_import_line_numbers().
  TestCSharpComplexityCalculation.test_complexity_with_control_flow: TestCSharpComplexityCalculation#test_complexity_with_control_flow().
  TestCSharpComplexityCalculation.test_simple_method_low_complexity: TestCSharpComplexityCalculation#test_simple_method_low_complexity().
  TestCSharpClassExtraction.test_extract_multiple_classes: TestCSharpClassExtraction#test_extract_multiple_classes().
  TestCSharpClassExtraction.test_extract_class_with_attributes: TestCSharpClassExtraction#test_extract_class_with_attributes().
  TestCSharpClassExtraction.test_method_attribute_names_extracted: TestCSharpClassExtraction#test_method_attribute_names_extracted().
  TestCSharpClassExtraction.test_class_methods_extraction: TestCSharpClassExtraction#test_class_methods_extraction().
  TestCSharpFunctionExtraction.test_extract_simple_method: TestCSharpFunctionExtraction#test_extract_simple_method().
  TestCSharpFunctionExtraction.test_extract_async_methods: TestCSharpFunctionExtraction#test_extract_async_methods().
  TestCSharpFunctionExtraction.test_methods_carry_parent_class: TestCSharpFunctionExtraction#test_methods_carry_parent_class().
  TestCSharpVariableExtraction.test_extract_private_field: TestCSharpVariableExtraction#test_extract_private_field().
  TestCSharpImportExtraction.test_extract_simple_using: TestCSharpImportExtraction#test_extract_simple_using().
  TestCSharpPropertyExtraction.test_extract_auto_property: TestCSharpPropertyExtraction#test_extract_auto_property().
  TestCSharpPropertyExtraction.test_extract_various_properties: TestCSharpPropertyExtraction#test_extract_various_properties().
  TestCSharpNamespaceHandling.test_extract_namespace: TestCSharpNamespaceHandling#test_extract_namespace().
  TestCSharpNamespaceHandling.test_nested_namespace: TestCSharpNamespaceHandling#test_nested_namespace().
  TestCSharpExtractorHelpers.test_cache_invalidation: TestCSharpExtractorHelpers#test_cache_invalidation().
  TestCSharpClassExtraction.test_extract_with_none_source: TestCSharpClassExtraction#test_extract_with_none_source().
  TestCSharpExtractorHelpers.test_traverse_iterative: TestCSharpExtractorHelpers#test_traverse_iterative().
  TestCSharpExtractorHelpers.test_get_node_text_optimized: TestCSharpExtractorHelpers#test_get_node_text_optimized().
  TestCSharpClassExtraction.test_extract_empty_tree: TestCSharpClassExtraction#test_extract_empty_tree().
  TestCSharpFunctionExtraction.test_extract_functions_empty_tree: TestCSharpFunctionExtraction#test_extract_functions_empty_tree().
  TestCSharpVariableExtraction.test_extract_variables_empty_tree: TestCSharpVariableExtraction#test_extract_variables_empty_tree().
  TestCSharpImportExtraction.test_extract_imports_empty_tree: TestCSharpImportExtraction#test_extract_imports_empty_tree().
  INTERFACE_CODE: INTERFACE_CODE.
  CONTROL_FLOW_CODE: CONTROL_FLOW_CODE.
  ASYNC_METHOD_CODE: ASYNC_METHOD_CODE.
  PROPERTY_VARIATIONS_CODE: PROPERTY_VARIATIONS_CODE.
  TestCSharpClassExtraction: TestCSharpClassExtraction#
  TestCSharpFunctionExtraction: TestCSharpFunctionExtraction#
  TestCSharpVariableExtraction: TestCSharpVariableExtraction#
  TestCSharpImportExtraction: TestCSharpImportExtraction#
  TestCSharpPropertyExtraction: TestCSharpPropertyExtraction#
  TestCSharpComplexityCalculation: TestCSharpComplexityCalculation#
  TestCSharpNamespaceHandling: TestCSharpNamespaceHandling#
  TestCSharpExtractorHelpers: TestCSharpExtractorHelpers#
---
# Module: [`tests/unit/languages/test_csharp_plugin_elements.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_elements.py)

## Classes
### `TestCSharpClassExtraction`
- def: [`tests/unit/languages/test_csharp_plugin_elements.py:263`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_elements.py#L263)
- doc: Test C# class extraction.
- signature: `class TestCSharpClassExtraction:`
- members:
  - `test_class_attribute_names_extracted(self)` — [`L310`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_elements.py#L310) — [TDD] Class attribute names must be populated — not empty list.
  - `test_class_constructor_extraction(self)` — [`L395`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_elements.py#L395) — Test that constructors are extracted.
  - `test_class_methods_extraction(self)` — [`L384`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_elements.py#L384) — Test that class methods are extracted as part of class.
  - `test_extract_abstract_class(self)` — [`L363`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_elements.py#L363) — Test extraction of abstract class.
  - `test_extract_class_with_attributes(self)` — [`L300`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_elements.py#L300) — Test extraction of class with attributes.
  - `test_extract_class_with_generics(self)` — [`L373`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_elements.py#L373) — Test extraction of generic class.
  - `test_extract_empty_tree(self)` — [`L412`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_elements.py#L412) — Test extraction with empty/None tree.
  - `test_extract_interface(self)` — [`L278`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_elements.py#L278) — Test extraction of an interface.
  - `test_extract_multiple_classes(self)` — [`L289`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_elements.py#L289) — Test extraction of multiple classes.
  - `test_extract_simple_class(self)` — [`L266`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_elements.py#L266) — Test extraction of a simple class.
  - `test_extract_with_none_source(self)` — [`L418`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_elements.py#L418) — Test extraction with None source code.
  - `test_method_attribute_names_extracted(self)` — [`L336`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_elements.py#L336) — [TDD] Method attribute names must be populated — not empty list.
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`raw_text`](../../../tree_sitter_analyzer/models/base.md#CodeElement.raw_text), [`CSharpPlugin`](../../../tree_sitter_analyzer/languages/csharp_plugin.md#CSharpPlugin), [`extractor`](../../../tree_sitter_analyzer/languages/csharp_plugin.md#CSharpPlugin.extractor), [`extract_classes`](../../../tree_sitter_analyzer/languages/csharp_plugin.md#CSharpElementExtractor.extract_classes), [`extract_functions`](../../../tree_sitter_analyzer/languages/csharp_plugin.md#CSharpElementExtractor.extract_functions), [`modifiers`](../../../tree_sitter_analyzer/models/base.md#Class.modifiers), [`visibility`](../../../tree_sitter_analyzer/models/base.md#Class.visibility), [`CSharpElementExtractor`](../../../tree_sitter_analyzer/languages/csharp_plugin.md#CSharpElementExtractor), [`annotations`](../../../tree_sitter_analyzer/models/base.md#Class.annotations), [`annotations`](../../../tree_sitter_analyzer/models/base.md#Function.annotations), [`methods`](../../../tree_sitter_analyzer/models/base.md#Class.methods)  (4 test-only)

### `TestCSharpComplexityCalculation`
- def: [`tests/unit/languages/test_csharp_plugin_elements.py:725`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_elements.py#L725)
- doc: Test complexity calculation for C# code.
- signature: `class TestCSharpComplexityCalculation:`
- members:
  - `test_complexity_with_control_flow(self)` — [`L728`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_elements.py#L728) — Test complexity calculation with control flow statements.
  - `test_simple_method_low_complexity(self)` — [`L740`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_elements.py#L740) — Test that simple method has low complexity.
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`CSharpPlugin`](../../../tree_sitter_analyzer/languages/csharp_plugin.md#CSharpPlugin), [`complexity_score`](../../../tree_sitter_analyzer/models/base.md#Function.complexity_score), [`extractor`](../../../tree_sitter_analyzer/languages/csharp_plugin.md#CSharpPlugin.extractor), [`extract_functions`](../../../tree_sitter_analyzer/languages/csharp_plugin.md#CSharpElementExtractor.extract_functions)  (3 test-only)

### `TestCSharpExtractorHelpers`
- def: [`tests/unit/languages/test_csharp_plugin_elements.py:777`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_elements.py#L777)
- doc: Test CSharpElementExtractor helper methods.
- signature: `class TestCSharpExtractorHelpers:`
- members:
  - `test_cache_invalidation(self)` — [`L799`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_elements.py#L799) — Test that source code is properly set between extractions.
  - `test_get_node_text_optimized(self)` — [`L780`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_elements.py#L780) — Test optimized node text extraction.
  - `test_traverse_iterative(self)` — [`L788`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_elements.py#L788) — Test iterative tree traversal.
- uses (calls/refs, reference-scoped): [`CSharpPlugin`](../../../tree_sitter_analyzer/languages/csharp_plugin.md#CSharpPlugin), [`extract_classes`](../../../tree_sitter_analyzer/languages/csharp_plugin.md#CSharpElementExtractor.extract_classes), [`CSharpElementExtractor`](../../../tree_sitter_analyzer/languages/csharp_plugin.md#CSharpElementExtractor), [`source_code`](../../../tree_sitter_analyzer/languages/csharp_plugin.md#CSharpElementExtractor.source_code), [`_traverse_iterative`](../../../tree_sitter_analyzer/languages/csharp_plugin.md#CSharpElementExtractor._traverse_iterative), [`content_lines`](../../../tree_sitter_analyzer/languages/csharp_plugin.md#CSharpElementExtractor.content_lines)  (2 test-only)

### `TestCSharpFunctionExtraction`
- def: [`tests/unit/languages/test_csharp_plugin_elements.py:428`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_elements.py#L428)
- doc: Test C# function/method extraction.
- signature: `class TestCSharpFunctionExtraction:`
- members:
  - `test_extract_async_methods(self)` — [`L441`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_elements.py#L441) — Test extraction of async methods.
  - `test_extract_constructor(self)` — [`L473`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_elements.py#L473) — Test constructor extraction.
  - `test_extract_functions_empty_tree(self)` — [`L513`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_elements.py#L513) — Test function extraction with empty tree.
  - `test_extract_method_modifiers(self)` — [`L486`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_elements.py#L486) — Test extraction of method modifiers.
  - `test_extract_method_parameters(self)` — [`L450`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_elements.py#L450) — Test that method parameters are extracted.
  - `test_extract_method_with_parameters(self)` — [`L461`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_elements.py#L461) — Test method with parameters.
  - `test_extract_simple_method(self)` — [`L431`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_elements.py#L431) — Test extraction of simple method.
  - `test_extract_virtual_method(self)` — [`L498`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_elements.py#L498) — Test extraction of virtual method.
  - `test_method_complexity_calculation(self)` — [`L519`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_elements.py#L519) — Test method complexity calculation.
  - `test_methods_carry_parent_class(self)` — [`L531`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_elements.py#L531) — [TDD] #766 — every C# method/property/constructor must expose its owning
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`raw_text`](../../../tree_sitter_analyzer/models/base.md#CodeElement.raw_text), [`CSharpPlugin`](../../../tree_sitter_analyzer/languages/csharp_plugin.md#CSharpPlugin), [`complexity_score`](../../../tree_sitter_analyzer/models/base.md#Function.complexity_score), [`extractor`](../../../tree_sitter_analyzer/languages/csharp_plugin.md#CSharpPlugin.extractor), [`parameters`](../../../tree_sitter_analyzer/models/base.md#Function.parameters), [`extract_functions`](../../../tree_sitter_analyzer/languages/csharp_plugin.md#CSharpElementExtractor.extract_functions), [`receiver_type`](../../../tree_sitter_analyzer/models/base.md#Function.receiver_type), [`modifiers`](../../../tree_sitter_analyzer/models/base.md#Function.modifiers), [`CSharpElementExtractor`](../../../tree_sitter_analyzer/languages/csharp_plugin.md#CSharpElementExtractor)  (5 test-only)

### `TestCSharpImportExtraction`
- def: [`tests/unit/languages/test_csharp_plugin_elements.py:659`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_elements.py#L659)
- doc: Test C# import (using directive) extraction.
- signature: `class TestCSharpImportExtraction:`
- members:
  - `test_extract_imports_empty_tree(self)` — [`L682`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_elements.py#L682) — Test import extraction with empty tree.
  - `test_extract_simple_using(self)` — [`L662`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_elements.py#L662) — Test extraction of simple using directive.
  - `test_extract_static_using(self)` — [`L672`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_elements.py#L672) — Test extraction of static using directive.
  - `test_import_line_numbers(self)` — [`L688`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_elements.py#L688) — Test that import line numbers are correct.
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`CSharpPlugin`](../../../tree_sitter_analyzer/languages/csharp_plugin.md#CSharpPlugin), [`extractor`](../../../tree_sitter_analyzer/languages/csharp_plugin.md#CSharpPlugin.extractor), [`extract_imports`](../../../tree_sitter_analyzer/languages/csharp_plugin.md#CSharpElementExtractor.extract_imports), [`CSharpElementExtractor`](../../../tree_sitter_analyzer/languages/csharp_plugin.md#CSharpElementExtractor), [`is_static`](../../../tree_sitter_analyzer/models/base.md#Import.is_static)  (3 test-only)

### `TestCSharpNamespaceHandling`
- def: [`tests/unit/languages/test_csharp_plugin_elements.py:752`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_elements.py#L752)
- doc: Test namespace handling.
- signature: `class TestCSharpNamespaceHandling:`
- members:
  - `test_extract_namespace(self)` — [`L755`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_elements.py#L755) — Test namespace extraction from class.
  - `test_nested_namespace(self)` — [`L765`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_elements.py#L765) — Test handling of nested namespaces.
- uses (calls/refs, reference-scoped): [`CSharpPlugin`](../../../tree_sitter_analyzer/languages/csharp_plugin.md#CSharpPlugin), [`extractor`](../../../tree_sitter_analyzer/languages/csharp_plugin.md#CSharpPlugin.extractor), [`extract_classes`](../../../tree_sitter_analyzer/languages/csharp_plugin.md#CSharpElementExtractor.extract_classes), [`full_qualified_name`](../../../tree_sitter_analyzer/models/base.md#Class.full_qualified_name)  (3 test-only)

### `TestCSharpPropertyExtraction`
- def: [`tests/unit/languages/test_csharp_plugin_elements.py:699`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_elements.py#L699)
- doc: Test C# property extraction.
- signature: `class TestCSharpPropertyExtraction:`
- members:
  - `test_extract_auto_property(self)` — [`L702`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_elements.py#L702) — Test extraction of auto-property.
  - `test_extract_various_properties(self)` — [`L712`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_elements.py#L712) — Test extraction of various property types.
- uses (calls/refs, reference-scoped): [`raw_text`](../../../tree_sitter_analyzer/models/base.md#CodeElement.raw_text), [`CSharpPlugin`](../../../tree_sitter_analyzer/languages/csharp_plugin.md#CSharpPlugin), [`extractor`](../../../tree_sitter_analyzer/languages/csharp_plugin.md#CSharpPlugin.extractor), [`extract_classes`](../../../tree_sitter_analyzer/languages/csharp_plugin.md#CSharpElementExtractor.extract_classes)  (3 test-only)

### `TestCSharpVariableExtraction`
- def: [`tests/unit/languages/test_csharp_plugin_elements.py:584`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_elements.py#L584)
- doc: Test C# variable/field extraction.
- signature: `class TestCSharpVariableExtraction:`
- members:
  - `test_extract_const_field(self)` — [`L597`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_elements.py#L597) — Test extraction of const field.
  - `test_extract_event_field(self)` — [`L629`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_elements.py#L629) — Test extraction of event field.
  - `test_extract_field_type(self)` — [`L617`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_elements.py#L617) — Test that field type is extracted.
  - `test_extract_private_field(self)` — [`L587`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_elements.py#L587) — Test extraction of private field.
  - `test_extract_readonly_field(self)` — [`L607`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_elements.py#L607) — Test extraction of readonly field.
  - `test_extract_static_field(self)` — [`L647`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_elements.py#L647) — Test extraction of static field.
  - `test_extract_variables_empty_tree(self)` — [`L641`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_elements.py#L641) — Test variable extraction with empty tree.
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`raw_text`](../../../tree_sitter_analyzer/models/base.md#CodeElement.raw_text), [`CSharpPlugin`](../../../tree_sitter_analyzer/languages/csharp_plugin.md#CSharpPlugin), [`extractor`](../../../tree_sitter_analyzer/languages/csharp_plugin.md#CSharpPlugin.extractor), [`variable_type`](../../../tree_sitter_analyzer/models/base.md#Variable.variable_type), [`is_constant`](../../../tree_sitter_analyzer/models/base.md#Variable.is_constant), [`extract_variables`](../../../tree_sitter_analyzer/languages/csharp_plugin.md#CSharpElementExtractor.extract_variables), [`modifiers`](../../../tree_sitter_analyzer/models/base.md#Variable.modifiers), [`CSharpElementExtractor`](../../../tree_sitter_analyzer/languages/csharp_plugin.md#CSharpElementExtractor)  (3 test-only)

## Functions
- `get_tree_for_code(code: str, plugin: CSharpPlugin)` — [`L250`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_elements.py#L250) — Helper to parse C# code and return tree.

## Module values
- `ASYNC_METHOD_CODE` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_elements.py#L50)
- `COMPLEX_CLASS_CODE` — [`L75`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_elements.py#L75)
- `CONTROL_FLOW_CODE` — [`L193`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_elements.py#L193)
- `INTERFACE_CODE` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_elements.py#L36)
- `PROPERTY_VARIATIONS_CODE` — [`L153`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_elements.py#L153)
- `SIMPLE_CLASS_CODE` — [`L11`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_elements.py#L11)

