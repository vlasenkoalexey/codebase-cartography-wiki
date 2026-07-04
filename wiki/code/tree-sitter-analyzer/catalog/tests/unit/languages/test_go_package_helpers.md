---
title: 'Module: tests/unit/languages/test_go_package_helpers.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_go_package_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_go_package_helpers`/
symbols:
  TestExtractGoPackage.test_extracts_package: TestExtractGoPackage#test_extracts_package().
  TestGoPackageName.test_finds_package_identifier: TestGoPackageName#test_finds_package_identifier().
  TestExtractGoPackage.test_no_identifier_returns_none: TestExtractGoPackage#test_no_identifier_returns_none().
  TestGoPackageName.test_no_identifier: TestGoPackageName#test_no_identifier().
  TestGoPackageName.test_wrong_child_type: TestGoPackageName#test_wrong_child_type().
  _get_text: _get_text().
  _mock_node: _mock_node().
  TestExtractGoPackage.test_exception_returns_none: TestExtractGoPackage#test_exception_returns_none().
  _mock_identifier_child: _mock_identifier_child().
  TestExtractGoPackage: TestExtractGoPackage#
  TestGoPackageName: TestGoPackageName#
---
# Module: [`tests/unit/languages/test_go_package_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_package_helpers.py)

## Classes
### `TestExtractGoPackage`
- def: [`tests/unit/languages/test_go_package_helpers.py:34`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_package_helpers.py#L34)
- signature: `class TestExtractGoPackage:`
- members:
  - `test_exception_returns_none(self)` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_package_helpers.py#L50)
  - `test_extracts_package(self)` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_package_helpers.py#L35)
  - `test_no_identifier_returns_none(self)` — [`L43`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_package_helpers.py#L43)
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`language`](../../../tree_sitter_analyzer/models/base.md#CodeElement.language), [`Package`](../../../tree_sitter_analyzer/models/base.md#Package), [`extract_go_package`](../../../tree_sitter_analyzer/languages/_go_package_helpers.md#extract_go_package)  (3 test-only)

### `TestGoPackageName`
- def: [`tests/unit/languages/test_go_package_helpers.py:58`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_package_helpers.py#L58)
- signature: `class TestGoPackageName:`
- members:
  - `test_finds_package_identifier(self)` — [`L59`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_package_helpers.py#L59)
  - `test_no_identifier(self)` — [`L63`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_package_helpers.py#L63)
  - `test_wrong_child_type(self)` — [`L67`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_package_helpers.py#L67)
- uses (calls/refs, reference-scoped): [`_go_package_name`](../../../tree_sitter_analyzer/languages/_go_package_helpers.md#_go_package_name)  (3 test-only)

## Functions
- `_get_text(node)` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_package_helpers.py#L28)
- `_mock_identifier_child(name="main")` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_package_helpers.py#L21)
- `_mock_node(children=None, start_row=0, end_row=0, text="package main")` — [`L12`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_package_helpers.py#L12)

