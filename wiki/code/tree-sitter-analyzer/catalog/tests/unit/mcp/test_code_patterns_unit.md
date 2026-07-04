---
title: 'Module: tests/unit/mcp/test_code_patterns_unit.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_code_patterns_unit.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_code_patterns_unit`/Test
symbols:
  TestCodePatternsToolSchema.test_get_tool_schema_returns_required_fields: CodePatternsToolSchema#test_get_tool_schema_returns_required_fields().
  TestCodePatternsToolSchema.test_get_tool_definition_has_name: CodePatternsToolSchema#test_get_tool_definition_has_name().
  TestCodePatternsToolSchema.test_validate_arguments_missing_file_path_raises: CodePatternsToolSchema#test_validate_arguments_missing_file_path_raises().
  TestCodePatternsToolSchema.test_validate_arguments_invalid_category_raises: CodePatternsToolSchema#test_validate_arguments_invalid_category_raises().
  TestCodePatternsToolSchema.test_validate_arguments_valid: CodePatternsToolSchema#test_validate_arguments_valid().
  TestCheckPythonAntiPatterns.test_mutable_default_list: CheckPythonAntiPatterns#test_mutable_default_list().
  TestCheckPythonAntiPatterns.test_bare_except: CheckPythonAntiPatterns#test_bare_except().
  TestCheckPythonAntiPatterns.test_print_in_function: CheckPythonAntiPatterns#test_print_in_function().
  TestCheckPythonAntiPatterns.test_clean_code_no_patterns: CheckPythonAntiPatterns#test_clean_code_no_patterns().
  TestCheckPythonAntiPatterns.test_print_at_module_level_ignored: CheckPythonAntiPatterns#test_print_at_module_level_ignored().
  TestCheckPythonAntiPatterns.test_print_in_multiline_docstring_ignored: CheckPythonAntiPatterns#test_print_in_multiline_docstring_ignored().
  TestCheckPythonAntiPatterns.test_print_in_single_line_docstring_ignored: CheckPythonAntiPatterns#test_print_in_single_line_docstring_ignored().
  TestCheckPythonAntiPatterns.test_print_outside_docstring_still_flagged: CheckPythonAntiPatterns#test_print_outside_docstring_still_flagged().
  TestCheckPythonAntiPatterns.test_bare_except_in_docstring_ignored: CheckPythonAntiPatterns#test_bare_except_in_docstring_ignored().
  TestCheckJsAntiPatterns.test_var_usage: CheckJsAntiPatterns#test_var_usage().
  TestCheckJsAntiPatterns.test_loose_equality: CheckJsAntiPatterns#test_loose_equality().
  TestCheckJsAntiPatterns.test_strict_equality_not_flagged: CheckJsAntiPatterns#test_strict_equality_not_flagged().
  TestCheckJsAntiPatterns.test_commented_var_ignored: CheckJsAntiPatterns#test_commented_var_ignored().
  TestCheckJavaAntiPatterns.test_system_out_println: CheckJavaAntiPatterns#test_system_out_println().
  TestCheckJavaAntiPatterns.test_print_stacktrace: CheckJavaAntiPatterns#test_print_stacktrace().
  TestCheckJavaAntiPatterns.test_commented_println_ignored: CheckJavaAntiPatterns#test_commented_println_ignored().
  TestDetectAntiPatterns.test_nonexistent_file_returns_empty: DetectAntiPatterns#test_nonexistent_file_returns_empty().
  TestDetectAntiPatterns.test_detects_python_patterns: DetectAntiPatterns#test_detects_python_patterns().
  TestDetectAntiPatterns.test_detects_js_patterns: DetectAntiPatterns#test_detects_js_patterns().
  TestDetectAntiPatterns.test_unsupported_language_returns_empty: DetectAntiPatterns#test_unsupported_language_returns_empty().
  TestDetectSmellsAndSecurity.test_detect_smells_nonexistent_file_returns_empty: DetectSmellsAndSecurity#test_detect_smells_nonexistent_file_returns_empty().
  TestDetectSmellsAndSecurity.test_detect_security_nonexistent_file_returns_empty: DetectSmellsAndSecurity#test_detect_security_nonexistent_file_returns_empty().
  TestDetectSmellsAndSecurity.test_detect_smells_valid_file: DetectSmellsAndSecurity#test_detect_smells_valid_file().
  TestBuildSummary.test_empty_patterns: BuildSummary#test_empty_patterns().
  TestBuildSummary.test_mixed_severity: BuildSummary#test_mixed_severity().
  TestBuildSummary.test_only_critical: BuildSummary#test_only_critical().
  TestSeverityOrder.test_info_is_lowest: SeverityOrder#test_info_is_lowest().
  TestSeverityOrder.test_warning_below_critical: SeverityOrder#test_warning_below_critical().
  TestSeverityOrder.test_three_levels: SeverityOrder#test_three_levels().
  TestAntiPatternLineNumbers.test_python_anti_patterns_have_line_numbers: AntiPatternLineNumbers#test_python_anti_patterns_have_line_numbers().
  TestAntiPatternLineNumbers.test_js_anti_patterns_have_line_numbers: AntiPatternLineNumbers#test_js_anti_patterns_have_line_numbers().
  TestAntiPatternLineNumbers.test_java_anti_patterns_have_line_numbers: AntiPatternLineNumbers#test_java_anti_patterns_have_line_numbers().
  TestAntiPatternIds.test_python_anti_patterns_have_ids: AntiPatternIds#test_python_anti_patterns_have_ids().
  TestAntiPatternIds.test_js_anti_patterns_have_ids: AntiPatternIds#test_js_anti_patterns_have_ids().
  TestAntiPatternIds.test_java_anti_patterns_have_ids: AntiPatternIds#test_java_anti_patterns_have_ids().
  TestDetectAntiPatternsTypescript.test_typescript_uses_js_patterns: DetectAntiPatternsTypescript#test_typescript_uses_js_patterns().
  TestDetectSecurityWithRealFile.test_detect_security_returns_list_for_valid_file: DetectSecurityWithRealFile#test_detect_security_returns_list_for_valid_file().
  TestDetectSecurityWithRealFile.test_detect_security_handles_unreadable_gracefully: DetectSecurityWithRealFile#test_detect_security_handles_unreadable_gracefully().
  TestCodePatternsToolSchema: CodePatternsToolSchema#
  TestCheckPythonAntiPatterns: CheckPythonAntiPatterns#
  TestCheckJsAntiPatterns: CheckJsAntiPatterns#
  TestCheckJavaAntiPatterns: CheckJavaAntiPatterns#
  TestDetectAntiPatterns: DetectAntiPatterns#
  TestDetectSmellsAndSecurity: DetectSmellsAndSecurity#
  TestBuildSummary: BuildSummary#
  TestSeverityOrder: SeverityOrder#
  TestAntiPatternLineNumbers: AntiPatternLineNumbers#
  TestAntiPatternIds: AntiPatternIds#
  TestDetectAntiPatternsTypescript: DetectAntiPatternsTypescript#
  TestDetectSecurityWithRealFile: DetectSecurityWithRealFile#
