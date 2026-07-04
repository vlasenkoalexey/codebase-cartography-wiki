---
title: 'Module: tests/unit/mcp/test_analyze_code_structure_modifiers.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_analyze_code_structure_modifiers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_analyze_code_structure_modifiers`/TestAnalyzeCodeStructureTool
symbols:
  TestAnalyzeCodeStructureToolConvertParameters.test_convert_parameters_empty: ConvertParameters#test_convert_parameters_empty().
  TestAnalyzeCodeStructureToolConvertParameters.test_convert_parameters_dict: ConvertParameters#test_convert_parameters_dict().
  TestAnalyzeCodeStructureToolConvertParameters.test_convert_parameters_object: ConvertParameters#test_convert_parameters_object().
  TestAnalyzeCodeStructureToolGetMethodModifiers.test_get_method_modifiers_none: GetMethodModifiers#test_get_method_modifiers_none().
  TestAnalyzeCodeStructureToolGetMethodModifiers.test_get_method_modifiers_static: GetMethodModifiers#test_get_method_modifiers_static().
  TestAnalyzeCodeStructureToolGetMethodModifiers.test_get_method_modifiers_final: GetMethodModifiers#test_get_method_modifiers_final().
  TestAnalyzeCodeStructureToolGetMethodModifiers.test_get_method_modifiers_abstract: GetMethodModifiers#test_get_method_modifiers_abstract().
  TestAnalyzeCodeStructureToolGetMethodModifiers.test_get_method_modifiers_multiple: GetMethodModifiers#test_get_method_modifiers_multiple().
  TestAnalyzeCodeStructureToolGetFieldModifiers.test_get_field_modifiers_none: GetFieldModifiers#test_get_field_modifiers_none().
  TestAnalyzeCodeStructureToolGetFieldModifiers.test_get_field_modifiers_private: GetFieldModifiers#test_get_field_modifiers_private().
  TestAnalyzeCodeStructureToolGetFieldModifiers.test_get_field_modifiers_static: GetFieldModifiers#test_get_field_modifiers_static().
  TestAnalyzeCodeStructureToolGetFieldModifiers.test_get_field_modifiers_multiple: GetFieldModifiers#test_get_field_modifiers_multiple().
  TestAnalyzeCodeStructureToolGetMethodParameters.test_get_method_parameters_empty: GetMethodParameters#test_get_method_parameters_empty().
  TestAnalyzeCodeStructureToolGetMethodParameters.test_get_method_parameters_list_of_strings: GetMethodParameters#test_get_method_parameters_list_of_strings().
  TestAnalyzeCodeStructureToolGetMethodParameters.test_get_method_parameters_list_of_dicts: GetMethodParameters#test_get_method_parameters_list_of_dicts().
  TestAnalyzeCodeStructureToolGetMethodParameters.test_get_method_parameters_mixed: GetMethodParameters#test_get_method_parameters_mixed().
  TestAnalyzeCodeStructureToolConvertParameters: ConvertParameters#
  TestAnalyzeCodeStructureToolGetMethodModifiers: GetMethodModifiers#
  TestAnalyzeCodeStructureToolGetFieldModifiers: GetFieldModifiers#
  TestAnalyzeCodeStructureToolGetMethodParameters: GetMethodParameters#
---
# Module: [`tests/unit/mcp/test_analyze_code_structure_modifiers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_modifiers.py)

## Classes
### `TestAnalyzeCodeStructureToolConvertParameters`
- def: [`tests/unit/mcp/test_analyze_code_structure_modifiers.py:14`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_modifiers.py#L14)
- doc: Tests for _convert_parameters helper.
- signature: `class TestAnalyzeCodeStructureToolConvertParameters:`
- members:
  - `test_convert_parameters_dict(self)` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_modifiers.py#L22) — Test converting dict parameters.
  - `test_convert_parameters_empty(self)` — [`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_modifiers.py#L17) — Test converting empty parameters.
  - `test_convert_parameters_object(self)` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_modifiers.py#L30) — Test converting object parameters.
- uses (calls/refs, reference-scoped): [`_convert_parameters`](../../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#_convert_parameters)

### `TestAnalyzeCodeStructureToolGetFieldModifiers`
- def: [`tests/unit/mcp/test_analyze_code_structure_modifiers.py:99`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_modifiers.py#L99)
- doc: Tests for _get_field_modifiers helper.
- signature: `class TestAnalyzeCodeStructureToolGetFieldModifiers:`
- members:
  - `test_get_field_modifiers_multiple(self)` — [`L134`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_modifiers.py#L134) — Test getting multiple modifiers.
  - `test_get_field_modifiers_none(self)` — [`L102`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_modifiers.py#L102) — Test getting modifiers with no modifiers.
  - `test_get_field_modifiers_private(self)` — [`L113`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_modifiers.py#L113) — Test getting private visibility.
  - `test_get_field_modifiers_static(self)` — [`L123`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_modifiers.py#L123) — Test getting static modifier.
- uses (calls/refs, reference-scoped): [`_get_field_modifiers`](../../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#_get_field_modifiers)

### `TestAnalyzeCodeStructureToolGetMethodModifiers`
- def: [`tests/unit/mcp/test_analyze_code_structure_modifiers.py:42`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_modifiers.py#L42)
- doc: Tests for _get_method_modifiers helper.
- signature: `class TestAnalyzeCodeStructureToolGetMethodModifiers:`
- members:
  - `test_get_method_modifiers_abstract(self)` — [`L75`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_modifiers.py#L75) — Test getting abstract modifier.
  - `test_get_method_modifiers_final(self)` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_modifiers.py#L65) — Test getting final modifier.
  - `test_get_method_modifiers_multiple(self)` — [`L85`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_modifiers.py#L85) — Test getting multiple modifiers.
  - `test_get_method_modifiers_none(self)` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_modifiers.py#L45) — Test getting modifiers with no modifiers.
  - `test_get_method_modifiers_static(self)` — [`L55`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_modifiers.py#L55) — Test getting static modifier.
- uses (calls/refs, reference-scoped): [`_get_method_modifiers`](../../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#_get_method_modifiers)

### `TestAnalyzeCodeStructureToolGetMethodParameters`
- def: [`tests/unit/mcp/test_analyze_code_structure_modifiers.py:148`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_modifiers.py#L148)
- doc: Tests for _get_method_parameters helper.
- signature: `class TestAnalyzeCodeStructureToolGetMethodParameters:`
- members:
  - `test_get_method_parameters_empty(self)` — [`L151`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_modifiers.py#L151) — Test getting empty parameters.
  - `test_get_method_parameters_list_of_dicts(self)` — [`L171`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_modifiers.py#L171) — Test getting parameters as list of dicts.
  - `test_get_method_parameters_list_of_strings(self)` — [`L159`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_modifiers.py#L159) — Test getting parameters as list of strings.
  - `test_get_method_parameters_mixed(self)` — [`L181`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_modifiers.py#L181) — Test getting mixed parameters.
- uses (calls/refs, reference-scoped): [`_get_method_parameters`](../../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#_get_method_parameters)

