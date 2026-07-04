---
title: 'Module: tests/unit/mcp/test_code_patterns_execute.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_code_patterns_execute.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_code_patterns_execute`/
symbols:
  _make_python_with_anti_patterns: _make_python_with_anti_patterns().
  TestExecuteSeverityFiltering.test_patterns_sorted_by_severity_desc: TestExecuteSeverityFiltering#test_patterns_sorted_by_severity_desc().
  TestExecuteAntiPatterns.test_execute_detects_python_anti_patterns: TestExecuteAntiPatterns#test_execute_detects_python_anti_patterns().
  TestExecuteAntiPatterns.test_execute_detects_js_anti_patterns: TestExecuteAntiPatterns#test_execute_detects_js_anti_patterns().
  TestExecuteAntiPatterns.test_execute_detects_java_anti_patterns: TestExecuteAntiPatterns#test_execute_detects_java_anti_patterns().
  TestExecuteAntiPatterns.test_execute_clean_file_no_anti_patterns: TestExecuteAntiPatterns#test_execute_clean_file_no_anti_patterns().
  TestExecuteCategoryFiltering.test_category_smells_only: TestExecuteCategoryFiltering#test_category_smells_only().
  TestExecuteCategoryFiltering.test_category_security_only: TestExecuteCategoryFiltering#test_category_security_only().
  TestExecuteCategoryFiltering.test_category_all_includes_everything: TestExecuteCategoryFiltering#test_category_all_includes_everything().
  TestExecuteCategoryFiltering.test_default_categories_is_all: TestExecuteCategoryFiltering#test_default_categories_is_all().
  TestExecuteCategoryFiltering.test_multiple_categories: TestExecuteCategoryFiltering#test_multiple_categories().
  TestExecuteSeverityFiltering.test_severity_threshold_critical: TestExecuteSeverityFiltering#test_severity_threshold_critical().
  TestExecuteSeverityFiltering.test_severity_threshold_warning: TestExecuteSeverityFiltering#test_severity_threshold_warning().
  TestExecuteSeverityFiltering.test_severity_threshold_info_includes_all: TestExecuteSeverityFiltering#test_severity_threshold_info_includes_all().
  TestExecuteSeverityFiltering.test_default_severity_is_info: TestExecuteSeverityFiltering#test_default_severity_is_info().
  TestExecuteResponseStructure.test_response_has_required_fields: TestExecuteResponseStructure#test_response_has_required_fields().
  TestExecuteResponseStructure.test_language_detected: TestExecuteResponseStructure#test_language_detected().
  TestExecuteResponseStructure.test_by_category_counts: TestExecuteResponseStructure#test_by_category_counts().
  TestExecuteResponseStructure.test_patterns_capped_at_50: TestExecuteResponseStructure#test_patterns_capped_at_50().
  TestExecuteResponseStructure.test_each_pattern_has_required_keys: TestExecuteResponseStructure#test_each_pattern_has_required_keys().
  TestExecuteWorkflowHint.test_hint_mentions_critical_when_present: TestExecuteWorkflowHint#test_hint_mentions_critical_when_present().
  TestExecuteWorkflowHint.test_hint_mentions_refactoring_suggestions: TestExecuteWorkflowHint#test_hint_mentions_refactoring_suggestions().
  TestExecuteWorkflowHint.test_hint_warns_when_no_critical: TestExecuteWorkflowHint#test_hint_warns_when_no_critical().
  TestExecuteEdgeCases.test_toon_format_requested: TestExecuteEdgeCases#test_toon_format_requested().
  TestExecuteEdgeCases.test_json_format_requested: TestExecuteEdgeCases#test_json_format_requested().
  TestExecuteEdgeCases.test_nonexistent_file_raises: TestExecuteEdgeCases#test_nonexistent_file_raises().
  TestExecuteEdgeCases.test_directory_path_raises: TestExecuteEdgeCases#test_directory_path_raises().
  TestExecuteEdgeCases.test_typescript_uses_js_detector: TestExecuteEdgeCases#test_typescript_uses_js_detector().
  _make_clean_python: _make_clean_python().
  _make_js_with_anti_patterns: _make_js_with_anti_patterns().
  _make_java_with_anti_patterns: _make_java_with_anti_patterns().
  TestExecuteAntiPatterns: TestExecuteAntiPatterns#
  TestExecuteCategoryFiltering: TestExecuteCategoryFiltering#
  TestExecuteSeverityFiltering: TestExecuteSeverityFiltering#
  TestExecuteResponseStructure: TestExecuteResponseStructure#
  TestExecuteWorkflowHint: TestExecuteWorkflowHint#
  TestExecuteEdgeCases: TestExecuteEdgeCases#
---
# Module: [`tests/unit/mcp/test_code_patterns_execute.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_execute.py)

