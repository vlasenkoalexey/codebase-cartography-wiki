---
title: 'Module: tests/unit/cli/test_cli_package.py'
type: catalog
provenance: extracted
module: tests/unit/cli/test_cli_package.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.cli.test_cli_package`/test_cli_
symbols:
  test_cli_info_commands_imported: info_commands_imported().
  test_cli_all_attribute: all_attribute().
  test_cli_import_error_fallback: import_error_fallback().
  test_cli_import_error_fallback.BlockFinder: import_error_fallback().BlockFinder#
  test_cli_imports: imports().
  test_cli_exports: exports().
  test_cli_has_dir: has_dir().
  test_cli_import_error_fallback.BlockFinder.find_spec: import_error_fallback().BlockFinder#find_spec().
---
# Module: [`tests/unit/cli/test_cli_package.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_package.py)

## Classes
### `BlockFinder`
- def: [`tests/unit/cli/test_cli_package.py:100`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_package.py#L100)
- signature: `class BlockFinder:`
- members:
  - `find_spec(self, fullname, path, target=None)` — [`L101`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_package.py#L101)
- used by: (1 test-only callers)

## Functions
- `test_cli_all_attribute()` — [`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_package.py#L41) — Test that CLI __all__ contains expected attributes.
- `test_cli_exports()` — [`L16`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_package.py#L16) — Test that CLI package exports expected names.
- `test_cli_has_dir()` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_package.py#L73) — Test that CLI package has expected directory structure.
- `test_cli_import_error_fallback()` — [`L89`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_package.py#L89) — Test CLI package sets None fallbacks when core imports fail.
- `test_cli_imports()` — [`L9`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_package.py#L9) — Test that CLI package can be imported.
- `test_cli_info_commands_imported()` — [`L55`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_cli_package.py#L55) — Test that CLI info commands are properly imported.

