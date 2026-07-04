---
title: 'Module: tests/unit/core/test_request.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_request.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_request`/TestAnalysisRequest#
symbols:
  TestAnalysisRequest.test_init_with_all_parameters: test_init_with_all_parameters().
  TestAnalysisRequest.test_init_with_defaults: test_init_with_defaults().
  TestAnalysisRequest.test_init_with_partial_parameters: test_init_with_partial_parameters().
  TestAnalysisRequest.test_from_mcp_arguments_all_fields: test_from_mcp_arguments_all_fields().
  TestAnalysisRequest.test_from_mcp_arguments_minimal: test_from_mcp_arguments_minimal().
  TestAnalysisRequest.test_from_mcp_arguments_empty: test_from_mcp_arguments_empty().
  TestAnalysisRequest.test_from_mcp_arguments_preserves_defaults: test_from_mcp_arguments_preserves_defaults().
  TestAnalysisRequest.test_boolean_flags_combinations: test_boolean_flags_combinations().
  TestAnalysisRequest.test_from_mcp_arguments_none_values: test_from_mcp_arguments_none_values().
  TestAnalysisRequest.test_from_mcp_arguments_type_coercion: test_from_mcp_arguments_type_coercion().
  TestAnalysisRequest.test_from_mcp_arguments_extra_fields: test_from_mcp_arguments_extra_fields().
  TestAnalysisRequest.test_multiple_from_mcp_calls: test_multiple_from_mcp_calls().
  TestAnalysisRequest.test_format_type_variations: test_format_type_variations().
  TestAnalysisRequest.test_queries_list: test_queries_list().
  TestAnalysisRequest.test_queries_empty_list: test_queries_empty_list().
  TestAnalysisRequest.test_language_variations: test_language_variations().
  TestAnalysisRequest.test_request_immutability_check: test_request_immutability_check().
  TestAnalysisRequest.test_from_mcp_arguments_with_special_characters: test_from_mcp_arguments_with_special_characters().
  TestAnalysisRequest.test_dataclass_not_frozen: test_dataclass_not_frozen().
  TestAnalysisRequest.test_file_path_required: test_file_path_required().
  TestAnalysisRequest: ''
---
# Module: [`tests/unit/core/test_request.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_request.py)

## Classes
### `TestAnalysisRequest`
- def: [`tests/unit/core/test_request.py:11`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_request.py#L11)
- doc: AnalysisRequest测试类
- signature: `class TestAnalysisRequest:`
- members:
  - `test_boolean_flags_combinations(self)` — [`L164`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_request.py#L164) — 测试布尔标志的不同组合
  - `test_dataclass_not_frozen(self)` — [`L63`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_request.py#L63) — 测试dataclass不是frozen的
  - `test_file_path_required(self)` — [`L151`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_request.py#L151) — 测试file_path是必需的
  - `test_format_type_variations(self)` — [`L157`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_request.py#L157) — 测试不同的format_type值
  - `test_from_mcp_arguments_all_fields(self)` — [`L69`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_request.py#L69) — 测试从MCP参数创建请求（所有字段）
  - `test_from_mcp_arguments_empty(self)` — [`L95`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_request.py#L95) — 测试从空MCP参数创建请求
  - `test_from_mcp_arguments_extra_fields(self)` — [`L105`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_request.py#L105) — 测试从包含额外字段的MCP参数创建请求
  - `test_from_mcp_arguments_minimal(self)` — [`L85`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_request.py#L85) — 测试从MCP参数创建请求（最小参数）
  - `test_from_mcp_arguments_none_values(self)` — [`L120`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_request.py#L120) — 测试从包含None值的MCP参数创建请求
  - `test_from_mcp_arguments_preserves_defaults(self)` — [`L229`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_request.py#L229) — 测试from_mcp_arguments保留未提供字段的默认值
  - `test_from_mcp_arguments_type_coercion(self)` — [`L137`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_request.py#L137) — 测试MCP参数类型强制转换
  - `test_from_mcp_arguments_with_special_characters(self)` — [`L252`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_request.py#L252) — 测试MCP参数中的特殊字符
  - `test_init_with_all_parameters(self)` — [`L14`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_request.py#L14) — 测试使用所有参数初始化
  - `test_init_with_defaults(self)` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_request.py#L35) — 测试使用默认参数初始化
  - `test_init_with_partial_parameters(self)` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_request.py#L47) — 测试使用部分参数初始化
  - `test_language_variations(self)` — [`L206`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_request.py#L206) — 测试不同的language值
  - `test_multiple_from_mcp_calls(self)` — [`L239`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_request.py#L239) — 测试多次调用from_mcp_arguments
  - `test_queries_empty_list(self)` — [`L197`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_request.py#L197) — 测试空的queries列表
  - `test_queries_list(self)` — [`L187`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_request.py#L187) — 测试queries列表参数
  - `test_request_immutability_check(self)` — [`L213`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_request.py#L213) — 测试请求对象的可变性（dataclass不是frozen）
- uses (calls/refs, reference-scoped): [`AnalysisRequest`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest), [`file_path`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest.file_path), [`language`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest.language), [`include_complexity`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest.include_complexity), [`include_details`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest.include_details), [`format_type`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest.format_type), [`include_queries`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest.include_queries), [`queries`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest.queries), [`include_elements`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest.include_elements), [`from_mcp_arguments`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest.from_mcp_arguments)