---
# Module: [`tests/unit/mcp/test_code_patterns_unit.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_unit.py)

## Classes
### `TestAntiPatternIds`
- def: [`tests/unit/mcp/test_code_patterns_unit.py:348`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_unit.py#L348)
- signature: `class TestAntiPatternIds:`
- members:
  - `test_java_anti_patterns_have_ids(self)` — [`L381`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_unit.py#L381)
  - `test_js_anti_patterns_have_ids(self)` — [`L373`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_unit.py#L373)
  - `test_python_anti_patterns_have_ids(self)` — [`L349`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_unit.py#L349)
- uses (calls/refs, reference-scoped): [`_check_python_anti_patterns`](../../../tree_sitter_analyzer/mcp/tools/utils/anti_patterns.md#_check_python_anti_patterns), [`_check_js_anti_patterns`](../../../tree_sitter_analyzer/mcp/tools/utils/anti_patterns.md#_check_js_anti_patterns), [`_check_java_anti_patterns`](../../../tree_sitter_analyzer/mcp/tools/utils/anti_patterns.md#_check_java_anti_patterns)

### `TestAntiPatternLineNumbers`
- def: [`tests/unit/mcp/test_code_patterns_unit.py:312`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_unit.py#L312)
- signature: `class TestAntiPatternLineNumbers:`
- members:
  - `test_java_anti_patterns_have_line_numbers(self)` — [`L335`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_unit.py#L335)
  - `test_js_anti_patterns_have_line_numbers(self)` — [`L328`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_unit.py#L328)
  - `test_python_anti_patterns_have_line_numbers(self)` — [`L313`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_unit.py#L313)
- uses (calls/refs, reference-scoped): [`_check_python_anti_patterns`](../../../tree_sitter_analyzer/mcp/tools/utils/anti_patterns.md#_check_python_anti_patterns), [`_check_js_anti_patterns`](../../../tree_sitter_analyzer/mcp/tools/utils/anti_patterns.md#_check_js_anti_patterns), [`_check_java_anti_patterns`](../../../tree_sitter_analyzer/mcp/tools/utils/anti_patterns.md#_check_java_anti_patterns)

### `TestBuildSummary`
- def: [`tests/unit/mcp/test_code_patterns_unit.py:268`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_unit.py#L268)
- signature: `class TestBuildSummary:`
- members:
  - `test_empty_patterns(self)` — [`L269`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_unit.py#L269)
  - `test_mixed_severity(self)` — [`L272`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_unit.py#L272)
  - `test_only_critical(self)` — [`L285`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_unit.py#L285)
- uses (calls/refs, reference-scoped): [`_build_summary`](../../../tree_sitter_analyzer/mcp/tools/code_patterns_tool.md#_build_summary)

### `TestCheckJavaAntiPatterns`
- def: [`tests/unit/mcp/test_code_patterns_unit.py:193`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_unit.py#L193)
- signature: `class TestCheckJavaAntiPatterns:`
- members:
  - `test_commented_println_ignored(self)` — [`L206`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_unit.py#L206)
  - `test_print_stacktrace(self)` — [`L200`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_unit.py#L200)
  - `test_system_out_println(self)` — [`L194`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_unit.py#L194)
- uses (calls/refs, reference-scoped): [`_check_java_anti_patterns`](../../../tree_sitter_analyzer/mcp/tools/utils/anti_patterns.md#_check_java_anti_patterns)

### `TestCheckJsAntiPatterns`
- def: [`tests/unit/mcp/test_code_patterns_unit.py:162`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_unit.py#L162)
- signature: `class TestCheckJsAntiPatterns:`
- members:
  - `test_commented_var_ignored(self)` — [`L181`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_unit.py#L181)
  - `test_loose_equality(self)` — [`L169`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_unit.py#L169)
  - `test_strict_equality_not_flagged(self)` — [`L175`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_unit.py#L175)
  - `test_var_usage(self)` — [`L163`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_unit.py#L163)
- uses (calls/refs, reference-scoped): [`_check_js_anti_patterns`](../../../tree_sitter_analyzer/mcp/tools/utils/anti_patterns.md#_check_js_anti_patterns)

### `TestCheckPythonAntiPatterns`
- def: [`tests/unit/mcp/test_code_patterns_unit.py:59`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_unit.py#L59)
- signature: `class TestCheckPythonAntiPatterns:`
- members:
  - `test_bare_except(self)` — [`L69`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_unit.py#L69)
  - `test_bare_except_in_docstring_ignored(self)` — [`L140`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_unit.py#L140)
  - `test_clean_code_no_patterns(self)` — [`L84`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_unit.py#L84)
  - `test_mutable_default_list(self)` — [`L60`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_unit.py#L60)
  - `test_print_at_module_level_ignored(self)` — [`L95`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_unit.py#L95)
  - `test_print_in_function(self)` — [`L75`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_unit.py#L75)
  - `test_print_in_multiline_docstring_ignored(self)` — [`L101`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_unit.py#L101) — Dogfood regression: --code-patterns previously flagged docstring
  - `test_print_in_single_line_docstring_ignored(self)` — [`L119`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_unit.py#L119)
  - `test_print_outside_docstring_still_flagged(self)` — [`L129`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_unit.py#L129) — Don't over-correct: real print() in a function body must still flag.
- uses (calls/refs, reference-scoped): [`_check_python_anti_patterns`](../../../tree_sitter_analyzer/mcp/tools/utils/anti_patterns.md#_check_python_anti_patterns)

### `TestCodePatternsToolSchema`
- def: [`tests/unit/mcp/test_code_patterns_unit.py:24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_unit.py#L24)
- signature: `class TestCodePatternsToolSchema:`
- members:
  - `test_get_tool_definition_has_name(self)` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_unit.py#L32)
  - `test_get_tool_schema_returns_required_fields(self)` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_unit.py#L25)
  - `test_validate_arguments_invalid_category_raises(self)` — [`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_unit.py#L41)
  - `test_validate_arguments_missing_file_path_raises(self)` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_unit.py#L37)
  - `test_validate_arguments_valid(self)` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_unit.py#L47)
- uses (calls/refs, reference-scoped): [`CodePatternsTool`](../../../tree_sitter_analyzer/mcp/tools/code_patterns_tool.md#CodePatternsTool), [`get_tool_schema`](../../../tree_sitter_analyzer/mcp/tools/code_patterns_tool.md#CodePatternsTool.get_tool_schema), [`validate_arguments`](../../../tree_sitter_analyzer/mcp/tools/code_patterns_tool.md#CodePatternsTool.validate_arguments), [`get_tool_definition`](../../../tree_sitter_analyzer/mcp/tools/code_patterns_tool.md#CodePatternsTool.get_tool_definition)

### `TestDetectAntiPatterns`
- def: [`tests/unit/mcp/test_code_patterns_unit.py:218`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_unit.py#L218)
- signature: `class TestDetectAntiPatterns:`
- members:
  - `test_detects_js_patterns(self, tmp_path)` — [`L229`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_unit.py#L229)
  - `test_detects_python_patterns(self, tmp_path)` — [`L223`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_unit.py#L223)
  - `test_nonexistent_file_returns_empty(self, tmp_path)` — [`L219`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_unit.py#L219)
  - `test_unsupported_language_returns_empty(self, tmp_path)` — [`L235`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_unit.py#L235)
- uses (calls/refs, reference-scoped): [`_detect_anti_patterns`](../../../tree_sitter_analyzer/mcp/tools/code_patterns_tool.md#_detect_anti_patterns)

### `TestDetectAntiPatternsTypescript`
- def: [`tests/unit/mcp/test_code_patterns_unit.py:395`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_unit.py#L395)
- signature: `class TestDetectAntiPatternsTypescript:`
- members:
  - `test_typescript_uses_js_patterns(self, tmp_path)` — [`L396`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_unit.py#L396)
- uses (calls/refs, reference-scoped): [`_detect_anti_patterns`](../../../tree_sitter_analyzer/mcp/tools/code_patterns_tool.md#_detect_anti_patterns)

### `TestDetectSecurityWithRealFile`
- def: [`tests/unit/mcp/test_code_patterns_unit.py:409`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_unit.py#L409)
- signature: `class TestDetectSecurityWithRealFile:`
- members:
  - `test_detect_security_handles_unreadable_gracefully(self)` — [`L416`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_unit.py#L416)
  - `test_detect_security_returns_list_for_valid_file(self, tmp_path)` — [`L410`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_unit.py#L410)
- uses (calls/refs, reference-scoped): [`_detect_security`](../../../tree_sitter_analyzer/mcp/tools/code_patterns_tool.md#_detect_security)

### `TestDetectSmellsAndSecurity`
- def: [`tests/unit/mcp/test_code_patterns_unit.py:247`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_unit.py#L247)
- signature: `class TestDetectSmellsAndSecurity:`
- members:
  - `test_detect_security_nonexistent_file_returns_empty(self)` — [`L252`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_unit.py#L252)
  - `test_detect_smells_nonexistent_file_returns_empty(self)` — [`L248`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_unit.py#L248)
  - `test_detect_smells_valid_file(self, tmp_path)` — [`L256`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_unit.py#L256)
- uses (calls/refs, reference-scoped): [`_detect_smells`](../../../tree_sitter_analyzer/mcp/tools/code_patterns_tool.md#_detect_smells), [`_detect_security`](../../../tree_sitter_analyzer/mcp/tools/code_patterns_tool.md#_detect_security)

### `TestSeverityOrder`
- def: [`tests/unit/mcp/test_code_patterns_unit.py:296`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_unit.py#L296)
- signature: `class TestSeverityOrder:`
- members:
  - `test_info_is_lowest(self)` — [`L297`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_unit.py#L297)
  - `test_three_levels(self)` — [`L303`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_unit.py#L303)
  - `test_warning_below_critical(self)` — [`L300`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_unit.py#L300)
- uses (calls/refs, reference-scoped): [`_SEVERITY_ORDER`](../../../tree_sitter_analyzer/mcp/tools/code_patterns_tool.md#_SEVERITY_ORDER)

