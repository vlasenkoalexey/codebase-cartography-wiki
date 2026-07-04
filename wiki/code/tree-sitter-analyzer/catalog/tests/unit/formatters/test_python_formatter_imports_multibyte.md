---
title: 'Module: tests/unit/formatters/test_python_formatter_imports_multibyte.py'
type: catalog
provenance: extracted
module: tests/unit/formatters/test_python_formatter_imports_multibyte.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.formatters.test_python_formatter_imports_multibyte`/
symbols:
  _table_output: _table_output().
  test_imports_section_renders_clean_without_multibyte: test_imports_section_renders_clean_without_multibyte().
  test_imports_section_renders_clean_after_multibyte_docstring: test_imports_section_renders_clean_after_multibyte_docstring().
  _extract_import_block: _extract_import_block().
  _MULTIBYTE_PY_SOURCE: _MULTIBYTE_PY_SOURCE.
---
# Module: [`tests/unit/formatters/test_python_formatter_imports_multibyte.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_imports_multibyte.py)

## Functions
- `_extract_import_block(output: str)` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_imports_multibyte.py#L48)
- `_table_output(tmp_path: Path)` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_imports_multibyte.py#L39)
- `test_imports_section_renders_clean_after_multibyte_docstring(tmp_path: Path)` — [`L67`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_imports_multibyte.py#L67) — Regression: em-dash in docstring must not corrupt downstream imports.
- `test_imports_section_renders_clean_without_multibyte(tmp_path: Path)` — [`L92`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_imports_multibyte.py#L92) — Sanity: pure-ASCII source still produces clean imports (no regression).

## Module values
- `_MULTIBYTE_PY_SOURCE` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_imports_multibyte.py#L24)

