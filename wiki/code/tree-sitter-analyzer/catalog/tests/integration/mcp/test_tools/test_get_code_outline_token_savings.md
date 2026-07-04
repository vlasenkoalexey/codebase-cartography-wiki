---
title: 'Module: tests/integration/mcp/test_tools/test_get_code_outline_token_savings.py'
type: catalog
provenance: extracted
module: tests/integration/mcp/test_tools/test_get_code_outline_token_savings.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.mcp.test_tools.test_get_code_outline_token_savings`/
symbols:
  TestTokenSavingsGetCodeOutline.test_token_savings_summary: TestTokenSavingsGetCodeOutline#test_token_savings_summary().
  TestTokenSavingsGetCodeOutline.test_small_file_token_savings: TestTokenSavingsGetCodeOutline#test_small_file_token_savings().
  TestTokenSavingsGetCodeOutline.test_medium_file_token_savings: TestTokenSavingsGetCodeOutline#test_medium_file_token_savings().
  TestTokenSavingsGetCodeOutline.test_large_file_token_savings: TestTokenSavingsGetCodeOutline#test_large_file_token_savings().
  TestTokenSavingsGetCodeOutline.test_character_to_token_approximation: TestTokenSavingsGetCodeOutline#test_character_to_token_approximation().
  _payload_text: _payload_text().
  MEDIUM_PYTHON_CODE: MEDIUM_PYTHON_CODE.
  SMALL_PYTHON_CODE: SMALL_PYTHON_CODE.
  LARGE_JAVA_CODE: LARGE_JAVA_CODE.
  TestTokenSavingsGetCodeOutline: TestTokenSavingsGetCodeOutline#
---
# Module: [`tests/integration/mcp/test_tools/test_get_code_outline_token_savings.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_get_code_outline_token_savings.py)

## Classes
### `TestTokenSavingsGetCodeOutline`
- def: [`tests/integration/mcp/test_tools/test_get_code_outline_token_savings.py:372`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_get_code_outline_token_savings.py#L372)
- doc: 验证 TOON 格式相比 JSON 格式的 Token 节省效果
- signature: `class TestTokenSavingsGetCodeOutline:`
- members:
  - `test_character_to_token_approximation(self)` — [`L589`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_get_code_outline_token_savings.py#L589) — 验证字符数可作为 Token 数的近似指标
  - `test_large_file_token_savings(self)` — [`L476`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_get_code_outline_token_savings.py#L476) — 大文件（~250 行）：TOON 应至少节省 40% 字符
  - `test_medium_file_token_savings(self)` — [`L428`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_get_code_outline_token_savings.py#L428) — 中文件（~100 行）：TOON 应至少节省 40% 字符
  - `test_small_file_token_savings(self)` — [`L376`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_get_code_outline_token_savings.py#L376) — 小文件（~20 行）：TOON 应至少节省 40% 字符
  - `test_token_savings_summary(self)` — [`L524`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_get_code_outline_token_savings.py#L524) — 汇总测试：验证所有三种规模文件的平均 Token 节省效果
- uses (calls/refs, reference-scoped): [`GetCodeOutlineTool`](../../../../tree_sitter_analyzer/mcp/tools/get_code_outline_tool.md#GetCodeOutlineTool), [`execute`](../../../../tree_sitter_analyzer/mcp/tools/get_code_outline_tool.md#GetCodeOutlineTool.execute)  (4 test-only)

## Functions
- `_payload_text(result: dict)` — [`L18`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_get_code_outline_token_savings.py#L18) — Normalize v1.13.0+ direct-dict and legacy MCP-wrapped outputs.

## Module values
- `LARGE_JAVA_CODE` — [`L124`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_get_code_outline_token_savings.py#L124)
- `MEDIUM_PYTHON_CODE` — [`L50`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_get_code_outline_token_savings.py#L50)
- `SMALL_PYTHON_CODE` — [`L34`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_get_code_outline_token_savings.py#L34)

