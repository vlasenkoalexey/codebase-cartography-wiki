---
title: 'Module: tests/integration/mcp/test_user_story_1_integration.py'
type: catalog
provenance: extracted
module: tests/integration/mcp/test_user_story_1_integration.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.mcp.test_user_story_1_integration`/TestUserStory1Integration#
symbols:
  TestUserStory1Integration.test_files: test_files.
  TestUserStory1Integration.test_complete_analysis_workflow: test_complete_analysis_workflow().
  TestUserStory1Integration.test_large_file_token_optimization: test_large_file_token_optimization().
  TestUserStory1Integration.test_error_handling_integration: test_error_handling_integration().
  TestUserStory1Integration.test_multi_language_support: test_multi_language_support().
  TestUserStory1Integration.test_performance_requirements: test_performance_requirements().
  TestUserStory1Integration.test_user_story_acceptance_criteria: test_user_story_acceptance_criteria().
  TestUserStory1Integration.test_checkpoint_user_story_1_completion: test_checkpoint_user_story_1_completion().
  TestUserStory1Integration.scale_tool: scale_tool.
  TestUserStory1Integration.table_tool: table_tool.
  TestUserStory1Integration.teardown_method: teardown_method().
  TestUserStory1Integration: ''
  TestUserStory1Integration.setup_method: setup_method().
---
# Module: [`tests/integration/mcp/test_user_story_1_integration.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_1_integration.py)

## Classes
### `TestUserStory1Integration`
- def: [`tests/integration/mcp/test_user_story_1_integration.py:30`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_1_integration.py#L30)
- doc: Integration tests for User Story 1: Basic Code Analysis Tools
- signature: `class TestUserStory1Integration:`
- members:
  - `setup_method(self)` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_1_integration.py#L33) — Setup tools and test files for integration testing
  - `teardown_method(self)` — [`L462`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_1_integration.py#L462) — Cleanup test files
  - `test_checkpoint_user_story_1_completion(self)` — [`L745`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_1_integration.py#L745) — Checkpoint test: Verify User Story 1 is independently testable and complete
  - `test_complete_analysis_workflow(self)` — [`L473`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_1_integration.py#L473) — Test complete analysis workflow: scale → structure → integration
  - `test_error_handling_integration(self)` — [`L570`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_1_integration.py#L570) — Test error handling across both tools
  - `test_large_file_token_optimization(self)` — [`L530`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_1_integration.py#L530) — Test token optimization strategy for large files
  - `test_multi_language_support(self)` — [`L610`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_1_integration.py#L610) — Test multi-language support across both tools
  - `test_performance_requirements(self)` — [`L665`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_1_integration.py#L665) — Test performance requirements for User Story 1
  - `test_user_story_acceptance_criteria(self)` — [`L699`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_1_integration.py#L699) — Test User Story 1 acceptance criteria
  - `scale_tool` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_1_integration.py#L36)
  - `table_tool` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_1_integration.py#L37)
  - `test_files` — [`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_user_story_1_integration.py#L40)
- uses (calls/refs, reference-scoped): [`AnalyzeCodeStructureTool`](../../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#AnalyzeCodeStructureTool), [`AnalyzeScaleTool`](../../../tree_sitter_analyzer/mcp/tools/analyze_scale_tool.md#AnalyzeScaleTool), [`execute`](../../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#AnalyzeCodeStructureTool.execute), [`execute`](../../../tree_sitter_analyzer/mcp/tools/analyze_scale_tool.md#AnalyzeScaleTool.execute)

