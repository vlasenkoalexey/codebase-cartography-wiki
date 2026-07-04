---
title: 'Module: tests/unit/test_doc_cli_examples.py'
type: catalog
provenance: extracted
module: tests/unit/test_doc_cli_examples.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_doc_cli_examples`/
symbols:
  test_documented_cli_flags_exist_in_parser: test_documented_cli_flags_exist_in_parser().
  PROJECT_ROOT: PROJECT_ROOT.
  test_canonical_cli_reference_doc_has_examples: test_canonical_cli_reference_doc_has_examples().
  _iter_cli_lines: _iter_cli_lines().
  DOC_PATHS: DOC_PATHS.
  DOCS_REQUIRING_CLI_EXAMPLES: DOCS_REQUIRING_CLI_EXAMPLES.
  _CLI_LINE: _CLI_LINE.
  _FLAG: _FLAG.
---
# Module: [`tests/unit/test_doc_cli_examples.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_doc_cli_examples.py)

## Functions
- `_iter_cli_lines()` — [`L48`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_doc_cli_examples.py#L48) — Yield ``(path, line_number, tail_after_command)`` for every CLI
- `test_canonical_cli_reference_doc_has_examples()` — [`L87`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_doc_cli_examples.py#L87) — Guard against the canonical CLI-reference doc(s) going empty.
- `test_documented_cli_flags_exist_in_parser()` — [`L62`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_doc_cli_examples.py#L62) — Every --flag mentioned in our docs must be a registered argparse

## Module values
- `DOCS_REQUIRING_CLI_EXAMPLES` — [`L33`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_doc_cli_examples.py#L33)
- `DOC_PATHS` — [`L22`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_doc_cli_examples.py#L22)
- `PROJECT_ROOT` — [`L18`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_doc_cli_examples.py#L18)
- `_CLI_LINE` — [`L41`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_doc_cli_examples.py#L41)
- `_FLAG` — [`L45`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_doc_cli_examples.py#L45)

