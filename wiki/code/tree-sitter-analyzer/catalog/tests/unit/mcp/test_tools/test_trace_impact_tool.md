---
title: 'Module: tests/unit/mcp/test_tools/test_trace_impact_tool.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_tools/test_trace_impact_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_tools.test_trace_impact_tool`/Test
symbols:
  TestTraceImpactToolBasic.tool: TraceImpactToolBasic#tool.
  TestTraceImpactToolBasic.test_init: TraceImpactToolBasic#test_init().
  TestTraceImpactToolExecution.tool: TraceImpactToolExecution#tool.
  TestTraceImpactToolLanguageDetection.tool: TraceImpactToolLanguageDetection#tool.
  TestTraceImpactToolBasic.test_get_tool_definition: TraceImpactToolBasic#test_get_tool_definition().
  TestTraceImpactToolBasic.test_validate_arguments_valid: TraceImpactToolBasic#test_validate_arguments_valid().
  TestTraceImpactToolBasic.test_validate_arguments_missing_symbol: TraceImpactToolBasic#test_validate_arguments_missing_symbol().
  TestTraceImpactToolBasic.test_validate_arguments_empty_symbol: TraceImpactToolBasic#test_validate_arguments_empty_symbol().
  TestTraceImpactToolBasic.test_validate_arguments_invalid_file_path_type: TraceImpactToolBasic#test_validate_arguments_invalid_file_path_type().
  TestTraceImpactToolBasic.test_validate_arguments_invalid_case_sensitive_type: TraceImpactToolBasic#test_validate_arguments_invalid_case_sensitive_type().
  TestTraceImpactToolBasic.test_validate_arguments_invalid_max_results: TraceImpactToolBasic#test_validate_arguments_invalid_max_results().
  TestTraceImpactToolBasic.test_validate_arguments_invalid_exclude_patterns_type: TraceImpactToolBasic#test_validate_arguments_invalid_exclude_patterns_type().
  TestTraceImpactToolExecution.test_execute_no_matches: TraceImpactToolExecution#test_execute_no_matches().
  TestTraceImpactToolExecution.test_execute_with_matches: TraceImpactToolExecution#test_execute_with_matches().
  TestTraceImpactToolExecution.test_execute_with_language_filtering: TraceImpactToolExecution#test_execute_with_language_filtering().
  TestTraceImpactToolExecution.test_execute_with_max_results_truncation: TraceImpactToolExecution#test_execute_with_max_results_truncation().
  TestTraceImpactToolExecution.test_execute_ripgrep_not_installed: TraceImpactToolExecution#test_execute_ripgrep_not_installed().
  TestTraceImpactToolExecution.test_execute_timeout: TraceImpactToolExecution#test_execute_timeout().
  TestTraceImpactToolExecution.test_execute_with_multiple_roots: TraceImpactToolExecution#test_execute_with_multiple_roots().
  TestTraceImpactToolLanguageDetection.test_get_extensions_for_language_java: TraceImpactToolLanguageDetection#test_get_extensions_for_language_java().
  TestTraceImpactToolLanguageDetection.test_get_extensions_for_language_python: TraceImpactToolLanguageDetection#test_get_extensions_for_language_python().
  TestTraceImpactToolLanguageDetection.test_get_extensions_for_language_javascript: TraceImpactToolLanguageDetection#test_get_extensions_for_language_javascript().
  TestTraceImpactToolLanguageDetection.test_get_extensions_for_language_unknown: TraceImpactToolLanguageDetection#test_get_extensions_for_language_unknown().
  TestTraceImpactToolExecution.setup_method: TraceImpactToolExecution#setup_method().
  TestR37sImpactGuidanceGrammar.test_low_impact_single_caller_uses_singular: R37sImpactGuidanceGrammar#test_low_impact_single_caller_uses_singular().
  TestR37sImpactGuidanceGrammar.test_low_impact_multiple_callers_uses_plural: R37sImpactGuidanceGrammar#test_low_impact_multiple_callers_uses_plural().
  TestR37sImpactGuidanceGrammar.test_low_impact_five_callers_uses_plural: R37sImpactGuidanceGrammar#test_low_impact_five_callers_uses_plural().
  TestTraceImpactToolBasic: TraceImpactToolBasic#
  TestTraceImpactToolBasic.setup_method: TraceImpactToolBasic#setup_method().
  TestTraceImpactToolExecution: TraceImpactToolExecution#
  TestTraceImpactToolLanguageDetection: TraceImpactToolLanguageDetection#
  TestTraceImpactToolLanguageDetection.setup_method: TraceImpactToolLanguageDetection#setup_method().
  TestR37sImpactGuidanceGrammar: R37sImpactGuidanceGrammar#
---
# Module: [`tests/unit/mcp/test_tools/test_trace_impact_tool.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_trace_impact_tool.py)

