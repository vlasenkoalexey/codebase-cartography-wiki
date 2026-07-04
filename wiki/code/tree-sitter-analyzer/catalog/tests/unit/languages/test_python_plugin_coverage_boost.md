---
title: 'Module: tests/unit/languages/test_python_plugin_coverage_boost.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_python_plugin_coverage_boost.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_python_plugin_coverage_boost`/
symbols:
  _parse: _parse().
  TestExtractDetailedFunctionInfo.find_nodes: TestExtractDetailedFunctionInfo#find_nodes().
  TestExtractDecoratorsFromNode.find_nodes: TestExtractDecoratorsFromNode#find_nodes().
  TestExtractReturnTypeFromNode.find_nodes: TestExtractReturnTypeFromNode#find_nodes().
  TestExtractDocstringFromNode.find_nodes: TestExtractDocstringFromNode#find_nodes().
  TestExtractSuperclassesFromNode.find_nodes: TestExtractSuperclassesFromNode#find_nodes().
  TestExtractPackages.test_with_init_file: TestExtractPackages#test_with_init_file().
  TestExtractPackages.test_no_init_file: TestExtractPackages#test_no_init_file().
  TestExtractPackages.test_no_current_file: TestExtractPackages#test_no_current_file().
  TestExtractDecoratorsFromNode.test_decorated_function: TestExtractDecoratorsFromNode#test_decorated_function().
  TestExtractDecoratorsFromNode.test_no_decorators: TestExtractDecoratorsFromNode#test_no_decorators().
  TestExtractReturnTypeFromNode.test_with_return_type: TestExtractReturnTypeFromNode#test_with_return_type().
  TestExtractReturnTypeFromNode.test_no_return_type: TestExtractReturnTypeFromNode#test_no_return_type().
  TestExtractDocstringFromNode.test_function_docstring: TestExtractDocstringFromNode#test_function_docstring().
  TestExtractDocstringFromNode.test_class_docstring: TestExtractDocstringFromNode#test_class_docstring().
  TestExtractFunctionBody.test_simple_body: TestExtractFunctionBody#test_simple_body().
  TestExtractSuperclassesFromNode.test_with_superclass: TestExtractSuperclassesFromNode#test_with_superclass().
  TestExtractSuperclassesFromNode.test_no_superclass: TestExtractSuperclassesFromNode#test_no_superclass().
  TestExtractDetailedFunctionInfo.test_async_function: TestExtractDetailedFunctionInfo#test_async_function().
  TestExtractDetailedFunctionInfo.test_dunder_method_is_public: TestExtractDetailedFunctionInfo#test_dunder_method_is_public().
  TestExtractDetailedFunctionInfo.test_private_method: TestExtractDetailedFunctionInfo#test_private_method().
  TestExtractFunctionBody.find_nodes: TestExtractFunctionBody#find_nodes().
  plugin: plugin().
  extractor: extractor().
  test_python_plugin_basic: test_python_plugin_basic().
  TestExtractImportsManual.test_simple_import: TestExtractImportsManual#test_simple_import().
  TestExtractImportsManual.test_from_import: TestExtractImportsManual#test_from_import().
  TestExtractImportsManual.test_from_import_single: TestExtractImportsManual#test_from_import_single().
  TestExtractImportsManual.test_empty_code: TestExtractImportsManual#test_empty_code().
  TestExtractImportsManual.test_no_imports: TestExtractImportsManual#test_no_imports().
  TestGetNodeTypeForElement.test_function: TestGetNodeTypeForElement#test_function().
  TestGetNodeTypeForElement.test_class: TestGetNodeTypeForElement#test_class().
  TestGetNodeTypeForElement.test_variable: TestGetNodeTypeForElement#test_variable().
  TestGetNodeTypeForElement.test_import: TestGetNodeTypeForElement#test_import().
  TestExtractImportsManual: TestExtractImportsManual#
  TestExtractPackages: TestExtractPackages#
  TestGetNodeTypeForElement: TestGetNodeTypeForElement#
  TestGetNodeTypeForElement.test_unknown: TestGetNodeTypeForElement#test_unknown().
  TestExtractDecoratorsFromNode: TestExtractDecoratorsFromNode#
  TestExtractReturnTypeFromNode: TestExtractReturnTypeFromNode#
  TestExtractDocstringFromNode: TestExtractDocstringFromNode#
  TestExtractFunctionBody: TestExtractFunctionBody#
  TestExtractSuperclassesFromNode: TestExtractSuperclassesFromNode#
  TestCalculateComplexity: TestCalculateComplexity#
  TestCalculateComplexity.test_simple: TestCalculateComplexity#test_simple().
  TestCalculateComplexity.test_with_branches: TestCalculateComplexity#test_with_branches().
  TestExtractDetailedFunctionInfo: TestExtractDetailedFunctionInfo#
  TestGetElementCategories: TestGetElementCategories#
  TestGetElementCategories.test_returns_dict: TestGetElementCategories#test_returns_dict().
  TestGetElementCategories.test_all_values_are_lists: TestGetElementCategories#test_all_values_are_lists().
  TestExtractElementsErrorHandling: TestExtractElementsErrorHandling#
  TestExtractElementsErrorHandling.test_with_bad_tree: TestExtractElementsErrorHandling#test_with_bad_tree().
  TestSupportedQueries: TestSupportedQueries#
  TestSupportedQueries.test_supported_queries_list: TestSupportedQueries#test_supported_queries_list().
