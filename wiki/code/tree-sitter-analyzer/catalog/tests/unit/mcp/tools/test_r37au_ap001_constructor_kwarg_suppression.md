---
title: 'Module: tests/unit/mcp/tools/test_r37au_ap001_constructor_kwarg_suppression.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/tools/test_r37au_ap001_constructor_kwarg_suppression.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.tools.test_r37au_ap001_constructor_kwarg_suppression`/
symbols:
  _ids: _ids().
  TestAP001ConstructorCallsClean.test_constructor_kwarg_empty_list_is_not_ap001: TestAP001ConstructorCallsClean#test_constructor_kwarg_empty_list_is_not_ap001().
  TestAP001ConstructorCallsClean.test_function_call_kwarg_empty_dict_is_not_ap001: TestAP001ConstructorCallsClean#test_function_call_kwarg_empty_dict_is_not_ap001().
  TestAP001ConstructorCallsClean.test_local_variable_assignment_is_not_ap001: TestAP001ConstructorCallsClean#test_local_variable_assignment_is_not_ap001().
  TestAP001RealDefaultsStillDetected.test_real_mutable_default_at_def: TestAP001RealDefaultsStillDetected#test_real_mutable_default_at_def().
  TestAP001RealDefaultsStillDetected.test_keyword_only_mutable_default_detected: TestAP001RealDefaultsStillDetected#test_keyword_only_mutable_default_detected().
  TestAP001RealDefaultsStillDetected.test_async_function_default_detected: TestAP001RealDefaultsStillDetected#test_async_function_default_detected().
  TestAP001ConstructorCallsClean: TestAP001ConstructorCallsClean#
  TestAP001RealDefaultsStillDetected: TestAP001RealDefaultsStillDetected#
  test_sql_formatter_helper_self_scan: test_sql_formatter_helper_self_scan().
---
# Module: [`tests/unit/mcp/tools/test_r37au_ap001_constructor_kwarg_suppression.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_r37au_ap001_constructor_kwarg_suppression.py)

## Classes
### `TestAP001ConstructorCallsClean`
- def: [`tests/unit/mcp/tools/test_r37au_ap001_constructor_kwarg_suppression.py:32`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_r37au_ap001_constructor_kwarg_suppression.py#L32)
- doc: The 11 false positives in _sql_formatter_wrapper_helpers.py all
- signature: `class TestAP001ConstructorCallsClean:`
- members:
  - `test_constructor_kwarg_empty_list_is_not_ap001(self, tmp_path: Path)` — [`L37`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_r37au_ap001_constructor_kwarg_suppression.py#L37)
  - `test_function_call_kwarg_empty_dict_is_not_ap001(self, tmp_path: Path)` — [`L56`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_r37au_ap001_constructor_kwarg_suppression.py#L56)
  - `test_local_variable_assignment_is_not_ap001(self, tmp_path: Path)` — [`L71`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_r37au_ap001_constructor_kwarg_suppression.py#L71)
- uses (calls/refs, reference-scoped): [`detect_anti_patterns`](../../../../tree_sitter_analyzer/mcp/tools/utils/anti_patterns.md#detect_anti_patterns)  (1 test-only)

### `TestAP001RealDefaultsStillDetected`
- def: [`tests/unit/mcp/tools/test_r37au_ap001_constructor_kwarg_suppression.py:84`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_r37au_ap001_constructor_kwarg_suppression.py#L84)
- doc: The AST-based detector must still catch real bugs.
- signature: `class TestAP001RealDefaultsStillDetected:`
- members:
  - `test_async_function_default_detected(self, tmp_path: Path)` — [`L119`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_r37au_ap001_constructor_kwarg_suppression.py#L119)
  - `test_keyword_only_mutable_default_detected(self, tmp_path: Path)` — [`L109`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_r37au_ap001_constructor_kwarg_suppression.py#L109) — Keyword-only ``def f(*, x=[])`` defaults live in kw_defaults.
  - `test_real_mutable_default_at_def(self, tmp_path: Path, default_literal: str)` — [`L91`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_r37au_ap001_constructor_kwarg_suppression.py#L91)
- uses (calls/refs, reference-scoped): [`detect_anti_patterns`](../../../../tree_sitter_analyzer/mcp/tools/utils/anti_patterns.md#detect_anti_patterns)  (1 test-only)

## Functions
- `_ids(findings: list[dict[str, object]])` — [`L28`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_r37au_ap001_constructor_kwarg_suppression.py#L28)
- `test_sql_formatter_helper_self_scan()` — [`L130`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_r37au_ap001_constructor_kwarg_suppression.py#L130) — End-to-end: scan the file that prompted r37au — 11 false positives

