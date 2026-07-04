---
title: 'Module: tests/unit/mcp/tools/test_element_extractor_coverage.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/tools/test_element_extractor_coverage.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.tools.test_element_extractor_coverage`/
symbols:
  _make_element: _make_element().
  _make_result: _make_result().
  TestGetFunctions.test_extracts_functions: TestGetFunctions#test_extracts_functions().
  TestGetFunctions.test_skips_non_functions: TestGetFunctions#test_skips_non_functions().
  TestGetFunctions.test_function_attributes: TestGetFunctions#test_function_attributes().
  TestGetClasses.test_extracts_classes_with_methods_attr: TestGetClasses#test_extracts_classes_with_methods_attr().
  TestGetClasses.test_class_without_methods_computes_from_line_range: TestGetClasses#test_class_without_methods_computes_from_line_range().
  TestGetClasses.test_no_classes: TestGetClasses#test_no_classes().
  TestGetImports.test_extracts_imports: TestGetImports#test_extracts_imports().
  TestGetImports.test_no_imports: TestGetImports#test_no_imports().
  TestGetAllExports.test_exports_classes_functions_constants: TestGetAllExports#test_exports_classes_functions_constants().
  TestGetAllExports.test_class_export_has_method_count: TestGetAllExports#test_class_export_has_method_count().
  TestGetStructure.test_extracts_structure: TestGetStructure#test_extracts_structure().
  TestGetStructure.test_truncates_at_30: TestGetStructure#test_truncates_at_30().
  TestGetFunctionsInClass.test_finds_class_methods: TestGetFunctionsInClass#test_finds_class_methods().
  TestGetFunctionsInClass.test_class_not_found: TestGetFunctionsInClass#test_class_not_found().
  TestGetFunctionsInClass.test_method_attributes: TestGetFunctionsInClass#test_method_attributes().
  TestExtractElements.test_valid_python_file: TestExtractElements#test_valid_python_file().
  TestGetFunctions.test_empty_elements: TestGetFunctions#test_empty_elements().
  TestGetAllExports.test_empty: TestGetAllExports#test_empty().
  TestGetStructure.test_empty: TestGetStructure#test_empty().
  TestExtractElements.test_unsupported_language_returns_none: TestExtractElements#test_unsupported_language_returns_none().
  TestExtractElements.test_binary_file_returns_none: TestExtractElements#test_binary_file_returns_none().
  TestExtractElements: TestExtractElements#
  TestGetFunctions: TestGetFunctions#
  TestGetClasses: TestGetClasses#
  TestGetImports: TestGetImports#
  TestGetAllExports: TestGetAllExports#
  TestGetStructure: TestGetStructure#
  TestGetFunctionsInClass: TestGetFunctionsInClass#
---
# Module: [`tests/unit/mcp/tools/test_element_extractor_coverage.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_element_extractor_coverage.py)