---
# Module: [`tests/unit/languages/test_python_plugin_coverage_boost.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_coverage_boost.py)

## Classes
### `TestCalculateComplexity`
- def: [`tests/unit/languages/test_python_plugin_coverage_boost.py:325`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_coverage_boost.py#L325)
- signature: `class TestCalculateComplexity:`
- members:
  - `test_simple(self, extractor)` — [`L326`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_coverage_boost.py#L326)
  - `test_with_branches(self, extractor)` — [`L330`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_coverage_boost.py#L330)

### `TestExtractDecoratorsFromNode`
- def: [`tests/unit/languages/test_python_plugin_coverage_boost.py:159`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_coverage_boost.py#L159)
- signature: `class TestExtractDecoratorsFromNode:`
- members:
  - `find_nodes(node, node_type)` — [`L165`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_coverage_boost.py#L165)
  - `test_decorated_function(self, extractor, plugin)` — [`L160`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_coverage_boost.py#L160)
  - `test_no_decorators(self, extractor, plugin)` — [`L178`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_coverage_boost.py#L178)
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `TestExtractDetailedFunctionInfo`
- def: [`tests/unit/languages/test_python_plugin_coverage_boost.py:336`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_coverage_boost.py#L336)
- signature: `class TestExtractDetailedFunctionInfo:`
- members:
  - `find_nodes(node, node_type)` — [`L341`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_coverage_boost.py#L341)
  - `test_async_function(self, extractor, plugin)` — [`L337`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_coverage_boost.py#L337)
  - `test_dunder_method_is_public(self, extractor, plugin)` — [`L357`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_coverage_boost.py#L357)
  - `test_private_method(self, extractor, plugin)` — [`L376`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_coverage_boost.py#L376)
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `TestExtractDocstringFromNode`
- def: [`tests/unit/languages/test_python_plugin_coverage_boost.py:232`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_coverage_boost.py#L232)
- signature: `class TestExtractDocstringFromNode:`
- members:
  - `find_nodes(node, node_type)` — [`L237`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_coverage_boost.py#L237)
  - `test_class_docstring(self, extractor, plugin)` — [`L251`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_coverage_boost.py#L251)
  - `test_function_docstring(self, extractor, plugin)` — [`L233`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_coverage_boost.py#L233)
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `TestExtractElementsErrorHandling`
- def: [`tests/unit/languages/test_python_plugin_coverage_boost.py:413`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_coverage_boost.py#L413)
- signature: `class TestExtractElementsErrorHandling:`
- members:
  - `test_with_bad_tree(self, plugin)` — [`L414`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_coverage_boost.py#L414)

### `TestExtractFunctionBody`
- def: [`tests/unit/languages/test_python_plugin_coverage_boost.py:270`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_coverage_boost.py#L270)
- signature: `class TestExtractFunctionBody:`
- members:
  - `find_nodes(node, node_type)` — [`L275`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_coverage_boost.py#L275)
  - `test_simple_body(self, extractor, plugin)` — [`L271`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_coverage_boost.py#L271)
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `TestExtractImportsManual`
- def: [`tests/unit/languages/test_python_plugin_coverage_boost.py:57`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_coverage_boost.py#L57)
- signature: `class TestExtractImportsManual:`
- members:
  - `test_empty_code(self, extractor, plugin)` — [`L84`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_coverage_boost.py#L84)
  - `test_from_import(self, extractor, plugin)` — [`L67`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_coverage_boost.py#L67)
  - `test_from_import_single(self, extractor, plugin)` — [`L77`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_coverage_boost.py#L77)
  - `test_no_imports(self, extractor, plugin)` — [`L90`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_coverage_boost.py#L90)
  - `test_simple_import(self, extractor, plugin)` — [`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_coverage_boost.py#L58)
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `TestExtractPackages`
- def: [`tests/unit/languages/test_python_plugin_coverage_boost.py:97`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_coverage_boost.py#L97)
- signature: `class TestExtractPackages:`
- members:
  - `test_no_current_file(self, extractor)` — [`L122`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_coverage_boost.py#L122)
  - `test_no_init_file(self, extractor)` — [`L114`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_coverage_boost.py#L114)
  - `test_with_init_file(self, extractor)` — [`L98`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_coverage_boost.py#L98)
- uses (calls/refs, reference-scoped): [`PythonPlugin`](../../../tree_sitter_analyzer/languages/python_plugin/plugin.md#PythonPlugin)  (1 test-only)

### `TestExtractReturnTypeFromNode`
- def: [`tests/unit/languages/test_python_plugin_coverage_boost.py:196`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_coverage_boost.py#L196)
- signature: `class TestExtractReturnTypeFromNode:`
- members:
  - `find_nodes(node, node_type)` — [`L201`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_coverage_boost.py#L201)
  - `test_no_return_type(self, extractor, plugin)` — [`L214`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_coverage_boost.py#L214)
  - `test_with_return_type(self, extractor, plugin)` — [`L197`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_coverage_boost.py#L197)
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `TestExtractSuperclassesFromNode`
- def: [`tests/unit/languages/test_python_plugin_coverage_boost.py:289`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_coverage_boost.py#L289)
- signature: `class TestExtractSuperclassesFromNode:`
- members:
  - `find_nodes(node, node_type)` — [`L294`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_coverage_boost.py#L294)
  - `test_no_superclass(self, extractor, plugin)` — [`L307`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_coverage_boost.py#L307)
  - `test_with_superclass(self, extractor, plugin)` — [`L290`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_coverage_boost.py#L290)
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `TestGetElementCategories`
- def: [`tests/unit/languages/test_python_plugin_coverage_boost.py:396`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_coverage_boost.py#L396)
- signature: `class TestGetElementCategories:`
- members:
  - `test_all_values_are_lists(self, plugin)` — [`L407`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_coverage_boost.py#L407)
  - `test_returns_dict(self, plugin)` — [`L397`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_coverage_boost.py#L397)

### `TestGetNodeTypeForElement`
- def: [`tests/unit/languages/test_python_plugin_coverage_boost.py:130`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_coverage_boost.py#L130)
- signature: `class TestGetNodeTypeForElement:`
- members:
  - `test_class(self, plugin)` — [`L137`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_coverage_boost.py#L137)
  - `test_function(self, plugin)` — [`L131`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_coverage_boost.py#L131)
  - `test_import(self, plugin)` — [`L149`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_coverage_boost.py#L149)
  - `test_unknown(self, plugin)` — [`L155`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_coverage_boost.py#L155)
  - `test_variable(self, plugin)` — [`L143`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_coverage_boost.py#L143)
- uses (calls/refs, reference-scoped): [`Function`](../../../tree_sitter_analyzer/models/base.md#Function), [`Class`](../../../tree_sitter_analyzer/models/base.md#Class), [`Variable`](../../../tree_sitter_analyzer/models/base.md#Variable), [`Import`](../../../tree_sitter_analyzer/models/base.md#Import)

### `TestSupportedQueries`
- def: [`tests/unit/languages/test_python_plugin_coverage_boost.py:419`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_coverage_boost.py#L419)
- signature: `class TestSupportedQueries:`
- members:
  - `test_supported_queries_list(self, plugin)` — [`L420`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_coverage_boost.py#L420)

## Functions
- `_parse(plugin, code)` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_coverage_boost.py#L24)
- `extractor()` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_coverage_boost.py#L20)
- `plugin()` — [`L15`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_coverage_boost.py#L15)
- `test_python_plugin_basic(plugin)` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_coverage_boost.py#L30)

