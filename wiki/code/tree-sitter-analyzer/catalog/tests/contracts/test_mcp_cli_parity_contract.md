---
title: 'Module: tests/contracts/test_mcp_cli_parity_contract.py'
type: catalog
provenance: extracted
module: tests/contracts/test_mcp_cli_parity_contract.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.contracts.test_mcp_cli_parity_contract`/
symbols:
  test_registered_mcp_tools_have_cli_parity: test_registered_mcp_tools_have_cli_parity().
  test_facade_discovery_exposes_exactly_eight_facades: test_facade_discovery_exposes_exactly_eight_facades().
  PROJECT_ROOT: PROJECT_ROOT.
  test_all_facade_descriptions_contain_codegraph_keyword: test_all_facade_descriptions_contain_codegraph_keyword().
  test_facade_delegation_routes_each_action_to_expected_inner: test_facade_delegation_routes_each_action_to_expected_inner().
  test_every_tool_declares_mcp_annotations: test_every_tool_declares_mcp_annotations().
  _MAX_COMPOSED_TOOL_NAME: _MAX_COMPOSED_TOOL_NAME.
  _MCP_SERVER_NAME: _MCP_SERVER_NAME.
  SKIPPED_SCAN_DIRS: SKIPPED_SCAN_DIRS.
---
# Module: [`tests/contracts/test_mcp_cli_parity_contract.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/contracts/test_mcp_cli_parity_contract.py)

## Functions
- `test_all_facade_descriptions_contain_codegraph_keyword()` — [`L250`](../../../../../../raw/code/tree-sitter-analyzer/tests/contracts/test_mcp_cli_parity_contract.py#L250) — Fix ② discoverability contract: every facade description must contain
- `test_every_tool_declares_mcp_annotations()` — [`L416`](../../../../../../raw/code/tree-sitter-analyzer/tests/contracts/test_mcp_cli_parity_contract.py#L416) — Every registered MCP tool MUST set `annotations` in its tool definition.
- `test_facade_delegation_routes_each_action_to_expected_inner()` — [`L275`](../../../../../../raw/code/tree-sitter-analyzer/tests/contracts/test_mcp_cli_parity_contract.py#L275) — Delegation contract (PRD §5/§7): every (facade, action) reaches the
- `test_facade_discovery_exposes_exactly_eight_facades()` — [`L216`](../../../../../../raw/code/tree-sitter-analyzer/tests/contracts/test_mcp_cli_parity_contract.py#L216) — Discovery contract: the eager MCP surface is exactly the 8 facades.
- `test_registered_mcp_tools_have_cli_parity()` — [`L35`](../../../../../../raw/code/tree-sitter-analyzer/tests/contracts/test_mcp_cli_parity_contract.py#L35) — Every registered MCP tool must have a documented CLI access path.

## Module values
- `PROJECT_ROOT` — [`L23`](../../../../../../raw/code/tree-sitter-analyzer/tests/contracts/test_mcp_cli_parity_contract.py#L23)
- `SKIPPED_SCAN_DIRS` — [`L24`](../../../../../../raw/code/tree-sitter-analyzer/tests/contracts/test_mcp_cli_parity_contract.py#L24)
- `_MAX_COMPOSED_TOOL_NAME` — [`L213`](../../../../../../raw/code/tree-sitter-analyzer/tests/contracts/test_mcp_cli_parity_contract.py#L213)
- `_MCP_SERVER_NAME` — [`L212`](../../../../../../raw/code/tree-sitter-analyzer/tests/contracts/test_mcp_cli_parity_contract.py#L212)

