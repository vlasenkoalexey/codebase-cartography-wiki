---
title: 'Module: tests/integration/formatters/comprehensive_test_suite.py'
type: catalog
provenance: extracted
module: tests/integration/formatters/comprehensive_test_suite.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.formatters.comprehensive_test_suite`/
symbols:
  ComprehensiveFormatTestSuite.run_comprehensive_tests: ComprehensiveFormatTestSuite#run_comprehensive_tests().
  run_regression_test_suite: run_regression_test_suite().
  run_quick_format_validation: run_quick_format_validation().
  ComprehensiveFormatTestSuite.config: ComprehensiveFormatTestSuite#config.
  ComprehensiveFormatTestSuite.results_dir: ComprehensiveFormatTestSuite#results_dir.
  ComprehensiveFormatTestSuite: ComprehensiveFormatTestSuite#
  _ensure_config_defaults: _ensure_config_defaults().
  ComprehensiveFormatTestSuite.test_data_manager: ComprehensiveFormatTestSuite#test_data_manager.
  run_full_validation_suite: run_full_validation_suite().
  run_enabled_phases: run_enabled_phases().
  ComprehensiveFormatTestSuite.golden_master_tester: ComprehensiveFormatTestSuite#golden_master_tester.
  ComprehensiveFormatTestSuite.json_validator: ComprehensiveFormatTestSuite#json_validator.
  ComprehensiveFormatTestSuite.enhanced_assertions: ComprehensiveFormatTestSuite#enhanced_assertions.
  ComprehensiveFormatTestSuite.real_implementation_validation: ComprehensiveFormatTestSuite#real_implementation_validation.
  ComprehensiveSuiteDataMixin._prepare_test_data: ComprehensiveSuiteDataMixin#_prepare_test_data().
  ComprehensiveFormatTestSuite._initialize_test_components: ComprehensiveFormatTestSuite#_initialize_test_components().
  ComprehensiveFormatTestSuite.golden_master_manager: ComprehensiveFormatTestSuite#golden_master_manager.
  ComprehensiveFormatTestSuite.performance_tester: ComprehensiveFormatTestSuite#performance_tester.
  ComprehensiveSuiteDataMixin: ComprehensiveSuiteDataMixin#
  ComprehensiveSuiteDataMixin._load_created_test_data: ComprehensiveSuiteDataMixin#_load_created_test_data().
  ComprehensiveFormatTestSuite.__init__: ComprehensiveFormatTestSuite#__init__().
  ComprehensiveFormatTestSuite.markdown_validator: ComprehensiveFormatTestSuite#markdown_validator.
  ComprehensiveFormatTestSuite.csv_validator: ComprehensiveFormatTestSuite#csv_validator.
  ComprehensiveFormatTestSuite.table_format_integration: ComprehensiveFormatTestSuite#table_format_integration.
  ComprehensiveFormatTestSuite.format_consistency: ComprehensiveFormatTestSuite#format_consistency.
  PHASES: PHASES.
  _test_data_set_source: _test_data_set_source().
  _default_python_test_data: _default_python_test_data().
  __all__: __all__.
---
# Module: [`tests/integration/formatters/comprehensive_test_suite.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/comprehensive_test_suite.py)

## Classes
### `ComprehensiveFormatTestSuite`  ·  implements/extends ComprehensiveSuiteDataMixin, ComprehensiveSuitePhasesMixin
- def: [`tests/integration/formatters/comprehensive_test_suite.py:160`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/comprehensive_test_suite.py#L160)
- doc: Main comprehensive format testing suite
- signature: `class ComprehensiveFormatTestSuite(ComprehensiveSuiteDataMixin, ComprehensiveSuitePhasesMixin):`
- members:
  - `_initialize_test_components(self)` — [`L174`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/comprehensive_test_suite.py#L174) — Initialize all test components
  - `run_comprehensive_tests(self, analyzer_function: callable, test_data_sources: list[dict[str, Any]] | None = None)` — [`L209`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/comprehensive_test_suite.py#L209) — Run comprehensive format testing suite
  - `config` — [`L166`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/comprehensive_test_suite.py#L166)
  - `csv_validator` — [`L186`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/comprehensive_test_suite.py#L186)
  - `enhanced_assertions` — [`L190`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/comprehensive_test_suite.py#L190)
  - `format_consistency` — [`L195`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/comprehensive_test_suite.py#L195)
  - `golden_master_manager` — [`L179`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/comprehensive_test_suite.py#L179)
  - `golden_master_tester` — [`L182`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/comprehensive_test_suite.py#L182)
  - `json_validator` — [`L187`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/comprehensive_test_suite.py#L187)
  - `markdown_validator` — [`L185`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/comprehensive_test_suite.py#L185)
  - `performance_tester` — [`L205`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/comprehensive_test_suite.py#L205)
  - `real_implementation_validation` — [`L196`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/comprehensive_test_suite.py#L196)
  - `results_dir` — [`L169`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/comprehensive_test_suite.py#L169)
  - `table_format_integration` — [`L194`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/comprehensive_test_suite.py#L194)
  - `test_data_manager` — [`L200`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/comprehensive_test_suite.py#L200)
- protocol/private: `__init__`[`L165`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/comprehensive_test_suite.py#L165)
- uses (calls/refs, reference-scoped): (35 test-only callers)
- used by: (9 test-only callers)

### `ComprehensiveSuiteDataMixin`
- def: [`tests/integration/formatters/comprehensive_test_suite.py:107`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/comprehensive_test_suite.py#L107)
- doc: Prepares generated or fallback test data for suite phases.
- signature: `class ComprehensiveSuiteDataMixin:`
- members:
  - `_prepare_test_data(self)` — [`L110`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/comprehensive_test_suite.py#L110) — Prepare test data for comprehensive testing
- protocol/private: `_load_created_test_data`[`L129`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/comprehensive_test_suite.py#L129)
- uses (calls/refs, reference-scoped): (3 test-only callers)
- used by: (2 test-only callers)

## Functions
- `_default_python_test_data()` — [`L149`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/comprehensive_test_suite.py#L149)
- `_ensure_config_defaults(config: FormatTestSuiteConfig)` — [`L267`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/comprehensive_test_suite.py#L267)
- `_test_data_set_source(test_id: str, test_data_set: Any)` — [`L138`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/comprehensive_test_suite.py#L138)
- `run_enabled_phases(suite: Any, analyzer_function: callable, test_data_sources: list[dict[str, Any]], results: TestSuiteResults)` — [`L250`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/comprehensive_test_suite.py#L250) — Run enabled suite phases and update aggregate counts.
- `run_full_validation_suite(analyzer_function)` — [`L333`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/comprehensive_test_suite.py#L333) — Run complete validation suite with all tests enabled
- `run_quick_format_validation(analyzer_function, test_data: str, language: str = "python")` — [`L279`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/comprehensive_test_suite.py#L279) — Quick format validation for development use
- `run_regression_test_suite(analyzer_function)` — [`L312`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/comprehensive_test_suite.py#L312) — Run regression test suite with focus on golden master and performance

## Module values
- `PHASES` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/comprehensive_test_suite.py#L49)
- `__all__` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/comprehensive_test_suite.py#L39)

