---
title: 'Module: tests/unit/security/test_security_integration.py'
type: catalog
provenance: extracted
module: tests/unit/security/test_security_integration.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.security.test_security_integration`/TestSecurityIntegration#
symbols:
  TestSecurityIntegration.test_mcp_tools_security_integration: test_mcp_tools_security_integration().
  TestSecurityIntegration.test_security_validator_consistency: test_security_validator_consistency().
  TestSecurityIntegration.test_file: test_file.
  TestSecurityIntegration.test_analyze_scale_tool_security: test_analyze_scale_tool_security().
  TestSecurityIntegration.temp_dir: temp_dir.
  TestSecurityIntegration.test_analysis_engine_security_integration: test_analysis_engine_security_integration().
  TestSecurityIntegration.test_read_partial_tool_security: test_read_partial_tool_security().
  TestSecurityIntegration.test_cli_command_security_integration: test_cli_command_security_integration().
  TestSecurityIntegration.test_query_command_security: test_query_command_security().
  TestSecurityIntegration.test_performance_impact: test_performance_impact().
  TestSecurityIntegration.test_audit_logging: test_audit_logging().
  TestSecurityIntegration.test_error_handling_security: test_error_handling_security().
  TestSecurityIntegration.setup_method: setup_method().
  TestSecurityIntegration.test_input_sanitization_consistency: test_input_sanitization_consistency().
  TestSecurityIntegration.test_cli_command_security_integration.TestCommand: test_cli_command_security_integration().TestCommand#
  TestSecurityIntegration.teardown_method: teardown_method().
  TestSecurityIntegration: ''
  TestSecurityIntegration.test_cli_command_security_integration.TestCommand.execute_async: test_cli_command_security_integration().TestCommand#execute_async().
---
# Module: [`tests/unit/security/test_security_integration.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_integration.py)

## Classes
### `TestCommand`  ·  implements/extends BaseCommand
- def: [`tests/unit/security/test_security_integration.py:187`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_integration.py#L187)
- signature: `class TestCommand(BaseCommand):`
- members:
  - `execute_async(self, language: str)` — [`L188`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_integration.py#L188)
- uses (calls/refs, reference-scoped): [`BaseCommand`](../../../tree_sitter_analyzer/cli/commands/base_command.md#BaseCommand)
- used by: [`BaseCommand`](../../../tree_sitter_analyzer/cli/commands/base_command.md#BaseCommand), [`execute_async`](../../../tree_sitter_analyzer/cli/commands/base_command.md#BaseCommand.execute_async)  (1 test-only)

### `TestSecurityIntegration`
- def: [`tests/unit/security/test_security_integration.py:26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_integration.py#L26)
- doc: Test security integration across all components.
- signature: `class TestSecurityIntegration:`
- members:
  - `setup_method(self)` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_integration.py#L29) — Set up test environment.
  - `teardown_method(self)` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_integration.py#L53) — Clean up test environment.
  - `test_analysis_engine_security_integration(self)` — [`L60`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_integration.py#L60) — Test that analysis engine properly validates file paths.
  - `test_analyze_scale_tool_security(self)` — [`L146`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_integration.py#L146) — Test AnalyzeScaleTool security validation.
  - `test_audit_logging(self)` — [`L294`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_integration.py#L294) — Test that security events are properly logged.
  - `test_cli_command_security_integration(self)` — [`L182`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_integration.py#L182) — Test CLI command security validation.
  - `test_error_handling_security(self)` — [`L317`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_integration.py#L317) — Test that error messages don't leak sensitive information.
  - `test_input_sanitization_consistency(self)` — [`L259`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_integration.py#L259) — Test that input sanitization is consistent across components.
  - `test_mcp_tools_security_integration(self)` — [`L79`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_integration.py#L79) — Test that MCP tools properly validate inputs.
  - `test_performance_impact(self)` — [`L276`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_integration.py#L276) — Test that security validation doesn't significantly impact performance.
  - `test_query_command_security(self)` — [`L205`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_integration.py#L205) — Test QueryCommand security for query strings.
  - `test_read_partial_tool_security(self)` — [`L116`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_integration.py#L116) — Test ReadPartialTool security validation.
  - `test_security_validator_consistency(self)` — [`L231`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_integration.py#L231) — Test that all components use consistent security validation.
  - `temp_dir` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_integration.py#L36)
  - `test_file` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_integration.py#L37)
- uses (calls/refs, reference-scoped): [`ReadPartialTool`](../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool), [`UnifiedAnalysisEngine`](../../../tree_sitter_analyzer/core/analysis_engine.md#UnifiedAnalysisEngine), [`SecurityValidator`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator), [`AnalyzeCodeStructureTool`](../../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#AnalyzeCodeStructureTool), [`AnalyzeScaleTool`](../../../tree_sitter_analyzer/mcp/tools/analyze_scale_tool.md#AnalyzeScaleTool), [`UniversalAnalyzeTool`](../../../tree_sitter_analyzer/mcp/tools/universal_analyze_tool.md#UniversalAnalyzeTool), [`validate_file_path`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator.validate_file_path), [`get_analysis_engine`](../../../tree_sitter_analyzer/core/analysis_engine.md#get_analysis_engine), [`execute`](../../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#AnalyzeCodeStructureTool.execute), [`execute`](../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool.execute), [`execute`](../../../tree_sitter_analyzer/mcp/tools/analyze_scale_tool.md#AnalyzeScaleTool.execute), [`execute`](../../../tree_sitter_analyzer/mcp/tools/universal_analyze_tool.md#UniversalAnalyzeTool.execute), [`analyze_file`](../../../tree_sitter_analyzer/core/_analysis_engine_file_mixin.md#UnifiedAnalysisEngineFileMixin.analyze_file), [`sanitize_input`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator.sanitize_input), [`QueryCommand`](../../../tree_sitter_analyzer/cli/commands/query_command.md#QueryCommand), [`security_validator`](../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.security_validator), [`validate_file`](../../../tree_sitter_analyzer/cli/commands/base_command.md#BaseCommand.validate_file), [`execute_async`](../../../tree_sitter_analyzer/cli/commands/query_command.md#QueryCommand.execute_async), [`_instances`](../../../tree_sitter_analyzer/core/analysis_engine.md#UnifiedAnalysisEngine._instances), [`security_validator`](../../../tree_sitter_analyzer/core/_analysis_engine_runtime_mixin.md#UnifiedAnalysisEngineRuntimeMixin.security_validator)  (1 test-only)

