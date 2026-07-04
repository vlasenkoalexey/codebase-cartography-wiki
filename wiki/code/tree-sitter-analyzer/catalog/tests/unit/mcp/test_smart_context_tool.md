---
title: 'Module: tests/unit/mcp/test_smart_context_tool.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_smart_context_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_smart_context_tool`/
symbols:
  TestAgentSummary.test_recommends_safe_to_edit_for_dangerous_files: TestAgentSummary#test_recommends_safe_to_edit_for_dangerous_files().
  TestAgentSummary.test_recommends_refactor_for_low_grade_files: TestAgentSummary#test_recommends_refactor_for_low_grade_files().
  _run: _run().
  TARGET_FILE: TARGET_FILE.
  tool: tool().
  TestExportExtraction.test_extracts_class: TestExportExtraction#test_extracts_class().
  TestExportExtraction.test_excludes_private_functions: TestExportExtraction#test_excludes_private_functions().
  TestStructureExtraction.test_extracts_structure: TestStructureExtraction#test_extracts_structure().
  TestSmartContextTool.test_execute_returns_complete_profile: TestSmartContextTool#test_execute_returns_complete_profile().
  TestSmartContextTool.test_agent_summary_guides_next_action: TestSmartContextTool#test_agent_summary_guides_next_action().
  TestSmartContextTool.test_health_has_grade_and_score: TestSmartContextTool#test_health_has_grade_and_score().
  TestSmartContextTool.test_exports_include_classes_and_functions: TestSmartContextTool#test_exports_include_classes_and_functions().
  TestSmartContextTool.test_structure_has_line_ranges: TestSmartContextTool#test_structure_has_line_ranges().
  TestSmartContextTool.test_dependencies_structure: TestSmartContextTool#test_dependencies_structure().
  TestSmartContextTool.test_edit_risk_is_valid: TestSmartContextTool#test_edit_risk_is_valid().
  TestSmartContextTool.test_line_count: TestSmartContextTool#test_line_count().
  TestSmartContextTool.test_language_detected: TestSmartContextTool#test_language_detected().
  TestSmartContextTool.test_toon_format_works: TestSmartContextTool#test_toon_format_works().
  TestSmartContextTool.test_json_format_works: TestSmartContextTool#test_json_format_works().
  PROJECT_ROOT: PROJECT_ROOT.
  TestSmartContextTool.test_file_not_found: TestSmartContextTool#test_file_not_found().
  TestSmartContextSyntaxGate.test_parse_broken_file_is_error_not_safe: TestSmartContextSyntaxGate#test_parse_broken_file_is_error_not_safe().
  TestSmartContextSyntaxGate.test_clean_file_is_not_gated: TestSmartContextSyntaxGate#test_clean_file_is_not_gated().
  TestQuickRisk.test_safe: TestQuickRisk#test_safe().
  TestQuickRisk.test_caution: TestQuickRisk#test_caution().
  TestQuickRisk.test_dangerous: TestQuickRisk#test_dangerous().
  TestSmartContextTool: TestSmartContextTool#
  TestSmartContextTool.test_validate_arguments_missing_path: TestSmartContextTool#test_validate_arguments_missing_path().
  TestSmartContextTool.test_validate_arguments_valid: TestSmartContextTool#test_validate_arguments_valid().
  TestSmartContextSyntaxGate: TestSmartContextSyntaxGate#
  TestExportExtraction: TestExportExtraction#
  TestStructureExtraction: TestStructureExtraction#
  TestQuickRisk: TestQuickRisk#
  TestAgentSummary: TestAgentSummary#
---
# Module: [`tests/unit/mcp/test_smart_context_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_smart_context_tool.py)

