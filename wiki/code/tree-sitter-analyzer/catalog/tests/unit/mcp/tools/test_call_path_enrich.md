---
title: 'Module: tests/unit/mcp/tools/test_call_path_enrich.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/tools/test_call_path_enrich.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.tools.test_call_path_enrich`/
symbols:
  _build_cache: _build_cache().
  _run_tool: _run_tool().
  test_inline_path_bodies_returns_verbatim_bodies: test_inline_path_bodies_returns_verbatim_bodies().
  test_inline_path_bodies_dedupes: test_inline_path_bodies_dedupes().
  test_body_truncation_caps_lines: test_body_truncation_caps_lines().
  test_build_dead_end_inlines_both_endpoints: test_build_dead_end_inlines_both_endpoints().
  test_tool_path_found_inlines_bodies_and_deterrent: test_tool_path_found_inlines_bodies_and_deterrent().
  test_tool_dead_end_inlines_endpoints_and_deterrent: test_tool_dead_end_inlines_endpoints_and_deterrent().
  test_tool_toon_format_carries_bodies: test_tool_toon_format_carries_bodies().
  test_inline_path_bodies_cpp_header_callee_lang_hint: test_inline_path_bodies_cpp_header_callee_lang_hint().
  test_inline_path_bodies_cpp_with_explicit_h_callee_file: test_inline_path_bodies_cpp_with_explicit_h_callee_file().
  _EDGES: _EDGES.
  _SRC_A: _SRC_A.
  _SRC_B: _SRC_B.
  _SRC_C: _SRC_C.
  _SYMBOLS: _SYMBOLS.
  _build_cache._callers: _build_cache()._callers().
  _build_cache._callees: _build_cache()._callees().
---
# Module: [`tests/unit/mcp/tools/test_call_path_enrich.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_call_path_enrich.py)

## Functions
- `_build_cache(tmp_path: Path)` — [`L64`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_call_path_enrich.py#L64) — Build a fixture cache with ast_call_edges + ast_index + real files.
- `_callees(name, file=None, depth=1)` — [`L160`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_call_path_enrich.py#L160)
- `_callers(name, file=None, depth=1)` — [`L152`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_call_path_enrich.py#L152)
- `_run_tool(tmp_path, cache, args)` — [`L398`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_call_path_enrich.py#L398)
- `test_body_truncation_caps_lines(tmp_path, monkeypatch)` — [`L351`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_call_path_enrich.py#L351)
- `test_build_dead_end_inlines_both_endpoints(tmp_path)` — [`L380`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_call_path_enrich.py#L380)
- `test_inline_path_bodies_cpp_header_callee_lang_hint(tmp_path)` — [`L210`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_call_path_enrich.py#L210) — #865: .h callee must not gate out C++ caller definitions.
- `test_inline_path_bodies_cpp_with_explicit_h_callee_file(tmp_path)` — [`L272`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_call_path_enrich.py#L272) — .h as explicit callee_file must not gate out C++ caller definitions (#865 P2).
- `test_inline_path_bodies_dedupes(tmp_path)` — [`L334`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_call_path_enrich.py#L334)
- `test_inline_path_bodies_returns_verbatim_bodies(tmp_path)` — [`L178`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_call_path_enrich.py#L178)
- `test_tool_dead_end_inlines_endpoints_and_deterrent(tmp_path)` — [`L434`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_call_path_enrich.py#L434)
- `test_tool_path_found_inlines_bodies_and_deterrent(tmp_path)` — [`L410`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_call_path_enrich.py#L410)
- `test_tool_toon_format_carries_bodies(tmp_path)` — [`L457`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_call_path_enrich.py#L457)

## Module values
- `_EDGES` — [`L37`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_call_path_enrich.py#L37)
- `_SRC_A` — [`L21`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_call_path_enrich.py#L21)
- `_SRC_B` — [`L27`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_call_path_enrich.py#L27)
- `_SRC_C` — [`L33`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_call_path_enrich.py#L33)
- `_SYMBOLS` — [`L57`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_call_path_enrich.py#L57)

