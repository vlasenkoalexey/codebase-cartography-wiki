---
title: 'Module: tests/unit/test_file_health_smells.py'
type: catalog
provenance: extracted
module: tests/unit/test_file_health_smells.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_file_health_smells`/Test
symbols:
  TestDetectCodeSmells.test_returns_list: DetectCodeSmells#test_returns_list().
  TestDetectCodeSmells.test_unreadable_file_returns_empty: DetectCodeSmells#test_unreadable_file_returns_empty().
  TestDetectCodeSmells.test_healthy_file_no_smells: DetectCodeSmells#test_healthy_file_no_smells().
  TestCheckOversizedFile.test_small_file_no_smell: CheckOversizedFile#test_small_file_no_smell().
  TestCheckOversizedFile.test_medium_file_warning: CheckOversizedFile#test_medium_file_warning().
  TestCheckOversizedFile.test_huge_file_critical: CheckOversizedFile#test_huge_file_critical().
  TestCheckOversizedFile.test_exact_threshold_no_smell: CheckOversizedFile#test_exact_threshold_no_smell().
  TestCheckDeepNesting.test_shallow_code_no_smell: CheckDeepNesting#test_shallow_code_no_smell().
  TestCheckDeepNesting.test_deep_nesting_warning: CheckDeepNesting#test_deep_nesting_warning().
  TestCheckGodClass.test_no_class_no_smell: CheckGodClass#test_no_class_no_smell().
  TestCheckGodClass.test_multiple_classes_no_smell: CheckGodClass#test_multiple_classes_no_smell().
  TestCheckGodClass.test_single_huge_class_critical: CheckGodClass#test_single_huge_class_critical().
  TestCheckGodClass.test_single_class_under_threshold: CheckGodClass#test_single_class_under_threshold().
  TestCheckLongFunctions.test_short_function_no_smell: CheckLongFunctions#test_short_function_no_smell().
  TestCheckLongFunctions.test_long_function_warning: CheckLongFunctions#test_long_function_warning().
  TestCheckLongFunctions.test_very_long_function_critical: CheckLongFunctions#test_very_long_function_critical().
  TestTechnicalDebtDetection.test_detects_markers: TechnicalDebtDetection#test_detects_markers().
  TestTechnicalDebtDetection.test_ignores_non_markers: TechnicalDebtDetection#test_ignores_non_markers().
  TestTechnicalDebtDetection.test_comment_text_extracts_comment: TechnicalDebtDetection#test_comment_text_extracts_comment().
  TestTechnicalDebtDetection.test_comment_text_no_comment: TechnicalDebtDetection#test_comment_text_no_comment().
  TestCheckTechnicalDebt.test_few_markers_no_smell: CheckTechnicalDebt#test_few_markers_no_smell().
  TestCheckTechnicalDebt.test_many_markers_triggers_smell: CheckTechnicalDebt#test_many_markers_triggers_smell().
  TestCheckElementSmells.test_no_analysis_uses_heuristic: CheckElementSmells#test_no_analysis_uses_heuristic().
  TestCheckElementSmells.test_with_analysis_checks_classes_and_functions: CheckElementSmells#test_with_analysis_checks_classes_and_functions().
  TestDetectCodeSmells: DetectCodeSmells#
  TestCheckOversizedFile: CheckOversizedFile#
  TestCheckDeepNesting: CheckDeepNesting#
  TestCheckGodClass: CheckGodClass#
  TestCheckLongFunctions: CheckLongFunctions#
  TestTechnicalDebtDetection: TechnicalDebtDetection#
  TestCheckTechnicalDebt: CheckTechnicalDebt#
  TestCheckElementSmells: CheckElementSmells#
---
# Module: [`tests/unit/test_file_health_smells.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_health_smells.py)

