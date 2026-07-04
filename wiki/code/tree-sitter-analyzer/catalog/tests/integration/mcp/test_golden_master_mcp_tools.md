---
title: 'Module: tests/integration/mcp/test_golden_master_mcp_tools.py'
type: catalog
provenance: extracted
module: tests/integration/mcp/test_golden_master_mcp_tools.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.mcp.test_golden_master_mcp_tools`/
symbols:
  SemanticComparator.compare_tool_responses: SemanticComparator#compare_tool_responses().
  SemanticComparator: SemanticComparator#
  GoldenMasterMCPTester.assert_matches_golden_master: GoldenMasterMCPTester#assert_matches_golden_master().
  SemanticComparator._compare_result_sets: SemanticComparator#_compare_result_sets().
  GoldenMasterMCPTester.golden_dir: GoldenMasterMCPTester#golden_dir.
  TestIntentAliasInvariance.test_locate_usage_search_content_invariance: TestIntentAliasInvariance#test_locate_usage_search_content_invariance().
  TestIntentAliasInvariance.test_map_structure_list_files_invariance: TestIntentAliasInvariance#test_map_structure_list_files_invariance().
  TestIntentAliasInvariance.test_extract_structure_analyze_code_structure_invariance: TestIntentAliasInvariance#test_extract_structure_analyze_code_structure_invariance().
  TestIntentAliasInvariance.test_navigate_structure_get_code_outline_invariance: TestIntentAliasInvariance#test_navigate_structure_get_code_outline_invariance().
  TestIntentAliasInvariance.test_find_impacted_code_find_and_grep_invariance: TestIntentAliasInvariance#test_find_impacted_code_find_and_grep_invariance().
  TestIntentAliasInvariance.test_multiple_aliases_same_tool_invariance: TestIntentAliasInvariance#test_multiple_aliases_same_tool_invariance().
  GoldenMasterMCPTester.save_golden_master: GoldenMasterMCPTester#save_golden_master().
  GoldenMasterMCPTester.load_golden_master: GoldenMasterMCPTester#load_golden_master().
  mcp_server: mcp_server().
  golden_tester: golden_tester().
  GoldenMasterMCPTester: GoldenMasterMCPTester#
  GoldenMasterMCPTester.__init__: GoldenMasterMCPTester#__init__().
  temp_test_file: temp_test_file().
  TestIntentAliasInvariance: TestIntentAliasInvariance#
  TestIncompleteModificationDetection: TestIncompleteModificationDetection#
  TestIncompleteModificationDetection.test_tool_response_structure_consistency: TestIncompleteModificationDetection#test_tool_response_structure_consistency().
---
# Module: [`tests/integration/mcp/test_golden_master_mcp_tools.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_golden_master_mcp_tools.py)

## Classes
### `GoldenMasterMCPTester`
- def: [`tests/integration/mcp/test_golden_master_mcp_tools.py:206`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_golden_master_mcp_tools.py#L206)
- doc: MCP 工具的 Golden Master 测试器
- signature: `class GoldenMasterMCPTester:`
- members:
  - `assert_matches_golden_master(self, tool_name: str, test_case: str, actual_response: dict[str, Any], update_golden: bool = False)` — [`L244`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_golden_master_mcp_tools.py#L244) — 断言响应与 golden master 匹配
  - `load_golden_master(self, tool_name: str, test_case: str)` — [`L231`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_golden_master_mcp_tools.py#L231) — 加载 golden master 基线
  - `save_golden_master(self, tool_name: str, test_case: str, response: dict[str, Any])` — [`L219`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_golden_master_mcp_tools.py#L219) — 保存 golden master 基线
  - `golden_dir` — [`L216`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_golden_master_mcp_tools.py#L216)
- protocol/private: `__init__`[`L213`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_golden_master_mcp_tools.py#L213)
- uses (calls/refs, reference-scoped): (2 test-only callers)
- used by: (1 test-only callers)

### `SemanticComparator`
- def: [`tests/integration/mcp/test_golden_master_mcp_tools.py:37`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_golden_master_mcp_tools.py#L37)
- doc: 语义比较器 - 理解工具响应的结构和意义
- signature: `class SemanticComparator:`
- members:
  - `_compare_result_sets(actual: list[Any], expected: list[Any], ignore_fields: set[str])` — [`L170`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_golden_master_mcp_tools.py#L170) — 比较结果集合（集合语义，忽略顺序）
  - `compare_tool_responses(actual: dict[str, Any] | list[Any], expected: dict[str, Any] | list[Any], ignore_fields: set[str] | None = None)` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_golden_master_mcp_tools.py#L49) — 比较两个工具响应是否语义等价
- used by: (7 test-only callers)

### `TestIncompleteModificationDetection`
- def: [`tests/integration/mcp/test_golden_master_mcp_tools.py:538`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_golden_master_mcp_tools.py#L538)
- doc: 不完整修改检测测试
- signature: `class TestIncompleteModificationDetection:`
- members:
  - `test_tool_response_structure_consistency(self, mcp_server, temp_test_file)` — [`L549`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_golden_master_mcp_tools.py#L549) — 所有工具必须返回一致的响应结构

### `TestIntentAliasInvariance`
- def: [`tests/integration/mcp/test_golden_master_mcp_tools.py:317`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_golden_master_mcp_tools.py#L317)
- doc: Intent Alias 不变性测试
- signature: `class TestIntentAliasInvariance:`
- members:
  - `test_extract_structure_analyze_code_structure_invariance(self, mcp_server, temp_test_file)` — [`L394`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_golden_master_mcp_tools.py#L394) — extract_structure 和 analyze_code_structure 必须返回相同结果
  - `test_find_impacted_code_find_and_grep_invariance(self, mcp_server, temp_test_file)` — [`L456`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_golden_master_mcp_tools.py#L456) — find_impacted_code 和 find_and_grep 必须返回相同结果
  - `test_locate_usage_search_content_invariance(self, mcp_server, temp_test_file)` — [`L325`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_golden_master_mcp_tools.py#L325) — locate_usage 和 search_content 必须返回相同结果
  - `test_map_structure_list_files_invariance(self, mcp_server, temp_test_file)` — [`L361`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_golden_master_mcp_tools.py#L361) — map_structure 和 list_files 必须返回相同结果
  - `test_multiple_aliases_same_tool_invariance(self, mcp_server, temp_test_file)` — [`L489`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_golden_master_mcp_tools.py#L489) — 测试同一工具的多个 alias 返回相同结果 (find_usage 和 locate_usage)
  - `test_navigate_structure_get_code_outline_invariance(self, mcp_server, temp_test_file)` — [`L425`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_golden_master_mcp_tools.py#L425) — navigate_structure 和 get_code_outline 必须返回相同结果
- uses (calls/refs, reference-scoped): (2 test-only callers)

## Functions
- `golden_tester()` — [`L292`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_golden_master_mcp_tools.py#L292) — Session-scoped golden master tester
- `mcp_server()` — [`L286`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_golden_master_mcp_tools.py#L286) — Session-scoped MCP server
- `temp_test_file()` — [`L298`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_golden_master_mcp_tools.py#L298) — 创建临时测试文件（每个测试独立目录）

