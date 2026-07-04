---
title: 'Module: tests/integration/formatters/_enhanced_assertion_models.py'
type: catalog
provenance: extracted
module: tests/integration/formatters/_enhanced_assertion_models.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.formatters._enhanced_assertion_models`/
symbols:
  AssertionResult: AssertionResult#
  FormatElement: FormatElement#
  AssertionResult.message: AssertionResult#message.
  FormatElement.name: FormatElement#name.
  AssertionResult.passed: AssertionResult#passed.
  AssertionResult.severity: AssertionResult#severity.
  AssertionResult.details: AssertionResult#details.
  AssertionResult.suggestion: AssertionResult#suggestion.
  FormatElement.element_type: FormatElement#element_type.
  AssertionResult.location: AssertionResult#location.
  FormatElement.line_number: FormatElement#line_number.
  FormatElement.column_number: FormatElement#column_number.
  FormatElement.attributes: FormatElement#attributes.
  FormatElement.content: FormatElement#content.
---
# Module: [`tests/integration/formatters/_enhanced_assertion_models.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_enhanced_assertion_models.py)

## Classes
### `AssertionResult`
- def: [`tests/integration/formatters/_enhanced_assertion_models.py:8`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_enhanced_assertion_models.py#L8)
- doc: Result of an assertion with detailed information
- signature: `class AssertionResult:`
- members:
  - `details` — [`L13`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_enhanced_assertion_models.py#L13)
  - `location` — [`L15`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_enhanced_assertion_models.py#L15)
  - `message` — [`L12`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_enhanced_assertion_models.py#L12)
  - `passed` — [`L11`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_enhanced_assertion_models.py#L11)
  - `severity` — [`L14`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_enhanced_assertion_models.py#L14)
  - `suggestion` — [`L16`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_enhanced_assertion_models.py#L16)
- used by: (41 test-only callers)

### `FormatElement`
- def: [`tests/integration/formatters/_enhanced_assertion_models.py:20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_enhanced_assertion_models.py#L20)
- doc: Represents a format element with metadata
- signature: `class FormatElement:`
- members:
  - `attributes` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_enhanced_assertion_models.py#L28)
  - `column_number` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_enhanced_assertion_models.py#L27)
  - `content` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_enhanced_assertion_models.py#L25)
  - `element_type` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_enhanced_assertion_models.py#L23)
  - `line_number` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_enhanced_assertion_models.py#L26)
  - `name` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_enhanced_assertion_models.py#L24)
- used by: (26 test-only callers)

