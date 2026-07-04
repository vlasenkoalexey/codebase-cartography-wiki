---
title: 'Module: scripts/check_orphan_modules.py'
type: catalog
provenance: extracted
module: scripts/check_orphan_modules.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `scripts.check_orphan_modules`/
symbols:
  find_orphans: find_orphans().
  cmd_snapshot: cmd_snapshot().
  ROOT: ROOT.
  cmd_check: cmd_check().
  main: main().
  BASELINE: BASELINE.
  TESTS_DIR: TESTS_DIR.
  _tracked_source_files: _tracked_source_files().
  _test_stems: _test_stems().
  _read_baseline: _read_baseline().
  SOURCE_DIR: SOURCE_DIR.
  _expected_test_basename: _expected_test_basename().
---
# Module: [`scripts/check_orphan_modules.py`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_orphan_modules.py)

## Functions
- `_expected_test_basename(source: Path)` — [`L62`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_orphan_modules.py#L62) — E.g. ``tree_sitter_analyzer/_api_helpers.py`` -> ``test_api_helpers``.
- `_read_baseline()` — [`L81`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_orphan_modules.py#L81)
- `_test_stems()` — [`L54`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_orphan_modules.py#L54) — All test_*.py stems under tests/, lowercased.
- `_tracked_source_files()` — [`L35`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_orphan_modules.py#L35) — Tracked .py files under tree_sitter_analyzer/. Excludes __init__.py.
- `cmd_check()` — [`L105`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_orphan_modules.py#L105)
- `cmd_snapshot()` — [`L91`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_orphan_modules.py#L91)
- `find_orphans()` — [`L68`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_orphan_modules.py#L68)
- `main(argv: list[str] | None = None)` — [`L144`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_orphan_modules.py#L144)

## Module values
- `BASELINE` — [`L32`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_orphan_modules.py#L32)
- `ROOT` — [`L29`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_orphan_modules.py#L29)
- `SOURCE_DIR` — [`L30`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_orphan_modules.py#L30)
- `TESTS_DIR` — [`L31`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_orphan_modules.py#L31)

