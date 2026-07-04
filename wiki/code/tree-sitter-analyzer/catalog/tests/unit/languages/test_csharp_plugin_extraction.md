---
title: 'Module: tests/unit/languages/test_csharp_plugin_extraction.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_csharp_plugin_extraction.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_csharp_plugin_extraction`/
symbols:
  get_tree_for_code: get_tree_for_code().
  TestCSharpNamespacePackageExtraction.test_qualified_namespace_produces_package_element: TestCSharpNamespacePackageExtraction#test_qualified_namespace_produces_package_element().
  TestCSharpNamespacePackageExtraction.test_package_element_language_is_csharp: TestCSharpNamespacePackageExtraction#test_package_element_language_is_csharp().
  TestCSharpNamespacePackageExtraction.test_interface_namespace_extracted: TestCSharpNamespacePackageExtraction#test_interface_namespace_extracted().
  TestCSharpPerClassNamespaceFqn.test_multiple_block_namespaces: TestCSharpPerClassNamespaceFqn#test_multiple_block_namespaces().
  TestCSharpPerClassNamespaceFqn.test_nested_block_namespaces: TestCSharpPerClassNamespaceFqn#test_nested_block_namespaces().
  TestCSharpPerClassNamespaceFqn.test_single_block_namespace_regression: TestCSharpPerClassNamespaceFqn#test_single_block_namespace_regression().
  TestCSharpPerClassNamespaceFqn.test_file_scoped_namespace_regression: TestCSharpPerClassNamespaceFqn#test_file_scoped_namespace_regression().
  TestCSharpPerClassNamespaceFqn.test_no_namespace_regression: TestCSharpPerClassNamespaceFqn#test_no_namespace_regression().
  TestCSharpPerClassNamespaceFqn.test_nested_class_under_file_scoped_namespace: TestCSharpPerClassNamespaceFqn#test_nested_class_under_file_scoped_namespace().
  TestCSharpNamespacePackageExtraction.test_simple_namespace_produces_package_element: TestCSharpNamespacePackageExtraction#test_simple_namespace_produces_package_element().
  TestCSharpNamespacePackageExtraction.test_file_scoped_namespace_produces_package_element: TestCSharpNamespacePackageExtraction#test_file_scoped_namespace_produces_package_element().
  TestCSharpNamespacePackageExtraction.test_multiple_block_namespaces_are_all_extracted: TestCSharpNamespacePackageExtraction#test_multiple_block_namespaces_are_all_extracted().
  TestCSharpNamespacePackageExtraction.test_grouped_extract_elements_includes_packages: TestCSharpNamespacePackageExtraction#test_grouped_extract_elements_includes_packages().
  TestCSharpNamespacePackageExtraction.test_no_namespace_returns_empty: TestCSharpNamespacePackageExtraction#test_no_namespace_returns_empty().
  SIMPLE_CLASS_CODE: SIMPLE_CLASS_CODE.
  TestCSharpNamespacePackageExtraction.test_none_tree_returns_empty: TestCSharpNamespacePackageExtraction#test_none_tree_returns_empty().
  INTERFACE_CODE: INTERFACE_CODE.
  TestCSharpNamespacePackageExtraction: TestCSharpNamespacePackageExtraction#
  TestCSharpPerClassNamespaceFqn: TestCSharpPerClassNamespaceFqn#
---
# Module: [`tests/unit/languages/test_csharp_plugin_extraction.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_extraction.py)

