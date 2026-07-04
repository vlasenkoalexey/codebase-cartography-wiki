---
title: 'Module: tests/unit/languages/test_java_annotation_extraction.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_java_annotation_extraction.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_java_annotation_extraction`/
symbols:
  TestAnnotationExtractionOrder.test_reset_caches_preserves_annotations: TestAnnotationExtractionOrder#test_reset_caches_preserves_annotations().
  TestFieldAnnotationExtraction.test_field_annotation_extraction_pure_unit: TestFieldAnnotationExtraction#test_field_annotation_extraction_pure_unit().
  TestAnnotationExtractionOrder.test_annotations_preserved_after_extract_functions: TestAnnotationExtractionOrder#test_annotations_preserved_after_extract_functions().
  call: call().
  OWNER_CONTROLLER: OWNER_CONTROLLER.
  VET: VET.
  mcp_server: mcp_server().
  TestAnnotationExtractionOrder.test_methods_carry_annotations_from_extract_elements: TestAnnotationExtractionOrder#test_methods_carry_annotations_from_extract_elements().
  TestMCPToolAnnotationOutput.test_owner_controller_class_has_controller_annotation: TestMCPToolAnnotationOutput#test_owner_controller_class_has_controller_annotation().
  TestMCPToolAnnotationOutput.test_owner_controller_methods_have_mapping_annotations: TestMCPToolAnnotationOutput#test_owner_controller_methods_have_mapping_annotations().
  TestMCPToolAnnotationOutput.test_model_attribute_method_has_annotation: TestMCPToolAnnotationOutput#test_model_attribute_method_has_annotation().
  TestFieldAnnotationExtraction.test_vet_specialties_has_manytomany_annotation: TestFieldAnnotationExtraction#test_vet_specialties_has_manytomany_annotation().
  TestFieldAnnotationExtraction.test_vet_specialties_has_jointable_annotation: TestFieldAnnotationExtraction#test_vet_specialties_has_jointable_annotation().
  TestFieldAnnotationExtraction.test_annotation_text_includes_parameters: TestFieldAnnotationExtraction#test_annotation_text_includes_parameters().
  PETCLINIC_BASE: PETCLINIC_BASE.
  pytestmark: pytestmark.
  TestAnnotationExtractionOrder: TestAnnotationExtractionOrder#
  TestMCPToolAnnotationOutput: TestMCPToolAnnotationOutput#
  TestFieldAnnotationExtraction: TestFieldAnnotationExtraction#
---
# Module: [`tests/unit/languages/test_java_annotation_extraction.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_annotation_extraction.py)

## Classes
### `TestAnnotationExtractionOrder`
- def: [`tests/unit/languages/test_java_annotation_extraction.py:54`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_annotation_extraction.py#L54)
- doc: extract_annotations() must run before extract_functions/extract_classes
- signature: `class TestAnnotationExtractionOrder:`
- members:
  - `test_annotations_preserved_after_extract_functions(self)` — [`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_annotation_extraction.py#L58) — self.annotations must survive a call to extract_functions().
  - `test_methods_carry_annotations_from_extract_elements(self)` — [`L91`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_annotation_extraction.py#L91) — extract_elements() must return functions with non-empty annotations.
  - `test_reset_caches_preserves_annotations(self)` — [`L125`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_annotation_extraction.py#L125) — _reset_caches() must clear lookup caches but preserve self.annotations.
- uses (calls/refs, reference-scoped): [`JavaElementExtractor`](../../../tree_sitter_analyzer/languages/java_plugin.md#JavaElementExtractor), [`JavaPlugin`](../../../tree_sitter_analyzer/languages/java_plugin.md#JavaPlugin), [`extract_annotations`](../../../tree_sitter_analyzer/languages/java_plugin.md#JavaElementExtractor.extract_annotations), [`extract_functions`](../../../tree_sitter_analyzer/languages/java_plugin.md#JavaElementExtractor.extract_functions), [`extract_elements`](../../../tree_sitter_analyzer/languages/java_plugin.md#JavaPlugin.extract_elements), [`_reset_caches`](../../../tree_sitter_analyzer/languages/java_plugin.md#JavaElementExtractor._reset_caches), [`_annotation_cache`](../../../tree_sitter_analyzer/languages/java_plugin.md#JavaElementExtractor._annotation_cache), [`_node_text_cache`](../../../tree_sitter_analyzer/languages/java_plugin.md#JavaElementExtractor._node_text_cache), [`annotations`](../../../tree_sitter_analyzer/languages/java_plugin.md#JavaElementExtractor.annotations)

### `TestFieldAnnotationExtraction`
- def: [`tests/unit/languages/test_java_annotation_extraction.py:232`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_annotation_extraction.py#L232)
- doc: Field-level annotations must be extracted (field_declaration in containers).
- signature: `class TestFieldAnnotationExtraction:`
- members:
  - `test_annotation_text_includes_parameters(self, mcp_server)` — [`L275`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_annotation_extraction.py#L275) — Annotation text must include parameters, not just name.
  - `test_field_annotation_extraction_pure_unit(self)` — [`L303`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_annotation_extraction.py#L303) — Unit test: field annotations extracted without MCP server.
  - `test_vet_specialties_has_jointable_annotation(self, mcp_server)` — [`L256`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_annotation_extraction.py#L256) — Vet.specialties field must have @JoinTable annotation.
  - `test_vet_specialties_has_manytomany_annotation(self, mcp_server)` — [`L235`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_annotation_extraction.py#L235) — Vet.specialties field must have @ManyToMany annotation.
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`JavaElementExtractor`](../../../tree_sitter_analyzer/languages/java_plugin.md#JavaElementExtractor), [`extract_variables`](../../../tree_sitter_analyzer/languages/java_plugin.md#JavaElementExtractor.extract_variables), [`extract_annotations`](../../../tree_sitter_analyzer/languages/java_plugin.md#JavaElementExtractor.extract_annotations), [`annotations`](../../../tree_sitter_analyzer/models/base.md#Variable.annotations)  (2 test-only)

### `TestMCPToolAnnotationOutput`
- def: [`tests/unit/languages/test_java_annotation_extraction.py:150`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_annotation_extraction.py#L150)
- doc: MCP analyze_code_structure must surface annotations from model objects.
- signature: `class TestMCPToolAnnotationOutput:`
- members:
  - `test_model_attribute_method_has_annotation(self, mcp_server)` — [`L207`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_annotation_extraction.py#L207) — findOwner() with @ModelAttribute must have that annotation.
  - `test_owner_controller_class_has_controller_annotation(self, mcp_server)` — [`L153`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_annotation_extraction.py#L153) — OwnerController class must have @Controller in output.
  - `test_owner_controller_methods_have_mapping_annotations(self, mcp_server)` — [`L177`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_annotation_extraction.py#L177) — Methods with @GetMapping/@PostMapping must have those annotations in output.
- uses (calls/refs, reference-scoped): (2 test-only callers)

## Functions
- `call(coro)` — [`L44`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_annotation_extraction.py#L44) — Run async coroutine synchronously.
- `mcp_server()` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_annotation_extraction.py#L37) — MCP server pointed at spring-petclinic.

## Module values
- `OWNER_CONTROLLER` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_annotation_extraction.py#L22)
- `PETCLINIC_BASE` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_annotation_extraction.py#L21)
- `VET` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_annotation_extraction.py#L26)
- `pytestmark` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_annotation_extraction.py#L30)

