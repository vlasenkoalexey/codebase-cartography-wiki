---
title: 'Module: tests/contracts/test_internal_architecture_contract.py'
type: catalog
provenance: extracted
module: tests/contracts/test_internal_architecture_contract.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.contracts.test_internal_architecture_contract`/
symbols:
  PROJECT_ROOT: PROJECT_ROOT.
  test_mcp_command_specs_have_resolvable_tool_classes: test_mcp_command_specs_have_resolvable_tool_classes().
  test_no_mcp_tool_overrides_set_project_path: test_no_mcp_tool_overrides_set_project_path().
  test_package_and_mcp_versions_are_aligned: test_package_and_mcp_versions_are_aligned().
  test_ast_cache_call_edge_extraction_does_not_depend_on_call_graph: test_ast_cache_call_edge_extraction_does_not_depend_on_call_graph().
  test_callee_resolution_algorithm_has_single_shared_home: test_callee_resolution_algorithm_has_single_shared_home().
  test_no_mcp_tool_imports_from_cli: test_no_mcp_tool_imports_from_cli().
  test_mcp_server_module_does_not_eagerly_import_tools: test_mcp_server_module_does_not_eagerly_import_tools().
  _class_overrides_set_project_path: _class_overrides_set_project_path().
  SKIPPED_SCAN_DIRS: SKIPPED_SCAN_DIRS.
---
# Module: [`tests/contracts/test_internal_architecture_contract.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/contracts/test_internal_architecture_contract.py)

## Functions
- `_class_overrides_set_project_path(node: ast.ClassDef)` — [`L115`](../../../../../../raw/code/tree-sitter-analyzer/tests/contracts/test_internal_architecture_contract.py#L115) — Return True if the class body contains a ``set_project_path`` method.
- `test_ast_cache_call_edge_extraction_does_not_depend_on_call_graph()` — [`L46`](../../../../../../raw/code/tree-sitter-analyzer/tests/contracts/test_internal_architecture_contract.py#L46) — ASTCache and CallGraph must share extraction helpers without a back-edge.
- `test_callee_resolution_algorithm_has_single_shared_home()` — [`L61`](../../../../../../raw/code/tree-sitter-analyzer/tests/contracts/test_internal_architecture_contract.py#L61) — CallGraph/CrossFile/Synapse may expose APIs, but not bespoke algorithms.
- `test_mcp_command_specs_have_resolvable_tool_classes()` — [`L159`](../../../../../../raw/code/tree-sitter-analyzer/tests/contracts/test_internal_architecture_contract.py#L159) — ARCH-A2 regression: every MCP_COMMAND_SPECS entry's ``tool_attr``
- `test_mcp_server_module_does_not_eagerly_import_tools()` — [`L183`](../../../../../../raw/code/tree-sitter-analyzer/tests/contracts/test_internal_architecture_contract.py#L183) — PERF-3 regression: ``tree_sitter_analyzer.mcp.server`` must not import
- `test_no_mcp_tool_imports_from_cli()` — [`L77`](../../../../../../raw/code/tree-sitter-analyzer/tests/contracts/test_internal_architecture_contract.py#L77) — ARCH-A1 regression: ``mcp/tools/*.py`` must not import from
- `test_no_mcp_tool_overrides_set_project_path()` — [`L124`](../../../../../../raw/code/tree-sitter-analyzer/tests/contracts/test_internal_architecture_contract.py#L124) — ARCH-A4 regression: ``BaseMCPTool.set_project_path`` is final by
- `test_package_and_mcp_versions_are_aligned()` — [`L34`](../../../../../../raw/code/tree-sitter-analyzer/tests/contracts/test_internal_architecture_contract.py#L34) — Release prep must keep package and MCP server versions in lockstep.

## Module values
- `PROJECT_ROOT` — [`L23`](../../../../../../raw/code/tree-sitter-analyzer/tests/contracts/test_internal_architecture_contract.py#L23)
- `SKIPPED_SCAN_DIRS` — [`L24`](../../../../../../raw/code/tree-sitter-analyzer/tests/contracts/test_internal_architecture_contract.py#L24)

