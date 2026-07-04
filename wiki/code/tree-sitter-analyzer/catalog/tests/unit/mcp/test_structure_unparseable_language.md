---
title: 'Module: tests/unit/mcp/test_structure_unparseable_language.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_structure_unparseable_language.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_structure_unparseable_language`/
symbols:
  test_structure_boundary_classifies_as_language_unsupported: test_structure_boundary_classifies_as_language_unsupported().
  _unparseable_result: _unparseable_result().
  test_structure_boundary_classifies_as_language_unsupported.boundary: test_structure_boundary_classifies_as_language_unsupported().boundary().
  test_outline_does_not_mask_unparseable_language: test_outline_does_not_mask_unparseable_language().
  test_analyze_structure_does_not_mask_unparseable_language: test_analyze_structure_does_not_mask_unparseable_language().
  test_outline_cpp_in_py_file_surfaces_parse_errors: test_outline_cpp_in_py_file_surfaces_parse_errors().
  test_outline_cpp_in_py_agent_summary_warns: test_outline_cpp_in_py_agent_summary_warns().
  test_outline_nul_bytes_surfaces_encoding_warning: test_outline_nul_bytes_surfaces_encoding_warning().
  test_outline_nul_bytes_agent_summary_warns: test_outline_nul_bytes_agent_summary_warns().
  _patch_engine: _patch_engine().
  TARGET_FILE: TARGET_FILE.
  _patch_engine._fake_analyze: _patch_engine()._fake_analyze().
  test_structure_boundary_classifies_as_language_unsupported._fake_analyze: test_structure_boundary_classifies_as_language_unsupported()._fake_analyze().
  _CPP_CONTENT: _CPP_CONTENT.
  _PY_WITH_NUL: _PY_WITH_NUL.
---
# Module: [`tests/unit/mcp/test_structure_unparseable_language.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_structure_unparseable_language.py)

## Functions
- `_fake_analyze(_request)` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_structure_unparseable_language.py#L73)
- `_fake_analyze(_request)` — [`L137`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_structure_unparseable_language.py#L137)
- `_patch_engine(tool: object)` — [`L72`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_structure_unparseable_language.py#L72)
- `_unparseable_result()` — [`L61`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_structure_unparseable_language.py#L61) — The engine's honest output for a detected-but-unparseable language.
- `boundary(name: str, args: dict)` — [`L146`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_structure_unparseable_language.py#L146)
- `test_analyze_structure_does_not_mask_unparseable_language()` — [`L92`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_structure_unparseable_language.py#L92) — analyze (structure) must not report a failed parse as empty-success.
- `test_outline_cpp_in_py_agent_summary_warns(tmp_path)` — [`L202`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_structure_unparseable_language.py#L202) — #707: agent_summary also carries verdict=WARN for parse-error files.
- `test_outline_cpp_in_py_file_surfaces_parse_errors(tmp_path)` — [`L181`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_structure_unparseable_language.py#L181) — #707: C++ content in a .py file must set parse_errors=True, verdict=WARN.
- `test_outline_does_not_mask_unparseable_language()` — [`L80`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_structure_unparseable_language.py#L80) — get_code_outline must not report a failed parse as empty-success.
- `test_outline_nul_bytes_agent_summary_warns(tmp_path)` — [`L238`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_structure_unparseable_language.py#L238) — #707: agent_summary carries verdict=WARN + NUL-byte next_step for NUL files.
- `test_outline_nul_bytes_surfaces_encoding_warning(tmp_path)` — [`L219`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_structure_unparseable_language.py#L219) — #707: .py file with NUL bytes must set null_bytes=True, encoding_warning=True, verdict=WARN.
- `test_structure_boundary_classifies_as_language_unsupported()` — [`L102`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_structure_unparseable_language.py#L102) — The MCP boundary must surface an honest ``language_unsupported`` ERROR — documented in [tree_sitter_analyzer-mcp-server](../../../../concepts/tree_sitter_analyzer-mcp-server.md)

## Module values
- `TARGET_FILE` — [`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_structure_unparseable_language.py#L58)
- `_CPP_CONTENT` — [`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_structure_unparseable_language.py#L41)
- `_PY_WITH_NUL` — [`L54`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_structure_unparseable_language.py#L54)

