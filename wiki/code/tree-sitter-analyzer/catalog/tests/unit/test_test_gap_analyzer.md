---
title: 'Module: tests/unit/test_test_gap_analyzer.py'
type: catalog
provenance: extracted
module: tests/unit/test_test_gap_analyzer.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_test_gap_analyzer`/
symbols:
  _make_prod: _make_prod().
  TestAnalyzeCoverageGaps.test_gaps_have_priority: TestAnalyzeCoverageGaps#test_gaps_have_priority().
  TestAnalyzeCoverageGaps.test_finds_uncovered_symbols: TestAnalyzeCoverageGaps#test_finds_uncovered_symbols().
  TestAnalyzeCoverageGaps.test_empty_project: TestAnalyzeCoverageGaps#test_empty_project().
  TestPriorityScore.test_simple_function: TestPriorityScore#test_simple_function().
  TestPriorityScore.test_class_bonus: TestPriorityScore#test_class_bonus().
  TestPriorityScore.test_risk_bonus: TestPriorityScore#test_risk_bonus().
  TestMakeSuggestion.test_function: TestMakeSuggestion#test_function().
  TestMakeSuggestion.test_class: TestMakeSuggestion#test_class().
  TestMakeSuggestion.test_method: TestMakeSuggestion#test_method().
  TestMakeReason.test_function: TestMakeReason#test_function().
  TestMakeReason.test_class: TestMakeReason#test_class().
  TestMakeReason.test_high_complexity: TestMakeReason#test_high_complexity().
  TestAnalyzeCoverageGaps.test_coverage_percentage: TestAnalyzeCoverageGaps#test_coverage_percentage().
  TestAnalyzeCoverageGaps.test_language_filter: TestAnalyzeCoverageGaps#test_language_filter().
  TestAnalyzeCoverageGaps.test_max_gaps: TestAnalyzeCoverageGaps#test_max_gaps().
  TestAnalyzeCoverageGaps.test_include_covered: TestAnalyzeCoverageGaps#test_include_covered().
  TestAnalyzeCoverageGaps.test_summary_has_by_language: TestAnalyzeCoverageGaps#test_summary_has_by_language().
  TestAnalyzeCoverageGaps.test_summary_has_worst_files: TestAnalyzeCoverageGaps#test_summary_has_worst_files().
  TestIsTestFile.test_test_prefix: TestIsTestFile#test_test_prefix().
  TestIsTestFile.test_test_suffix: TestIsTestFile#test_test_suffix().
  TestIsTestFile.test_spec_suffix: TestIsTestFile#test_spec_suffix().
  TestIsTestFile.test_test_dir: TestIsTestFile#test_test_dir().
  TestIsTestFile.test_production_file: TestIsTestFile#test_production_file().
  TestIsTestFile.test_src_file: TestIsTestFile#test_src_file().
  TestExtractTestTargets.test_test_prefix: TestExtractTestTargets#test_test_prefix().
  TestExtractTestTargets.test_should_prefix: TestExtractTestTargets#test_should_prefix().
  TestExtractTestTargets.test_no_prefix: TestExtractTestTargets#test_no_prefix().
  TestExtractTestTargets.test_with_keyword: TestExtractTestTargets#test_with_keyword().
  TestRiskBand.test_low: TestRiskBand#test_low().
  TestRiskBand.test_medium: TestRiskBand#test_medium().
  TestRiskBand.test_high: TestRiskBand#test_high().
  TestRiskBand.test_critical: TestRiskBand#test_critical().
  TestIsTestFile: TestIsTestFile#
  TestExtractTestTargets: TestExtractTestTargets#
  TestRiskBand: TestRiskBand#
  TestPriorityScore: TestPriorityScore#
  TestMakeSuggestion: TestMakeSuggestion#
  TestMakeReason: TestMakeReason#
  TestAnalyzeCoverageGaps: TestAnalyzeCoverageGaps#
  TestAnalyzeCoverageGaps.project_with_gaps: TestAnalyzeCoverageGaps#project_with_gaps().
---
# Module: [`tests/unit/test_test_gap_analyzer.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_analyzer.py)

