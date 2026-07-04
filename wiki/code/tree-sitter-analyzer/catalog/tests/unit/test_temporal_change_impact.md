---
title: 'Module: tests/unit/test_temporal_change_impact.py'
type: catalog
provenance: extracted
module: tests/unit/test_temporal_change_impact.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_temporal_change_impact`/
symbols:
  TestHotZoneBumpsVerdict.test_hot_zone_bumps_verdict_to_caution: TestHotZoneBumpsVerdict#test_hot_zone_bumps_verdict_to_caution().
  test_module_imports_cleanly: test_module_imports_cleanly().
  indexed_relation_project: indexed_relation_project().
  _init_git_repo: _init_git_repo().
  callees_tool: callees_tool().
  _SAMPLE_PY: _SAMPLE_PY.
  _make_git_repo_path: _make_git_repo_path().
  _seed_hot_zone_row: _seed_hot_zone_row().
  _first_symbol_row: _first_symbol_row().
  _read_one_row: _read_one_row().
  _collect_risk_reason_strings: _collect_risk_reason_strings().
  _PROJECT_ROOT: _PROJECT_ROOT.
  PROJECT_ROOT: PROJECT_ROOT.
  TestHotZoneBumpsVerdict: TestHotZoneBumpsVerdict#
  TestCalleesActivationFlag: TestCalleesActivationFlag#
  TestCalleesActivationFlag.test_callees_tool_includes_activation_when_requested: TestCalleesActivationFlag#test_callees_tool_includes_activation_when_requested().
  TestCalleesActivationFlag.test_callees_tool_omits_activation_by_default: TestCalleesActivationFlag#test_callees_tool_omits_activation_by_default().
---
# Module: [`tests/unit/test_temporal_change_impact.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_temporal_change_impact.py)

## Classes
### `TestCalleesActivationFlag`
- def: [`tests/unit/test_temporal_change_impact.py:306`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_temporal_change_impact.py#L306)
- signature: `class TestCalleesActivationFlag:`
- members:
  - `test_callees_tool_includes_activation_when_requested(self, callees_tool)` — [`L308`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_temporal_change_impact.py#L308) — With ``include_activation=True`` every callee entry must expose
  - `test_callees_tool_omits_activation_by_default(self, callees_tool)` — [`L339`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_temporal_change_impact.py#L339) — Without the flag the response is byte-for-byte the legacy shape —

### `TestHotZoneBumpsVerdict`
- def: [`tests/unit/test_temporal_change_impact.py:178`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_temporal_change_impact.py#L178)
- signature: `class TestHotZoneBumpsVerdict:`
- members:
  - `test_hot_zone_bumps_verdict_to_caution(self, tmp_path, monkeypatch)` — [`L181`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_temporal_change_impact.py#L181) — A symbol with ``mod_count_30d >= 5`` in a CHANGED file must:
- uses (calls/refs, reference-scoped): [`ASTCache`](../../tree_sitter_analyzer/ast_cache.md#ASTCache), [`close`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.close), [`execute`](../../tree_sitter_analyzer/mcp/tools/change_impact_tool.md#ChangeImpactTool.execute), [`index_file`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.index_file), [`ChangeImpactTool`](../../tree_sitter_analyzer/mcp/tools/change_impact_tool.md#ChangeImpactTool), [`db_path`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.db_path)  (7 test-only)

## Functions
- `_collect_risk_reason_strings(result: dict)` — [`L254`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_temporal_change_impact.py#L254) — Walk the change-impact response and harvest any 'reason' strings.
- `_first_symbol_row(db_path: str, file_path: str)` — [`L151`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_temporal_change_impact.py#L151) — Return the smallest symbol id and stored path for ``file_path``.
- `_init_git_repo(repo: Path)` — [`L52`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_temporal_change_impact.py#L52) — Initialise a git repo inside ``repo`` with a single commit.
- `_make_git_repo_path(tmp_path: Path)` — [`L83`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_temporal_change_impact.py#L83) — Create a git repo under pytest's tmp_path for automatic cleanup.
- `_read_one_row(db_path: str, table: str)` — [`L239`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_temporal_change_impact.py#L239) — Return one row from ``table`` as dict, or None.
- `_seed_hot_zone_row(db_path: str, *, file_path: str, symbol_id: int, mod_count_30d: int)` — [`L90`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_temporal_change_impact.py#L90) — Insert (or upsert) a fake ``ast_symbol_activation`` row.
- `callees_tool(indexed_relation_project: str)` — [`L302`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_temporal_change_impact.py#L302)
- `indexed_relation_project(tmp_path: Path)` — [`L284`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_temporal_change_impact.py#L284)
- `test_module_imports_cleanly()` — [`L362`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_temporal_change_impact.py#L362) — Defensive: importing this test file must NOT itself raise.

## Module values
- `PROJECT_ROOT` — [`L35`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_temporal_change_impact.py#L35)
- `_PROJECT_ROOT` — [`L280`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_temporal_change_impact.py#L280)
- `_SAMPLE_PY` — [`L43`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_temporal_change_impact.py#L43)

