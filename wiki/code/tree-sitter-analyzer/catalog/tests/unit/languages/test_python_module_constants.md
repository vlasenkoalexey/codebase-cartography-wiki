---
title: 'Module: tests/unit/languages/test_python_module_constants.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_python_module_constants.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_python_module_constants`/
symbols:
  _variables: _variables().
  TestPluginModuleConstants.test_constant_extraction_failure_degrades_to_class_attrs: TestPluginModuleConstants#test_constant_extraction_failure_degrades_to_class_attrs().
  TestPluginModuleConstants.test_chained_assignment_captures_both_names: TestPluginModuleConstants#test_chained_assignment_captures_both_names().
  TestPluginModuleConstants.test_single_line_semicolon_assignments_capture_every_constant: TestPluginModuleConstants#test_single_line_semicolon_assignments_capture_every_constant().
  TestStructureSurfaceSeesModuleConstants.test_analyze_fields_contain_module_constants: TestStructureSurfaceSeesModuleConstants#test_analyze_fields_contain_module_constants().
  TestStructureSurfaceSeesModuleConstants.test_analyze_fields_exclude_locals_and_mutables: TestStructureSurfaceSeesModuleConstants#test_analyze_fields_exclude_locals_and_mutables().
  TestStructureSurfaceSeesModuleConstants.test_outline_field_count_includes_module_constants: TestStructureSurfaceSeesModuleConstants#test_outline_field_count_includes_module_constants().
  _SRC: _SRC.
  TestPluginModuleConstants.test_exactly_the_five_module_constants_extracted: TestPluginModuleConstants#test_exactly_the_five_module_constants_extracted().
  TestOutlineTopLevelFields.test_outline_surfaces_module_constants: TestOutlineTopLevelFields#test_outline_surfaces_module_constants().
  TestPluginModuleConstants.test_total_variable_count_is_six: TestPluginModuleConstants#test_total_variable_count_is_six().
  TestPluginModuleConstants.test_class_attribute_unchanged: TestPluginModuleConstants#test_class_attribute_unchanged().
  TestPluginModuleConstants.test_function_local_not_extracted: TestPluginModuleConstants#test_function_local_not_extracted().
  TestPluginModuleConstants.test_lowercase_unannotated_not_extracted: TestPluginModuleConstants#test_lowercase_unannotated_not_extracted().
  TestPluginModuleConstants.test_bare_annotation_not_extracted: TestPluginModuleConstants#test_bare_annotation_not_extracted().
  TestPluginModuleConstants.test_constant_lines_pinned: TestPluginModuleConstants#test_constant_lines_pinned().
  TestPluginModuleConstants.test_constant_types_and_visibility: TestPluginModuleConstants#test_constant_types_and_visibility().
  TestPluginModuleConstants.test_variables_sorted_by_line: TestPluginModuleConstants#test_variables_sorted_by_line().
  TestPluginModuleConstants.test_none_tree_yields_no_constants: TestPluginModuleConstants#test_none_tree_yields_no_constants().
  _MODULE_CONSTANT_NAMES: _MODULE_CONSTANT_NAMES.
  TestPluginModuleConstants._boom: TestPluginModuleConstants#_boom().
  TestPluginModuleConstants: TestPluginModuleConstants#
  TestStructureSurfaceSeesModuleConstants: TestStructureSurfaceSeesModuleConstants#
  TestOutlineTopLevelFields: TestOutlineTopLevelFields#
---
# Module: [`tests/unit/languages/test_python_module_constants.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_module_constants.py)