## Classes
### `TestAgentSummary`
- def: [`tests/unit/mcp/test_smart_context_tool.py:228`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_smart_context_tool.py#L228)
- signature: `class TestAgentSummary:`
- members:
  - `test_recommends_refactor_for_low_grade_files(self)` — [`L247`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_smart_context_tool.py#L247)
  - `test_recommends_safe_to_edit_for_dangerous_files(self)` — [`L229`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_smart_context_tool.py#L229)
- uses (calls/refs, reference-scoped): [`_build_agent_summary`](../../../tree_sitter_analyzer/mcp/tools/smart_context_tool.md#_build_agent_summary), [`risk`](../../../tree_sitter_analyzer/mcp/tools/smart_context_tool.md#AgentSummaryInput.risk), [`file_path`](../../../tree_sitter_analyzer/mcp/tools/smart_context_tool.md#AgentSummaryInput.file_path), [`grade`](../../../tree_sitter_analyzer/mcp/tools/smart_context_tool.md#AgentSummaryInput.grade), [`test_files`](../../../tree_sitter_analyzer/mcp/tools/smart_context_tool.md#AgentSummaryInput.test_files), [`AgentSummaryInput`](../../../tree_sitter_analyzer/mcp/tools/smart_context_tool.md#AgentSummaryInput), [`downstream_count`](../../../tree_sitter_analyzer/mcp/tools/smart_context_tool.md#AgentSummaryInput.downstream_count), [`export_count`](../../../tree_sitter_analyzer/mcp/tools/smart_context_tool.md#AgentSummaryInput.export_count), [`score`](../../../tree_sitter_analyzer/mcp/tools/smart_context_tool.md#AgentSummaryInput.score), [`weakest`](../../../tree_sitter_analyzer/mcp/tools/smart_context_tool.md#AgentSummaryInput.weakest)

### `TestExportExtraction`
- def: [`tests/unit/mcp/test_smart_context_tool.py:183`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_smart_context_tool.py#L183)
- signature: `class TestExportExtraction:`
- members:
  - `test_excludes_private_functions(self)` — [`L195`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_smart_context_tool.py#L195)
  - `test_extracts_class(self)` — [`L184`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_smart_context_tool.py#L184)
- uses (calls/refs, reference-scoped): [`extract_elements`](../../../tree_sitter_analyzer/mcp/tools/utils/element_extractor.md#extract_elements), [`get_all_exports`](../../../tree_sitter_analyzer/mcp/tools/utils/element_extractor.md#get_all_exports)  (1 test-only)

### `TestQuickRisk`
- def: [`tests/unit/mcp/test_smart_context_tool.py:217`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_smart_context_tool.py#L217)
- signature: `class TestQuickRisk:`
- members:
  - `test_caution(self)` — [`L221`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_smart_context_tool.py#L221)
  - `test_dangerous(self)` — [`L224`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_smart_context_tool.py#L224)
  - `test_safe(self)` — [`L218`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_smart_context_tool.py#L218)
- uses (calls/refs, reference-scoped): [`_quick_risk`](../../../tree_sitter_analyzer/mcp/tools/smart_context_tool.md#_quick_risk)

### `TestSmartContextSyntaxGate`
- def: [`tests/unit/mcp/test_smart_context_tool.py:152`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_smart_context_tool.py#L152)
- doc: #754: smart_context blended file_health + risk but bypassed the shared
- signature: `class TestSmartContextSyntaxGate:`
- members:
  - `test_clean_file_is_not_gated(self, tool, tmp_path)` — [`L174`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_smart_context_tool.py#L174)
  - `test_parse_broken_file_is_error_not_safe(self, tool, tmp_path)` — [`L160`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_smart_context_tool.py#L160)
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `TestSmartContextTool`
- def: [`tests/unit/mcp/test_smart_context_tool.py:55`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_smart_context_tool.py#L55)
- signature: `class TestSmartContextTool:`
- members:
  - `test_agent_summary_guides_next_action(self, tool)` — [`L74`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_smart_context_tool.py#L74)
  - `test_dependencies_structure(self, tool)` — [`L105`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_smart_context_tool.py#L105)
  - `test_edit_risk_is_valid(self, tool)` — [`L111`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_smart_context_tool.py#L111)
  - `test_execute_returns_complete_profile(self, tool)` — [`L63`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_smart_context_tool.py#L63)
  - `test_exports_include_classes_and_functions(self, tool)` — [`L93`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_smart_context_tool.py#L93)
  - `test_file_not_found(self, tool)` — [`L123`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_smart_context_tool.py#L123)
  - `test_health_has_grade_and_score(self, tool)` — [`L86`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_smart_context_tool.py#L86)
  - `test_json_format_works(self, tool)` — [`L140`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_smart_context_tool.py#L140)
  - `test_language_detected(self, tool)` — [`L119`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_smart_context_tool.py#L119)
  - `test_line_count(self, tool)` — [`L115`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_smart_context_tool.py#L115)
  - `test_structure_has_line_ranges(self, tool)` — [`L99`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_smart_context_tool.py#L99)
  - `test_toon_format_works(self, tool)` — [`L127`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_smart_context_tool.py#L127)
  - `test_validate_arguments_missing_path(self, tool)` — [`L56`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_smart_context_tool.py#L56)
  - `test_validate_arguments_valid(self, tool)` — [`L60`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_smart_context_tool.py#L60)
- uses (calls/refs, reference-scoped): (2 test-only callers)

### `TestStructureExtraction`
- def: [`tests/unit/mcp/test_smart_context_tool.py:205`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_smart_context_tool.py#L205)
- signature: `class TestStructureExtraction:`
- members:
  - `test_extracts_structure(self)` — [`L206`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_smart_context_tool.py#L206)
- uses (calls/refs, reference-scoped): [`extract_elements`](../../../tree_sitter_analyzer/mcp/tools/utils/element_extractor.md#extract_elements), [`get_structure`](../../../tree_sitter_analyzer/mcp/tools/utils/element_extractor.md#get_structure)  (1 test-only)

## Functions
- `_run(coro)` — [`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_smart_context_tool.py#L51)
- `tool(tmp_path)` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_smart_context_tool.py#L25)

## Module values
- `PROJECT_ROOT` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_smart_context_tool.py#L20)
- `TARGET_FILE` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_smart_context_tool.py#L21)

