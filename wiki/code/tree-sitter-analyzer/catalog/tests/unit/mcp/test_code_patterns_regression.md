---
title: 'Module: tests/unit/mcp/test_code_patterns_regression.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_code_patterns_regression.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_code_patterns_regression`/Test
symbols:
  TestCrossLanguageSmellDetection.test_code_patterns_long_method_js: CrossLanguageSmellDetection#test_code_patterns_long_method_js().
  TestCrossLanguageSmellDetection.test_code_patterns_god_class_js: CrossLanguageSmellDetection#test_code_patterns_god_class_js().
  TestG3SqlInjectionFalsePositives.test_g3_fp_please_update_call_sites: G3SqlInjectionFalsePositives#test_g3_fp_please_update_call_sites().
  TestG3SqlInjectionFalsePositives.test_g3_fp_drop_this_approach: G3SqlInjectionFalsePositives#test_g3_fp_drop_this_approach().
  TestG3SqlInjectionFalsePositives.test_g3_tp_select_from_users: G3SqlInjectionFalsePositives#test_g3_tp_select_from_users().
  TestG3SqlInjectionFalsePositives.test_g3_tp_insert_into_logs: G3SqlInjectionFalsePositives#test_g3_tp_insert_into_logs().
  TestG4NoDuplicateFindings.test_g4_sql_injection_appears_once: G4NoDuplicateFindings#test_g4_sql_injection_appears_once().
  TestG4NoDuplicateFindings.test_g4_count_matches_results_length: G4NoDuplicateFindings#test_g4_count_matches_results_length().
  TestG4NoDuplicateFindings.test_g4_dedup_does_not_swallow_non_security_smells: G4NoDuplicateFindings#test_g4_dedup_does_not_swallow_non_security_smells().
  TestCrossLanguageSmellDetection: CrossLanguageSmellDetection#
  TestG3SqlInjectionFalsePositives: G3SqlInjectionFalsePositives#
  TestG4NoDuplicateFindings: G4NoDuplicateFindings#
---
# Module: [`tests/unit/mcp/test_code_patterns_regression.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_regression.py)

## Classes
### `TestCrossLanguageSmellDetection`
- def: [`tests/unit/mcp/test_code_patterns_regression.py:18`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_regression.py#L18)
- signature: `class TestCrossLanguageSmellDetection:`
- members:
  - `test_code_patterns_god_class_js(self, tmp_path)` — [`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_regression.py#L51) — Bug M5 regression: a single 300+ line JS class MUST surface as god_class.
  - `test_code_patterns_long_method_js(self, tmp_path)` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_regression.py#L20) — Bug H1 regression: a 100+ line JS function MUST surface as long_method.
- uses (calls/refs, reference-scoped): [`execute`](../../../tree_sitter_analyzer/mcp/tools/code_patterns_tool.md#CodePatternsTool.execute), [`CodePatternsTool`](../../../tree_sitter_analyzer/mcp/tools/code_patterns_tool.md#CodePatternsTool)

### `TestG3SqlInjectionFalsePositives`
- def: [`tests/unit/mcp/test_code_patterns_regression.py:92`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_regression.py#L92)
- signature: `class TestG3SqlInjectionFalsePositives:`
- members:
  - `test_g3_fp_drop_this_approach(self, tmp_path)` — [`L120`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_regression.py#L120) — ``DROP this approach`` is figurative, not a DROP TABLE.
  - `test_g3_fp_please_update_call_sites(self, tmp_path)` — [`L94`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_regression.py#L94) — ``Please update {n} call sites`` is English, not SQL.
  - `test_g3_tp_insert_into_logs(self, tmp_path)` — [`L174`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_regression.py#L174) — Real INSERT with INTO clause MUST be flagged.
  - `test_g3_tp_select_from_users(self, tmp_path)` — [`L146`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_regression.py#L146) — Real SQL with FROM clause MUST be flagged.
- uses (calls/refs, reference-scoped): [`execute`](../../../tree_sitter_analyzer/mcp/tools/code_patterns_tool.md#CodePatternsTool.execute), [`CodePatternsTool`](../../../tree_sitter_analyzer/mcp/tools/code_patterns_tool.md#CodePatternsTool)

### `TestG4NoDuplicateFindings`
- def: [`tests/unit/mcp/test_code_patterns_regression.py:212`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_regression.py#L212)
- signature: `class TestG4NoDuplicateFindings:`
- members:
  - `test_g4_count_matches_results_length(self, tmp_path)` — [`L244`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_regression.py#L244) — ``count`` must equal ``len(results)`` after dedup.
  - `test_g4_dedup_does_not_swallow_non_security_smells(self, tmp_path)` — [`L265`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_regression.py#L265) — Dedup must only target the security mirror, not real smells.
  - `test_g4_sql_injection_appears_once(self, tmp_path)` — [`L214`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_code_patterns_regression.py#L214) — A single SQL-injection line yields exactly one ``results`` entry.
- uses (calls/refs, reference-scoped): [`execute`](../../../tree_sitter_analyzer/mcp/tools/code_patterns_tool.md#CodePatternsTool.execute), [`CodePatternsTool`](../../../tree_sitter_analyzer/mcp/tools/code_patterns_tool.md#CodePatternsTool)

