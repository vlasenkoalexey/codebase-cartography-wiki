---
title: 'Module: tests/unit/mcp/test_enum_error_enumeration.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_enum_error_enumeration.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_enum_error_enumeration`/
symbols:
  _ENUM_TOOLS._ENUM_TOOLS: _ENUM_TOOLS._ENUM_TOOLS.
  _capture_call_tool_handler: _capture_call_tool_handler().
  test_boundary_enum_error_lists_values_and_canonical_hint: test_boundary_enum_error_lists_values_and_canonical_hint().
  _capture_call_tool_handler.capture_decorator: _capture_call_tool_handler().capture_decorator().
  _capture_call_tool_handler.capture_decorator.decorator: _capture_call_tool_handler().capture_decorator().decorator().
  test_invalid_mode_enumerates_valid_values: test_invalid_mode_enumerates_valid_values().
---
# Module: [`tests/unit/mcp/test_enum_error_enumeration.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_enum_error_enumeration.py)

## Functions
- `_capture_call_tool_handler(server: TreeSitterAnalyzerMCPServer)` — [`L74`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_enum_error_enumeration.py#L74) — Capture the ``handle_call_tool`` closure registered by ``create_server``.
- `capture_decorator(name)` — [`L81`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_enum_error_enumeration.py#L81)
- `decorator(func)` — [`L82`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_enum_error_enumeration.py#L82)
- `test_boundary_enum_error_lists_values_and_canonical_hint(tmp_path)` — [`L94`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_enum_error_enumeration.py#L94) — #690 headline repro through the real boundary: viz action=similarity with
- `test_invalid_mode_enumerates_valid_values(tool_cls: type, expected_modes: set[str], tmp_path)` — [`L52`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_enum_error_enumeration.py#L52) — A bad ``mode`` raises a ValueError that lists the valid modes (#690).

## Module values
- `_ENUM_TOOLS` — [`L42`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_enum_error_enumeration.py#L42)