## Classes
### `TestR37sImpactGuidanceGrammar`
- def: [`tests/unit/mcp/test_tools/test_trace_impact_tool.py:262`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_trace_impact_tool.py#L262)
- doc: r37s dogfood: `_get_impact_level` emitted `"3 caller(s) found"` —
- signature: `class TestR37sImpactGuidanceGrammar:`
- members:
  - `test_low_impact_five_callers_uses_plural(self)` — [`L288`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_trace_impact_tool.py#L288) — 5 is still ``low`` per the existing bucket (count <= 5).
  - `test_low_impact_multiple_callers_uses_plural(self)` — [`L278`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_trace_impact_tool.py#L278)
  - `test_low_impact_single_caller_uses_singular(self)` — [`L268`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_trace_impact_tool.py#L268)
- uses (calls/refs, reference-scoped): [`_get_impact_level`](../../../../tree_sitter_analyzer/mcp/tools/trace_impact_tool.md#_get_impact_level)

### `TestTraceImpactToolBasic`
- def: [`tests/unit/mcp/test_tools/test_trace_impact_tool.py:15`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_trace_impact_tool.py#L15)
- doc: Basic functionality tests for trace_impact tool
- signature: `class TestTraceImpactToolBasic:`
- members:
  - `setup_method(self)` — [`L18`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_trace_impact_tool.py#L18) — Set up test fixtures
  - `test_get_tool_definition(self)` — [`L27`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_trace_impact_tool.py#L27) — Test tool definition structure
  - `test_init(self)` — [`L22`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_trace_impact_tool.py#L22) — Test tool initialization
  - `test_validate_arguments_empty_symbol(self)` — [`L56`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_trace_impact_tool.py#L56) — Test argument validation with empty symbol
  - `test_validate_arguments_invalid_case_sensitive_type(self)` — [`L68`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_trace_impact_tool.py#L68) — Test argument validation with invalid case_sensitive type
  - `test_validate_arguments_invalid_exclude_patterns_type(self)` — [`L80`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_trace_impact_tool.py#L80) — Test argument validation with invalid exclude_patterns type
  - `test_validate_arguments_invalid_file_path_type(self)` — [`L62`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_trace_impact_tool.py#L62) — Test argument validation with invalid file_path type
  - `test_validate_arguments_invalid_max_results(self)` — [`L74`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_trace_impact_tool.py#L74) — Test argument validation with invalid max_results
  - `test_validate_arguments_missing_symbol(self)` — [`L50`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_trace_impact_tool.py#L50) — Test argument validation with missing symbol
  - `test_validate_arguments_valid(self)` — [`L36`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_trace_impact_tool.py#L36) — Test argument validation with valid inputs
  - `tool` — [`L20`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_trace_impact_tool.py#L20)
- uses (calls/refs, reference-scoped): [`project_root`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.project_root), [`TraceImpactTool`](../../../../tree_sitter_analyzer/mcp/tools/trace_impact_tool.md#TraceImpactTool), [`validate_arguments`](../../../../tree_sitter_analyzer/mcp/tools/trace_impact_tool.md#TraceImpactTool.validate_arguments), [`get_tool_definition`](../../../../tree_sitter_analyzer/mcp/tools/trace_impact_tool.md#TraceImpactTool.get_tool_definition), [`language_detector`](../../../../tree_sitter_analyzer/mcp/tools/trace_impact_tool.md#TraceImpactTool.language_detector)

### `TestTraceImpactToolExecution`
- def: [`tests/unit/mcp/test_tools/test_trace_impact_tool.py:87`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_trace_impact_tool.py#L87)
- doc: Test trace_impact execution with mocked ripgrep
- signature: `class TestTraceImpactToolExecution:`
- members:
  - `setup_method(self)` — [`L90`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_trace_impact_tool.py#L90) — Set up test fixtures
  - `test_execute_no_matches(self)` — [`L95`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_trace_impact_tool.py#L95) — Test execution when no matches are found
  - `test_execute_ripgrep_not_installed(self)` — [`L185`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_trace_impact_tool.py#L185) — Test execution when ripgrep is not installed
  - `test_execute_timeout(self)` — [`L199`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_trace_impact_tool.py#L199) — Test execution timeout
  - `test_execute_with_language_filtering(self)` — [`L136`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_trace_impact_tool.py#L136) — Test execution with language filtering
  - `test_execute_with_matches(self)` — [`L112`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_trace_impact_tool.py#L112) — Test execution with successful matches
  - `test_execute_with_max_results_truncation(self)` — [`L160`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_trace_impact_tool.py#L160) — Test execution with max_results truncation
  - `test_execute_with_multiple_roots(self)` — [`L213`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_trace_impact_tool.py#L213) — Test execution with multiple project roots
  - `tool` — [`L92`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_trace_impact_tool.py#L92)
- uses (calls/refs, reference-scoped): [`execute`](../../../../tree_sitter_analyzer/mcp/tools/trace_impact_tool.md#TraceImpactTool.execute), [`TraceImpactTool`](../../../../tree_sitter_analyzer/mcp/tools/trace_impact_tool.md#TraceImpactTool)

### `TestTraceImpactToolLanguageDetection`
- def: [`tests/unit/mcp/test_tools/test_trace_impact_tool.py:229`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_trace_impact_tool.py#L229)
- doc: Test language detection and extension filtering
- signature: `class TestTraceImpactToolLanguageDetection:`
- members:
  - `setup_method(self)` — [`L232`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_trace_impact_tool.py#L232) — Set up test fixtures
  - `test_get_extensions_for_language_java(self)` — [`L236`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_trace_impact_tool.py#L236) — Test getting extensions for Java
  - `test_get_extensions_for_language_javascript(self)` — [`L248`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_trace_impact_tool.py#L248) — Test getting extensions for JavaScript
  - `test_get_extensions_for_language_python(self)` — [`L242`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_trace_impact_tool.py#L242) — Test getting extensions for Python
  - `test_get_extensions_for_language_unknown(self)` — [`L256`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_trace_impact_tool.py#L256) — Test getting extensions for unknown language
  - `tool` — [`L234`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_trace_impact_tool.py#L234)
- uses (calls/refs, reference-scoped): [`TraceImpactTool`](../../../../tree_sitter_analyzer/mcp/tools/trace_impact_tool.md#TraceImpactTool), [`_get_extensions_for_language`](../../../../tree_sitter_analyzer/mcp/tools/trace_impact_tool.md#TraceImpactTool._get_extensions_for_language)

