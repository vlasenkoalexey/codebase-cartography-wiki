---
title: 'Module: tests/integration/formatters/_comprehensive_suite_phase_helpers.py'
type: catalog
provenance: extracted
module: tests/integration/formatters/_comprehensive_suite_phase_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.formatters._comprehensive_suite_phase_helpers`/
symbols:
  PhaseCase.test_name: PhaseCase#test_name.
  PhaseCase.results: PhaseCase#results.
  PhaseCase.test_data: PhaseCase#test_data.
  add_error: add_error().
  PhaseCase: PhaseCase#
  PhaseCase.format_type: PhaseCase#format_type.
  PhaseCase.analyzer_function: PhaseCase#analyzer_function.
  add_pass: add_pass().
  new_phase_results: new_phase_results().
  add_failure: add_failure().
  FORMAT_TYPES: FORMAT_TYPES.
  call_analyzer: call_analyzer().
  is_non_empty_output: is_non_empty_output().
  is_valid_e2e_output: is_valid_e2e_output().
  e2e_failure_message: e2e_failure_message().
  is_schema_valid: is_schema_valid().
  is_specification_compliant: is_specification_compliant().
---
# Module: [`tests/integration/formatters/_comprehensive_suite_phase_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_phase_helpers.py)

## Classes
### `PhaseCase`
- def: [`tests/integration/formatters/_comprehensive_suite_phase_helpers.py:11`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_phase_helpers.py#L11)
- doc: Inputs for one phase case execution.
- signature: `class PhaseCase:`
- members:
  - `analyzer_function` — [`L14`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_phase_helpers.py#L14)
  - `format_type` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_phase_helpers.py#L18)
  - `results` — [`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_phase_helpers.py#L17)
  - `test_data` — [`L15`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_phase_helpers.py#L15)
  - `test_name` — [`L16`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_phase_helpers.py#L16)
- used by: (11 test-only callers)

## Functions
- `add_error(results: dict[str, Any], test_name: str, error: Exception | str)` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_phase_helpers.py#L45) — Record an errored test detail.
- `add_failure(results: dict[str, Any], test_name: str, message: str)` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_phase_helpers.py#L37) — Record a failed test detail.
- `add_pass(results: dict[str, Any], test_name: str, message: str)` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_phase_helpers.py#L29) — Record a passed test detail.
- `call_analyzer(analyzer_function: callable, source_code: str, format_type: str)` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_phase_helpers.py#L53) — Call analyzer functions that may be sync or async.
- `e2e_failure_message(format_type: str)` — [`L76`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_phase_helpers.py#L76)
- `is_non_empty_output(output: str)` — [`L64`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_phase_helpers.py#L64)
- `is_schema_valid(suite: Any, format_type: str, output: str)` — [`L84`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_phase_helpers.py#L84) — Validate generated output against the configured schema validator.
- `is_specification_compliant(format_type: str, output: str)` — [`L100`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_phase_helpers.py#L100) — Check the lightweight format compliance rules used by this suite.
- `is_valid_e2e_output(format_type: str, output: str)` — [`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_phase_helpers.py#L68)
- `new_phase_results(extra: dict[str, Any] | None = None)` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_phase_helpers.py#L21) — Create a standard phase result dictionary.

## Module values
- `FORMAT_TYPES` — [`L7`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_comprehensive_suite_phase_helpers.py#L7)