## Classes
### `TestCSharpNamespacePackageExtraction`
- def: [`tests/unit/languages/test_csharp_plugin_extraction.py:68`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_extraction.py#L68)
- doc: Issue #767 — namespace_declaration must be surfaced as a Package element
- signature: `class TestCSharpNamespacePackageExtraction:`
- members:
  - `test_file_scoped_namespace_produces_package_element(self)` — [`L99`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_extraction.py#L99) — C# 10 file-scoped namespace declarations use a distinct node type.
  - `test_grouped_extract_elements_includes_packages(self)` — [`L120`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_extraction.py#L120)
  - `test_interface_namespace_extracted(self)` — [`L142`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_extraction.py#L142) — Interface file namespace is correctly captured.
  - `test_multiple_block_namespaces_are_all_extracted(self)` — [`L109`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_extraction.py#L109)
  - `test_no_namespace_returns_empty(self)` — [`L128`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_extraction.py#L128) — A C# file without a namespace declaration returns no Package.
  - `test_none_tree_returns_empty(self)` — [`L137`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_extraction.py#L137) — extract_packages with a None tree returns an empty list.
  - `test_package_element_language_is_csharp(self)` — [`L81`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_extraction.py#L81) — Extracted Package element carries language='csharp'.
  - `test_qualified_namespace_produces_package_element(self)` — [`L72`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_extraction.py#L72) — Qualified namespace (MyApp.Models) is extracted as Package.
  - `test_simple_namespace_produces_package_element(self)` — [`L89`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_extraction.py#L89) — Single-segment namespace (MyApp) is also extracted.
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`language`](../../../tree_sitter_analyzer/models/base.md#CodeElement.language), [`CSharpPlugin`](../../../tree_sitter_analyzer/languages/csharp_plugin.md#CSharpPlugin), [`extractor`](../../../tree_sitter_analyzer/languages/csharp_plugin.md#CSharpPlugin.extractor), [`extract_packages`](../../../tree_sitter_analyzer/languages/csharp_plugin.md#CSharpElementExtractor.extract_packages), [`CSharpElementExtractor`](../../../tree_sitter_analyzer/languages/csharp_plugin.md#CSharpElementExtractor), [`extract_elements`](../../../tree_sitter_analyzer/languages/csharp_plugin.md#CSharpPlugin.extract_elements)  (3 test-only)

### `TestCSharpPerClassNamespaceFqn`
- def: [`tests/unit/languages/test_csharp_plugin_extraction.py:152`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_extraction.py#L152)
- doc: Bug #977 — each class's FQN must reflect its OWN enclosing namespace.
- signature: `class TestCSharpPerClassNamespaceFqn:`
- members:
  - `test_file_scoped_namespace_regression(self)` — [`L186`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_extraction.py#L186) — A file-scoped namespace still produces the correct FQN.
  - `test_multiple_block_namespaces(self)` — [`L155`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_extraction.py#L155) — Classes in the 2nd+ namespace get that namespace, not the first.
  - `test_nested_block_namespaces(self)` — [`L166`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_extraction.py#L166) — Nested block namespaces concatenate with '.'.
  - `test_nested_class_under_file_scoped_namespace(self)` — [`L206`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_extraction.py#L206) — A class nested inside another class under a file-scoped namespace.
  - `test_no_namespace_regression(self)` — [`L196`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_extraction.py#L196) — A class with no enclosing namespace keeps its bare name.
  - `test_single_block_namespace_regression(self)` — [`L176`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_extraction.py#L176) — A single block namespace still produces the correct FQN.
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`CSharpPlugin`](../../../tree_sitter_analyzer/languages/csharp_plugin.md#CSharpPlugin), [`extractor`](../../../tree_sitter_analyzer/languages/csharp_plugin.md#CSharpPlugin.extractor), [`extract_classes`](../../../tree_sitter_analyzer/languages/csharp_plugin.md#CSharpElementExtractor.extract_classes), [`full_qualified_name`](../../../tree_sitter_analyzer/models/base.md#Class.full_qualified_name)  (1 test-only)

## Functions
- `get_tree_for_code(code: str, plugin: CSharpPlugin)` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_extraction.py#L50) — Helper to parse C# code and return tree.

## Module values
- `INTERFACE_CODE` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_extraction.py#L36)
- `SIMPLE_CLASS_CODE` — [`L11`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_extraction.py#L11)

