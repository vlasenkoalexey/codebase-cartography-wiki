---
title: 'Module: tests/integration/formatters/_comprehensive_suite_models.py'
type: catalog
provenance: extracted
module: tests/integration/formatters/_comprehensive_suite_models.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.formatters._comprehensive_suite_models`/
symbols:
  create_test_suite_results: create_test_suite_results().
  suite_results_to_dict: suite_results_to_dict().
  TestSuiteResults: TestSuiteResults#
  FormatTestSuiteConfig: FormatTestSuiteConfig#
  finalize_test_suite_results: finalize_test_suite_results().
  TestSuiteResults.total_tests: TestSuiteResults#total_tests.
  TestSuiteResults.success_rate: TestSuiteResults#success_rate.
  FormatTestSuiteConfig.enable_performance_tests: FormatTestSuiteConfig#enable_performance_tests.
  TestSuiteResults.passed_tests: TestSuiteResults#passed_tests.
  TestSuiteResults.failed_tests: TestSuiteResults#failed_tests.
  FormatTestSuiteConfig.enable_golden_master: FormatTestSuiteConfig#enable_golden_master.
  FormatTestSuiteConfig.enable_integration_tests: FormatTestSuiteConfig#enable_integration_tests.
  FormatTestSuiteConfig.generate_test_data: FormatTestSuiteConfig#generate_test_data.
  TestSuiteResults.execution_time_seconds: TestSuiteResults#execution_time_seconds.
  FormatTestSuiteConfig.enable_end_to_end_tests: FormatTestSuiteConfig#enable_end_to_end_tests.
  FormatTestSuiteConfig.enable_cross_component_tests: FormatTestSuiteConfig#enable_cross_component_tests.
  FormatTestSuiteConfig.enable_enhanced_assertions: FormatTestSuiteConfig#enable_enhanced_assertions.
  TestSuiteResults.timestamp: TestSuiteResults#timestamp.
  FormatTestSuiteConfig.enable_schema_validation: FormatTestSuiteConfig#enable_schema_validation.
  FormatTestSuiteConfig.enable_specification_compliance: FormatTestSuiteConfig#enable_specification_compliance.
  FormatTestSuiteConfig.enable_format_contracts: FormatTestSuiteConfig#enable_format_contracts.
  FormatTestSuiteConfig.test_data_languages: FormatTestSuiteConfig#test_data_languages.
  FormatTestSuiteConfig.performance_iterations: FormatTestSuiteConfig#performance_iterations.
  FormatTestSuiteConfig.results_directory: FormatTestSuiteConfig#results_directory.
  TestSuiteResults.golden_master_results: TestSuiteResults#golden_master_results.
  TestSuiteResults.schema_validation_results: TestSuiteResults#schema_validation_results.
  TestSuiteResults.integration_test_results: TestSuiteResults#integration_test_results.
  TestSuiteResults.end_to_end_results: TestSuiteResults#end_to_end_results.
  TestSuiteResults.cross_component_results: TestSuiteResults#cross_component_results.
  TestSuiteResults.specification_compliance_results: TestSuiteResults#specification_compliance_results.
  TestSuiteResults.format_contract_results: TestSuiteResults#format_contract_results.
  TestSuiteResults.performance_test_results: TestSuiteResults#performance_test_results.
  TestSuiteResults.enhanced_assertion_results: TestSuiteResults#enhanced_assertion_results.
  FormatTestSuiteConfig.test_data_complexities: FormatTestSuiteConfig#test_data_complexities.
  FormatTestSuiteConfig.save_detailed_results: FormatTestSuiteConfig#save_detailed_results.
  TestSuiteResults.skipped_tests: TestSuiteResults#skipped_tests.
  FormatTestSuiteConfig.scalability_test_sizes: FormatTestSuiteConfig#scalability_test_sizes.
---
# Module: [`tests/integration/formatters/_comprehensive_suite_models.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_models.py)

## Classes
### `FormatTestSuiteConfig`
- def: [`tests/integration/formatters/_comprehensive_suite_models.py:9`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_models.py#L9)
- doc: Configuration for comprehensive test suite
- signature: `class FormatTestSuiteConfig:`
- members:
  - `enable_cross_component_tests` — [`L16`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_models.py#L16)
  - `enable_end_to_end_tests` — [`L15`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_models.py#L15)
  - `enable_enhanced_assertions` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_models.py#L20)
  - `enable_format_contracts` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_models.py#L18)
  - `enable_golden_master` — [`L12`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_models.py#L12)
  - `enable_integration_tests` — [`L14`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_models.py#L14)
  - `enable_performance_tests` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_models.py#L19)
  - `enable_schema_validation` — [`L13`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_models.py#L13)
  - `enable_specification_compliance` — [`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_models.py#L17)
  - `generate_test_data` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_models.py#L23)
  - `performance_iterations` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_models.py#L28)
  - `results_directory` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_models.py#L33)
  - `save_detailed_results` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_models.py#L32)
  - `scalability_test_sizes` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_models.py#L29)
  - `test_data_complexities` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_models.py#L25)
  - `test_data_languages` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_models.py#L24)
- used by: (23 test-only callers)

### `TestSuiteResults`
- def: [`tests/integration/formatters/_comprehensive_suite_models.py:37`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_models.py#L37)
- doc: Results from comprehensive test suite execution
- signature: `class TestSuiteResults:`
- members:
  - `cross_component_results` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_models.py#L49)
  - `end_to_end_results` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_models.py#L48)
  - `enhanced_assertion_results` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_models.py#L53)
  - `execution_time_seconds` — [`L55`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_models.py#L55)
  - `failed_tests` — [`L42`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_models.py#L42)
  - `format_contract_results` — [`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_models.py#L51)
  - `golden_master_results` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_models.py#L45)
  - `integration_test_results` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_models.py#L47)
  - `passed_tests` — [`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_models.py#L41)
  - `performance_test_results` — [`L52`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_models.py#L52)
  - `schema_validation_results` — [`L46`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_models.py#L46)
  - `skipped_tests` — [`L43`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_models.py#L43)
  - `specification_compliance_results` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_models.py#L50)
  - `success_rate` — [`L57`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_models.py#L57)
  - `timestamp` — [`L56`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_models.py#L56)
  - `total_tests` — [`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_models.py#L40)
- used by: (19 test-only callers)

## Functions
- `create_test_suite_results(start_time: datetime)` — [`L60`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_models.py#L60) — Create an empty result object for a suite run.
- `finalize_test_suite_results(results: TestSuiteResults, start_time: datetime)` — [`L82`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_models.py#L82) — Populate final timing and success-rate metrics.
- `suite_results_to_dict(results: TestSuiteResults)` — [`L94`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_models.py#L94) — Convert result dataclass to JSON-serializable dictionary.