## Classes
### `TestExecuteAntiPatterns`
- def: [`tests/unit/mcp/test_code_patterns_execute.py:63`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_execute.py#L63)
- signature: `class TestExecuteAntiPatterns:`
- members:
  - `test_execute_clean_file_no_anti_patterns(self, tmp_path)` — [`L103`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_execute.py#L103)
  - `test_execute_detects_java_anti_patterns(self, tmp_path)` — [`L91`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_execute.py#L91)
  - `test_execute_detects_js_anti_patterns(self, tmp_path)` — [`L79`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_execute.py#L79)
  - `test_execute_detects_python_anti_patterns(self, tmp_path)` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_execute.py#L65)
- uses (calls/refs, reference-scoped): [`execute`](../../../tree_sitter_analyzer/mcp/tools/code_patterns_tool.md#CodePatternsTool.execute), [`CodePatternsTool`](../../../tree_sitter_analyzer/mcp/tools/code_patterns_tool.md#CodePatternsTool)  (4 test-only)

### `TestExecuteCategoryFiltering`
- def: [`tests/unit/mcp/test_code_patterns_execute.py:116`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_execute.py#L116)
- signature: `class TestExecuteCategoryFiltering:`
- members:
  - `test_category_all_includes_everything(self, tmp_path)` — [`L140`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_execute.py#L140)
  - `test_category_security_only(self, tmp_path)` — [`L129`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_execute.py#L129)
  - `test_category_smells_only(self, tmp_path)` — [`L118`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_execute.py#L118)
  - `test_default_categories_is_all(self, tmp_path)` — [`L151`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_execute.py#L151)
  - `test_multiple_categories(self, tmp_path)` — [`L158`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_execute.py#L158)
- uses (calls/refs, reference-scoped): [`execute`](../../../tree_sitter_analyzer/mcp/tools/code_patterns_tool.md#CodePatternsTool.execute), [`CodePatternsTool`](../../../tree_sitter_analyzer/mcp/tools/code_patterns_tool.md#CodePatternsTool)  (1 test-only)

### `TestExecuteEdgeCases`
- def: [`tests/unit/mcp/test_code_patterns_execute.py:351`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_execute.py#L351)
- signature: `class TestExecuteEdgeCases:`
- members:
  - `test_directory_path_raises(self, tmp_path)` — [`L359`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_execute.py#L359)
  - `test_json_format_requested(self, tmp_path)` — [`L374`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_execute.py#L374)
  - `test_nonexistent_file_raises(self, tmp_path)` — [`L353`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_execute.py#L353)
  - `test_toon_format_requested(self, tmp_path)` — [`L365`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_execute.py#L365)
  - `test_typescript_uses_js_detector(self, tmp_path)` — [`L383`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_execute.py#L383)
- uses (calls/refs, reference-scoped): [`execute`](../../../tree_sitter_analyzer/mcp/tools/code_patterns_tool.md#CodePatternsTool.execute), [`CodePatternsTool`](../../../tree_sitter_analyzer/mcp/tools/code_patterns_tool.md#CodePatternsTool)  (1 test-only)

### `TestExecuteResponseStructure`
- def: [`tests/unit/mcp/test_code_patterns_execute.py:252`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_execute.py#L252)
- signature: `class TestExecuteResponseStructure:`
- members:
  - `test_by_category_counts(self, tmp_path)` — [`L280`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_execute.py#L280)
  - `test_each_pattern_has_required_keys(self, tmp_path)` — [`L298`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_execute.py#L298)
  - `test_language_detected(self, tmp_path)` — [`L273`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_execute.py#L273)
  - `test_patterns_capped_at_50(self, tmp_path)` — [`L291`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_execute.py#L291)
  - `test_response_has_required_fields(self, tmp_path)` — [`L254`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_execute.py#L254)
- uses (calls/refs, reference-scoped): [`execute`](../../../tree_sitter_analyzer/mcp/tools/code_patterns_tool.md#CodePatternsTool.execute), [`CodePatternsTool`](../../../tree_sitter_analyzer/mcp/tools/code_patterns_tool.md#CodePatternsTool)  (1 test-only)

### `TestExecuteSeverityFiltering`
- def: [`tests/unit/mcp/test_code_patterns_execute.py:178`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_execute.py#L178)
- signature: `class TestExecuteSeverityFiltering:`
- members:
  - `test_default_severity_is_info(self, tmp_path)` — [`L228`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_execute.py#L228)
  - `test_patterns_sorted_by_severity_desc(self, tmp_path)` — [`L236`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_execute.py#L236)
  - `test_severity_threshold_critical(self, tmp_path)` — [`L180`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_execute.py#L180)
  - `test_severity_threshold_info_includes_all(self, tmp_path)` — [`L212`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_execute.py#L212)
  - `test_severity_threshold_warning(self, tmp_path)` — [`L196`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_execute.py#L196)
- uses (calls/refs, reference-scoped): [`execute`](../../../tree_sitter_analyzer/mcp/tools/code_patterns_tool.md#CodePatternsTool.execute), [`CodePatternsTool`](../../../tree_sitter_analyzer/mcp/tools/code_patterns_tool.md#CodePatternsTool), [`_SEVERITY_ORDER`](../../../tree_sitter_analyzer/mcp/tools/code_patterns_tool.md#_SEVERITY_ORDER)  (1 test-only)

### `TestExecuteWorkflowHint`
- def: [`tests/unit/mcp/test_code_patterns_execute.py:317`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_execute.py#L317)
- signature: `class TestExecuteWorkflowHint:`
- members:
  - `test_hint_mentions_critical_when_present(self, tmp_path)` — [`L319`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_execute.py#L319)
  - `test_hint_mentions_refactoring_suggestions(self, tmp_path)` — [`L331`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_execute.py#L331)
  - `test_hint_warns_when_no_critical(self, tmp_path)` — [`L338`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_execute.py#L338)
- uses (calls/refs, reference-scoped): [`execute`](../../../tree_sitter_analyzer/mcp/tools/code_patterns_tool.md#CodePatternsTool.execute), [`CodePatternsTool`](../../../tree_sitter_analyzer/mcp/tools/code_patterns_tool.md#CodePatternsTool)  (2 test-only)

## Functions
- `_make_clean_python(tmp_path)` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_execute.py#L26)
- `_make_java_with_anti_patterns(tmp_path)` — [`L44`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_execute.py#L44)
- `_make_js_with_anti_patterns(tmp_path)` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_execute.py#L35)
- `_make_python_with_anti_patterns(tmp_path)` — [`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_execute.py#L17)

