---
title: 'Module: tree_sitter_analyzer/mcp/tools/nav_facade.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/nav_facade.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.nav_facade`/
symbols:
  build_nav_facade: build_nav_facade().
  build_nav_facade._test_map_route: build_nav_facade()._test_map_route().
  _is_collectible_caller: _is_collectible_caller().
  build_nav_facade._co_change_route: build_nav_facade()._co_change_route().
  _is_js_test_func: _is_js_test_func().
  _is_go_test_func: _is_go_test_func().
  build_nav_facade._callers_route: build_nav_facade()._callers_route().
  build_nav_facade._callees_route: build_nav_facade()._callees_route().
  _MAX_TEST_MAP: _MAX_TEST_MAP.
  _NAV_DESCRIPTION: _NAV_DESCRIPTION.
  build_nav_facade._test_map_route._record_edge: build_nav_facade()._test_map_route()._record_edge().
  _is_java_test_method: _is_java_test_method().
  build_nav_facade._context_route: build_nav_facade()._context_route().
  _is_pytest_collectible: _is_pytest_collectible().
  _is_python_file: _is_python_file().
  _test_map_next_step: _test_map_next_step().
  build_nav_facade._test_map_route._add_to_set: build_nav_facade()._test_map_route()._add_to_set().
  _NAV_ANNOTATIONS._NAV_ANNOTATIONS: _NAV_ANNOTATIONS._NAV_ANNOTATIONS.
---
# Module: [`tree_sitter_analyzer/mcp/tools/nav_facade.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/nav_facade.py)

## Functions
- `_add_to_set(file_path: str, name: str)` — [`L450`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/nav_facade.py#L450)
- `_callees_route(args: dict[str, Any])` — [`L376`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/nav_facade.py#L376) — R4: scope=point → direct callees; scope=graph → call-graph traversal.
- `_callers_route(args: dict[str, Any])` — [`L355`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/nav_facade.py#L355) — R4: scope=point → direct callers; scope=graph → call-graph traversal.
- `_co_change_route(args: dict[str, Any])` — [`L530`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/nav_facade.py#L530) — RFC-0014 Phase C: git-history co-change coupling.
- `_context_route(args: dict[str, Any])` — [`L325`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/nav_facade.py#L325) — Bespoke context route: normalize symbol/query → task (fix ③).
- `_is_collectible_caller(file_path: str, name: str, language: str = "")` — [`L133`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/nav_facade.py#L133) — Decide whether a test-file caller is an accepted test entry point.
- `_is_go_test_func(name: str)` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/nav_facade.py#L73) — True for Go test entry points: ``TestXxx``/``BenchmarkXxx``/``ExampleXxx``/``FuzzXxx``.
- `_is_java_test_method(name: str)` — [`L114`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/nav_facade.py#L114) — Heuristic for JUnit test methods (annotation-based, no name rule).
- `_is_js_test_func(name: str)` — [`L92`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/nav_facade.py#L92) — Heuristic for JS/TS test functions inside a test file.
- `_is_pytest_collectible(name: str)` — [`L54`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/nav_facade.py#L54) — Return True only for pytest-collectible function/method names.
- `_is_python_file(file_path: str)` — [`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/nav_facade.py#L68) — True for Python source files (where the pytest ``test_`` rule applies).
- `_record_edge(target: Any, file_path: str, name: str)` — [`L457`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/nav_facade.py#L457) — Count one (target → test) coverage edge, deduped per target.
- `_test_map_next_step(test_files: list[str], *, listed_function_count: int, unique_function_count: int, truncated: bool)` — [`L168`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/nav_facade.py#L168) — Build an honest next step for ``nav action=test_map``.
- `_test_map_route(args: dict[str, Any])` — [`L395`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/nav_facade.py#L395) — RFC-0014 Phase B: which tests exercise a function?
- `build_nav_facade(project_root: str | None = None)` — [`L282`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/nav_facade.py#L282) — Construct the ``nav`` facade wired to live inner tool instances. — documented in [tree_sitter_analyzer-mcp-tools-facade_tool](../../../../concepts/tree_sitter_analyzer-mcp-tools-facade_tool.md)

## Module values
- `_MAX_TEST_MAP` — [`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/nav_facade.py#L51)
- `_NAV_ANNOTATIONS` — [`L200`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/nav_facade.py#L200)
- `_NAV_DESCRIPTION` — [`L207`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/nav_facade.py#L207)