## Classes
### `TestAnalyzeCoverageGaps`
- def: [`tests/unit/test_test_gap_analyzer.py:143`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_analyzer.py#L143)
- signature: `class TestAnalyzeCoverageGaps:`
- members:
  - `project_with_gaps(self, tmp_path)` — [`L145`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_analyzer.py#L145)
  - `test_coverage_percentage(self, project_with_gaps)` — [`L169`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_analyzer.py#L169)
  - `test_empty_project(self, tmp_path)` — [`L193`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_analyzer.py#L193)
  - `test_finds_uncovered_symbols(self, project_with_gaps)` — [`L162`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_analyzer.py#L162)
  - `test_gaps_have_priority(self, project_with_gaps)` — [`L173`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_analyzer.py#L173)
  - `test_include_covered(self, project_with_gaps)` — [`L189`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_analyzer.py#L189)
  - `test_language_filter(self, project_with_gaps)` — [`L181`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_analyzer.py#L181)
  - `test_max_gaps(self, project_with_gaps)` — [`L185`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_analyzer.py#L185)
  - `test_summary_has_by_language(self, project_with_gaps)` — [`L199`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_analyzer.py#L199)
  - `test_summary_has_worst_files(self, project_with_gaps)` — [`L204`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_analyzer.py#L204)
- uses (calls/refs, reference-scoped): (13 test-only callers)

### `TestExtractTestTargets`
- def: [`tests/unit/test_test_gap_analyzer.py:53`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_analyzer.py#L53)
- signature: `class TestExtractTestTargets:`
- members:
  - `test_no_prefix(self)` — [`L63`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_analyzer.py#L63)
  - `test_should_prefix(self)` — [`L59`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_analyzer.py#L59)
  - `test_test_prefix(self)` — [`L54`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_analyzer.py#L54)
  - `test_with_keyword(self)` — [`L67`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_analyzer.py#L67)
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `TestIsTestFile`
- def: [`tests/unit/test_test_gap_analyzer.py:33`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_analyzer.py#L33)
- signature: `class TestIsTestFile:`
- members:
  - `test_production_file(self)` — [`L46`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_analyzer.py#L46)
  - `test_spec_suffix(self)` — [`L40`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_analyzer.py#L40)
  - `test_src_file(self)` — [`L49`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_analyzer.py#L49)
  - `test_test_dir(self)` — [`L43`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_analyzer.py#L43)
  - `test_test_prefix(self)` — [`L34`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_analyzer.py#L34)
  - `test_test_suffix(self)` — [`L37`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_analyzer.py#L37)
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `TestMakeReason`
- def: [`tests/unit/test_test_gap_analyzer.py:124`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_analyzer.py#L124)
- signature: `class TestMakeReason:`
- members:
  - `test_class(self)` — [`L131`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_analyzer.py#L131)
  - `test_function(self)` — [`L125`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_analyzer.py#L125)
  - `test_high_complexity(self)` — [`L137`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_analyzer.py#L137)
- uses (calls/refs, reference-scoped): (2 test-only callers)

### `TestMakeSuggestion`
- def: [`tests/unit/test_test_gap_analyzer.py:106`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_analyzer.py#L106)
- signature: `class TestMakeSuggestion:`
- members:
  - `test_class(self)` — [`L112`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_analyzer.py#L112)
  - `test_function(self)` — [`L107`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_analyzer.py#L107)
  - `test_method(self)` — [`L117`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_analyzer.py#L117)
- uses (calls/refs, reference-scoped): (2 test-only callers)

### `TestPriorityScore`
- def: [`tests/unit/test_test_gap_analyzer.py:89`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_analyzer.py#L89)
- signature: `class TestPriorityScore:`
- members:
  - `test_class_bonus(self)` — [`L95`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_analyzer.py#L95)
  - `test_risk_bonus(self)` — [`L100`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_analyzer.py#L100)
  - `test_simple_function(self)` — [`L90`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_analyzer.py#L90)
- uses (calls/refs, reference-scoped): (2 test-only callers)

### `TestRiskBand`
- def: [`tests/unit/test_test_gap_analyzer.py:72`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_analyzer.py#L72)
- signature: `class TestRiskBand:`
- members:
  - `test_critical(self)` — [`L85`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_analyzer.py#L85)
  - `test_high(self)` — [`L81`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_analyzer.py#L81)
  - `test_low(self)` — [`L73`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_analyzer.py#L73)
  - `test_medium(self)` — [`L77`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_analyzer.py#L77)
- uses (calls/refs, reference-scoped): (1 test-only callers)

## Functions
- `_make_prod(name, kind="function", **kw)` — [`L19`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_test_gap_analyzer.py#L19)