## Classes
### `TestExtractElements`
- def: [`tests/unit/mcp/tools/test_element_extractor_coverage.py:45`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_element_extractor_coverage.py#L45)
- signature: `class TestExtractElements:`
- members:
  - `test_binary_file_returns_none(self, tmp_path)` — [`L51`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_element_extractor_coverage.py#L51)
  - `test_unsupported_language_returns_none(self, tmp_path)` — [`L46`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_element_extractor_coverage.py#L46)
  - `test_valid_python_file(self, tmp_path)` — [`L56`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_element_extractor_coverage.py#L56)
- uses (calls/refs, reference-scoped): [`elements`](../../../../tree_sitter_analyzer/models/result.md#AnalysisResult.elements), [`extract_elements`](../../../../tree_sitter_analyzer/mcp/tools/utils/element_extractor.md#extract_elements)

### `TestGetAllExports`
- def: [`tests/unit/mcp/tools/test_element_extractor_coverage.py:156`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_element_extractor_coverage.py#L156)
- signature: `class TestGetAllExports:`
- members:
  - `test_class_export_has_method_count(self)` — [`L180`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_element_extractor_coverage.py#L180)
  - `test_empty(self)` — [`L187`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_element_extractor_coverage.py#L187)
  - `test_exports_classes_functions_constants(self)` — [`L157`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_element_extractor_coverage.py#L157)
- uses (calls/refs, reference-scoped): [`get_all_exports`](../../../../tree_sitter_analyzer/mcp/tools/utils/element_extractor.md#get_all_exports)  (2 test-only)

### `TestGetClasses`
- def: [`tests/unit/mcp/tools/test_element_extractor_coverage.py:109`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_element_extractor_coverage.py#L109)
- signature: `class TestGetClasses:`
- members:
  - `test_class_without_methods_computes_from_line_range(self)` — [`L121`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_element_extractor_coverage.py#L121)
  - `test_extracts_classes_with_methods_attr(self)` — [`L110`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_element_extractor_coverage.py#L110)
  - `test_no_classes(self)` — [`L133`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_element_extractor_coverage.py#L133)
- uses (calls/refs, reference-scoped): [`get_classes`](../../../../tree_sitter_analyzer/mcp/tools/utils/element_extractor.md#get_classes)  (2 test-only)

### `TestGetFunctions`
- def: [`tests/unit/mcp/tools/test_element_extractor_coverage.py:64`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_element_extractor_coverage.py#L64)
- signature: `class TestGetFunctions:`
- members:
  - `test_empty_elements(self)` — [`L87`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_element_extractor_coverage.py#L87)
  - `test_extracts_functions(self)` — [`L65`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_element_extractor_coverage.py#L65)
  - `test_function_attributes(self)` — [`L91`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_element_extractor_coverage.py#L91)
  - `test_skips_non_functions(self)` — [`L77`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_element_extractor_coverage.py#L77)
- uses (calls/refs, reference-scoped): [`get_functions`](../../../../tree_sitter_analyzer/mcp/tools/utils/element_extractor.md#get_functions)  (2 test-only)

### `TestGetFunctionsInClass`
- def: [`tests/unit/mcp/tools/test_element_extractor_coverage.py:216`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_element_extractor_coverage.py#L216)
- signature: `class TestGetFunctionsInClass:`
- members:
  - `test_class_not_found(self)` — [`L226`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_element_extractor_coverage.py#L226)
  - `test_finds_class_methods(self)` — [`L217`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_element_extractor_coverage.py#L217)
  - `test_method_attributes(self)` — [`L231`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_element_extractor_coverage.py#L231)
- uses (calls/refs, reference-scoped): [`get_functions_in_class`](../../../../tree_sitter_analyzer/mcp/tools/utils/element_extractor.md#get_functions_in_class)  (2 test-only)

### `TestGetImports`
- def: [`tests/unit/mcp/tools/test_element_extractor_coverage.py:139`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_element_extractor_coverage.py#L139)
- signature: `class TestGetImports:`
- members:
  - `test_extracts_imports(self)` — [`L140`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_element_extractor_coverage.py#L140)
  - `test_no_imports(self)` — [`L150`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_element_extractor_coverage.py#L150)
- uses (calls/refs, reference-scoped): [`get_imports`](../../../../tree_sitter_analyzer/mcp/tools/utils/element_extractor.md#get_imports)  (2 test-only)

### `TestGetStructure`
- def: [`tests/unit/mcp/tools/test_element_extractor_coverage.py:192`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_element_extractor_coverage.py#L192)
- signature: `class TestGetStructure:`
- members:
  - `test_empty(self)` — [`L211`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_element_extractor_coverage.py#L211)
  - `test_extracts_structure(self)` — [`L193`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_element_extractor_coverage.py#L193)
  - `test_truncates_at_30(self)` — [`L205`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_element_extractor_coverage.py#L205)
- uses (calls/refs, reference-scoped): [`get_structure`](../../../../tree_sitter_analyzer/mcp/tools/utils/element_extractor.md#get_structure)  (2 test-only)

## Functions
- `_make_element(name="test", element_type="function", start_line=1, end_line=10, parameters=None, is_static=False, visibility="public", methods=None)` — [`L17`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_element_extractor_coverage.py#L17)
- `_make_result(elements)` — [`L39`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_element_extractor_coverage.py#L39)

