---
title: 'Module: tests/integration/grammar_coverage/test_validator_integration.py'
type: catalog
provenance: extracted
module: tests/integration/grammar_coverage/test_validator_integration.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.grammar_coverage.test_validator_integration`/Test
symbols:
  TestValidatorWithRealCorpus.test_generate_coverage_report_format: ValidatorWithRealCorpus#test_generate_coverage_report_format().
  TestValidatorWithRealCorpus.test_validate_plugin_coverage_python: ValidatorWithRealCorpus#test_validate_plugin_coverage_python().
  TestValidatorWithRealCorpus.test_validate_plugin_coverage_sync_python: ValidatorWithRealCorpus#test_validate_plugin_coverage_sync_python().
  TestPluginIntegration.test_get_covered_node_types_from_plugin_python: PluginIntegration#test_get_covered_node_types_from_plugin_python().
  TestPluginIntegration.test_get_covered_node_types_unsupported_language: PluginIntegration#test_get_covered_node_types_unsupported_language().
  TestPluginIntegration.test_get_covered_node_types_empty_file: PluginIntegration#test_get_covered_node_types_empty_file().
  TestValidatorWithRealCorpus.test_parse_corpus_file_python: ValidatorWithRealCorpus#test_parse_corpus_file_python().
  TestValidatorWithRealCorpus.test_check_coverage_threshold: ValidatorWithRealCorpus#test_check_coverage_threshold().
  TestErrorHandling.test_nonexistent_corpus_file: ErrorHandling#test_nonexistent_corpus_file().
  TestErrorHandling.test_validate_unsupported_language: ErrorHandling#test_validate_unsupported_language().
  TestErrorHandling.test_get_covered_types_invalid_file: ErrorHandling#test_get_covered_types_invalid_file().
  TestPluginIntegration: PluginIntegration#
  TestValidatorWithRealCorpus: ValidatorWithRealCorpus#
  TestErrorHandling: ErrorHandling#
---
# Module: [`tests/integration/grammar_coverage/test_validator_integration.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/grammar_coverage/test_validator_integration.py)

## Classes
### `TestErrorHandling`
- def: [`tests/integration/grammar_coverage/test_validator_integration.py:225`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/grammar_coverage/test_validator_integration.py#L225)
- doc: Tests for error handling in validator
- signature: `class TestErrorHandling:`
- members:
  - `test_get_covered_types_invalid_file(self)` — [`L241`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/grammar_coverage/test_validator_integration.py#L241) — Test with invalid file path
  - `test_nonexistent_corpus_file(self)` — [`L228`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/grammar_coverage/test_validator_integration.py#L228) — Test with non-existent corpus file
  - `test_validate_unsupported_language(self)` — [`L235`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/grammar_coverage/test_validator_integration.py#L235) — Test validation with unsupported language
- uses (calls/refs, reference-scoped): [`_get_covered_node_types_from_plugin`](../../../tree_sitter_analyzer/grammar_coverage/validator.md#_get_covered_node_types_from_plugin), [`validate_plugin_coverage`](../../../tree_sitter_analyzer/grammar_coverage/validator.md#validate_plugin_coverage), [`_parse_corpus_file`](../../../tree_sitter_analyzer/grammar_coverage/validator.md#_parse_corpus_file)

### `TestPluginIntegration`
- def: [`tests/integration/grammar_coverage/test_validator_integration.py:25`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/grammar_coverage/test_validator_integration.py#L25)
- doc: Tests for plugin integration with validator
- signature: `class TestPluginIntegration:`
- members:
  - `test_get_covered_node_types_empty_file(self)` — [`L90`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/grammar_coverage/test_validator_integration.py#L90) — Test with empty file
  - `test_get_covered_node_types_from_plugin_python(self)` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/grammar_coverage/test_validator_integration.py#L29) — Test that covered node types are correctly detected from Python plugin
  - `test_get_covered_node_types_unsupported_language(self)` — [`L70`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/grammar_coverage/test_validator_integration.py#L70) — Test behavior with unsupported language
- uses (calls/refs, reference-scoped): [`_get_covered_node_types_from_plugin`](../../../tree_sitter_analyzer/grammar_coverage/validator.md#_get_covered_node_types_from_plugin)

### `TestValidatorWithRealCorpus`
- def: [`tests/integration/grammar_coverage/test_validator_integration.py:110`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/grammar_coverage/test_validator_integration.py#L110)
- doc: Tests using real corpus files if available
- signature: `class TestValidatorWithRealCorpus:`
- members:
  - `test_check_coverage_threshold(self)` — [`L212`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/grammar_coverage/test_validator_integration.py#L212) — Test coverage threshold checking
  - `test_generate_coverage_report_format(self)` — [`L186`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/grammar_coverage/test_validator_integration.py#L186) — Test coverage report generation format
  - `test_parse_corpus_file_python(self)` — [`L113`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/grammar_coverage/test_validator_integration.py#L113) — Test parsing a real Python corpus file
  - `test_validate_plugin_coverage_python(self)` — [`L134`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/grammar_coverage/test_validator_integration.py#L134) — Test full validation pipeline with Python corpus
  - `test_validate_plugin_coverage_sync_python(self)` — [`L163`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/grammar_coverage/test_validator_integration.py#L163) — Test synchronous validation with Python corpus
- uses (calls/refs, reference-scoped): [`validate_plugin_coverage`](../../../tree_sitter_analyzer/grammar_coverage/validator.md#validate_plugin_coverage), [`uncovered_types`](../../../tree_sitter_analyzer/grammar_coverage/validator.md#CoverageReport.uncovered_types), [`generate_coverage_report`](../../../tree_sitter_analyzer/grammar_coverage/validator.md#generate_coverage_report), [`coverage_percentage`](../../../tree_sitter_analyzer/grammar_coverage/validator.md#CoverageReport.coverage_percentage), [`check_coverage_threshold`](../../../tree_sitter_analyzer/grammar_coverage/validator.md#check_coverage_threshold), [`validate_plugin_coverage_sync`](../../../tree_sitter_analyzer/grammar_coverage/validator.md#validate_plugin_coverage_sync), [`covered_node_types`](../../../tree_sitter_analyzer/grammar_coverage/validator.md#CoverageReport.covered_node_types), [`total_node_types`](../../../tree_sitter_analyzer/grammar_coverage/validator.md#CoverageReport.total_node_types), [`CoverageReport`](../../../tree_sitter_analyzer/grammar_coverage/validator.md#CoverageReport), [`language`](../../../tree_sitter_analyzer/grammar_coverage/validator.md#CoverageReport.language), [`_parse_corpus_file`](../../../tree_sitter_analyzer/grammar_coverage/validator.md#_parse_corpus_file), [`corpus_file`](../../../tree_sitter_analyzer/grammar_coverage/validator.md#CoverageReport.corpus_file), [`actual_node_types`](../../../tree_sitter_analyzer/grammar_coverage/validator.md#CoverageReport.actual_node_types), [`expected_node_types`](../../../tree_sitter_analyzer/grammar_coverage/validator.md#CoverageReport.expected_node_types)