## Classes
### `TestCheckDeepNesting`
- def: [`tests/unit/test_file_health_smells.py:86`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_health_smells.py#L86)
- signature: `class TestCheckDeepNesting:`
- members:
  - `test_deep_nesting_warning(self)` — [`L92`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_health_smells.py#L92)
  - `test_shallow_code_no_smell(self)` — [`L87`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_health_smells.py#L87)
- uses (calls/refs, reference-scoped): [`_check_deep_nesting`](../../tree_sitter_analyzer/mcp/tools/utils/file_health_smells.md#_check_deep_nesting)

### `TestCheckElementSmells`
- def: [`tests/unit/test_file_health_smells.py:216`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_health_smells.py#L216)
- signature: `class TestCheckElementSmells:`
- members:
  - `test_no_analysis_uses_heuristic(self)` — [`L217`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_health_smells.py#L217) — When analysis is None, heuristic long-method detection runs.
  - `test_with_analysis_checks_classes_and_functions(self)` — [`L225`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_health_smells.py#L225) — When analysis is provided, god_class and long_method checks run.
- uses (calls/refs, reference-scoped): [`_check_element_smells`](../../tree_sitter_analyzer/mcp/tools/utils/file_health_smells.md#_check_element_smells)

### `TestCheckGodClass`
- def: [`tests/unit/test_file_health_smells.py:104`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_health_smells.py#L104)
- signature: `class TestCheckGodClass:`
- members:
  - `test_multiple_classes_no_smell(self)` — [`L110`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_health_smells.py#L110)
  - `test_no_class_no_smell(self)` — [`L105`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_health_smells.py#L105)
  - `test_single_class_under_threshold(self)` — [`L127`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_health_smells.py#L127)
  - `test_single_huge_class_critical(self)` — [`L119`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_health_smells.py#L119)
- uses (calls/refs, reference-scoped): [`_check_god_class`](../../tree_sitter_analyzer/mcp/tools/utils/file_health_smells.md#_check_god_class)

### `TestCheckLongFunctions`
- def: [`tests/unit/test_file_health_smells.py:139`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_health_smells.py#L139)
- signature: `class TestCheckLongFunctions:`
- members:
  - `test_long_function_warning(self)` — [`L146`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_health_smells.py#L146)
  - `test_short_function_no_smell(self)` — [`L140`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_health_smells.py#L140)
  - `test_very_long_function_critical(self)` — [`L153`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_health_smells.py#L153)
- uses (calls/refs, reference-scoped): [`_check_long_functions`](../../tree_sitter_analyzer/mcp/tools/utils/file_health_smells.md#_check_long_functions)

### `TestCheckOversizedFile`
- def: [`tests/unit/test_file_health_smells.py:56`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_health_smells.py#L56)
- signature: `class TestCheckOversizedFile:`
- members:
  - `test_exact_threshold_no_smell(self)` — [`L75`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_health_smells.py#L75)
  - `test_huge_file_critical(self)` — [`L68`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_health_smells.py#L68)
  - `test_medium_file_warning(self)` — [`L62`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_health_smells.py#L62)
  - `test_small_file_no_smell(self)` — [`L57`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_health_smells.py#L57)
- uses (calls/refs, reference-scoped): [`_check_oversized_file`](../../tree_sitter_analyzer/mcp/tools/utils/file_health_smells.md#_check_oversized_file)

### `TestCheckTechnicalDebt`
- def: [`tests/unit/test_file_health_smells.py:197`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_health_smells.py#L197)
- signature: `class TestCheckTechnicalDebt:`
- members:
  - `test_few_markers_no_smell(self)` — [`L198`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_health_smells.py#L198)
  - `test_many_markers_triggers_smell(self)` — [`L204`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_health_smells.py#L204)
- uses (calls/refs, reference-scoped): [`_check_technical_debt`](../../tree_sitter_analyzer/mcp/tools/utils/file_health_smells.md#_check_technical_debt)

### `TestDetectCodeSmells`
- def: [`tests/unit/test_file_health_smells.py:26`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_health_smells.py#L26)
- signature: `class TestDetectCodeSmells:`
- members:
  - `test_healthy_file_no_smells(self, tmp_path)` — [`L39`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_health_smells.py#L39) — Small, well-structured file should produce minimal smells.
  - `test_returns_list(self, tmp_path)` — [`L27`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_health_smells.py#L27) — Should always return a list, even for empty files.
  - `test_unreadable_file_returns_empty(self, tmp_path)` — [`L34`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_health_smells.py#L34) — File that raises on read should return empty list.
- uses (calls/refs, reference-scoped): [`detect_code_smells`](../../tree_sitter_analyzer/mcp/tools/utils/file_health_smells.md#detect_code_smells)

### `TestTechnicalDebtDetection`
- def: [`tests/unit/test_file_health_smells.py:165`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_health_smells.py#L165)
- signature: `class TestTechnicalDebtDetection:`
- members:
  - `test_comment_text_extracts_comment(self)` — [`L190`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_health_smells.py#L190)
  - `test_comment_text_no_comment(self)` — [`L193`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_health_smells.py#L193)
  - `test_detects_markers(self, line: str)` — [`L175`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_health_smells.py#L175)
  - `test_ignores_non_markers(self, line: str)` — [`L187`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_file_health_smells.py#L187)
- uses (calls/refs, reference-scoped): [`_has_technical_debt_marker`](../../tree_sitter_analyzer/mcp/tools/utils/file_health_smells.md#_has_technical_debt_marker), [`_comment_text`](../../tree_sitter_analyzer/mcp/tools/utils/file_health_smells.md#_comment_text)

