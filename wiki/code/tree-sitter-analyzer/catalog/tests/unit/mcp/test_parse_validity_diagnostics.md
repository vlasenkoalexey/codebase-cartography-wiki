---
title: 'Module: tests/unit/mcp/test_parse_validity_diagnostics.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_parse_validity_diagnostics.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_parse_validity_diagnostics`/test_
symbols:
  test_decode_replacement_falls_back_when_safe_decode_raises: decode_replacement_falls_back_when_safe_decode_raises().
  test_file_byte_diagnostics_degrades_on_read_error: file_byte_diagnostics_degrades_on_read_error().
  test_file_byte_diagnostics_reports_decode_replacement: file_byte_diagnostics_reports_decode_replacement().
  test_attach_input_diagnostics_tolerates_non_dict_agent_summary: attach_input_diagnostics_tolerates_non_dict_agent_summary().
  test_file_byte_diagnostics_ignores_missing_and_empty_files: file_byte_diagnostics_ignores_missing_and_empty_files().
  test_file_byte_diagnostics_degrades_on_read_error._raise_os_error: file_byte_diagnostics_degrades_on_read_error()._raise_os_error().
  test_decode_replacement_falls_back_when_safe_decode_raises._raise_decode_error: decode_replacement_falls_back_when_safe_decode_raises()._raise_decode_error().
---
# Module: [`tests/unit/mcp/test_parse_validity_diagnostics.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_parse_validity_diagnostics.py)

## Functions
- `_raise_decode_error(raw: bytes, encoding: str)` — [`L60`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_parse_validity_diagnostics.py#L60)
- `_raise_os_error(self: Path)` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_parse_validity_diagnostics.py#L26)
- `test_attach_input_diagnostics_tolerates_non_dict_agent_summary(tmp_path: Path)` — [`L72`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_parse_validity_diagnostics.py#L72)
- `test_decode_replacement_falls_back_when_safe_decode_raises(monkeypatch)` — [`L59`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_parse_validity_diagnostics.py#L59)
- `test_file_byte_diagnostics_degrades_on_read_error(tmp_path: Path, monkeypatch)` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_parse_validity_diagnostics.py#L20)
- `test_file_byte_diagnostics_ignores_missing_and_empty_files(tmp_path: Path)` — [`L11`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_parse_validity_diagnostics.py#L11)
- `test_file_byte_diagnostics_reports_decode_replacement(tmp_path: Path, monkeypatch)` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_parse_validity_diagnostics.py#L34)