## Classes
### `TestOutlineTopLevelFields`
- def: [`tests/unit/languages/test_python_module_constants.py:218`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_module_constants.py#L218)
- doc: Codex P2 on #645: field_count included module constants but no
- signature: `class TestOutlineTopLevelFields:`
- members:
  - `test_outline_surfaces_module_constants(self, tmp_path)` — [`L222`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_module_constants.py#L222)
- uses (calls/refs, reference-scoped): [`GetCodeOutlineTool`](../../../tree_sitter_analyzer/mcp/tools/get_code_outline_tool.md#GetCodeOutlineTool), [`execute`](../../../tree_sitter_analyzer/mcp/tools/get_code_outline_tool.md#GetCodeOutlineTool.execute)

### `TestPluginModuleConstants`
- def: [`tests/unit/languages/test_python_module_constants.py:70`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_module_constants.py#L70)
- doc: Plugin path: extract_variables emits module constants (#612 parity).
- signature: `class TestPluginModuleConstants:`
- members:
  - `test_bare_annotation_not_extracted(self)` — [`L95`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_module_constants.py#L95)
  - `test_chained_assignment_captures_both_names(self)` — [`L123`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_module_constants.py#L123)
  - `test_class_attribute_unchanged(self)` — [`L81`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_module_constants.py#L81)
  - `test_constant_extraction_failure_degrades_to_class_attrs(self, monkeypatch)` — [`L145`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_module_constants.py#L145)
  - `test_constant_lines_pinned(self)` — [`L99`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_module_constants.py#L99)
  - `test_constant_types_and_visibility(self)` — [`L110`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_module_constants.py#L110)
  - `test_exactly_the_five_module_constants_extracted(self)` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_module_constants.py#L73)
  - `test_function_local_not_extracted(self)` — [`L87`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_module_constants.py#L87)
  - `test_lowercase_unannotated_not_extracted(self)` — [`L91`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_module_constants.py#L91)
  - `test_none_tree_yields_no_constants(self)` — [`L142`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_module_constants.py#L142)
  - `test_single_line_semicolon_assignments_capture_every_constant(self)` — [`L133`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_module_constants.py#L133)
  - `test_total_variable_count_is_six(self)` — [`L77`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_module_constants.py#L77)
  - `test_variables_sorted_by_line(self)` — [`L119`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_module_constants.py#L119)
- protocol/private: `_boom`[`L150`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_module_constants.py#L150)
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`Parser`](../../../tree_sitter_analyzer/core/parser.md#Parser), [`tree`](../../../tree_sitter_analyzer/core/parser.md#ParseResult.tree), [`parse_code`](../../../tree_sitter_analyzer/core/parser.md#Parser.parse_code), [`PythonElementExtractor`](../../../tree_sitter_analyzer/languages/python_plugin/extractor.md#PythonElementExtractor), [`extract_variables`](../../../tree_sitter_analyzer/languages/python_plugin/_class_extractor_mixin.md#PythonClassExtractionMixin.extract_variables), [`extract_module_constants`](../../../tree_sitter_analyzer/languages/python_plugin/_element_builders.md#extract_module_constants)  (3 test-only)

### `TestStructureSurfaceSeesModuleConstants`
- def: [`tests/unit/languages/test_python_module_constants.py:162`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_module_constants.py#L162)
- doc: structure action=analyze / outline expose the constants as fields.
- signature: `class TestStructureSurfaceSeesModuleConstants:`
- members:
  - `test_analyze_fields_contain_module_constants(self, tmp_path)` — [`L166`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_module_constants.py#L166)
  - `test_analyze_fields_exclude_locals_and_mutables(self, tmp_path)` — [`L183`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_module_constants.py#L183)
  - `test_outline_field_count_includes_module_constants(self, tmp_path)` — [`L200`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_module_constants.py#L200)
- uses (calls/refs, reference-scoped): [`AnalyzeCodeStructureTool`](../../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#AnalyzeCodeStructureTool), [`GetCodeOutlineTool`](../../../tree_sitter_analyzer/mcp/tools/get_code_outline_tool.md#GetCodeOutlineTool), [`execute`](../../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#AnalyzeCodeStructureTool.execute), [`execute`](../../../tree_sitter_analyzer/mcp/tools/get_code_outline_tool.md#GetCodeOutlineTool.execute)  (2 test-only)

## Functions
- `_variables()` — [`L64`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_module_constants.py#L64)

## Module values
- `_MODULE_CONSTANT_NAMES` — [`L55`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_module_constants.py#L55)
- `_SRC` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_module_constants.py#L35)

