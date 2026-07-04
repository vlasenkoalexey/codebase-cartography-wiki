---
title: 'Module: tests/integration/test_synapse_backfill.py'
type: catalog
provenance: extracted
module: tests/integration/test_synapse_backfill.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.test_synapse_backfill`/
symbols:
  test_backfill_no_reparse: test_backfill_no_reparse().
  seeded_project: seeded_project().
  _reset_resolution_columns: _reset_resolution_columns().
  test_backfill_no_reparse.counting_parse: test_backfill_no_reparse().counting_parse().
---
# Module: [`tests/integration/test_synapse_backfill.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_synapse_backfill.py)

## Functions
- `_reset_resolution_columns(cache: ASTCache)` — [`L46`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_synapse_backfill.py#L46) — Force every edge back to 'unknown' so backfill has work to do.
- `counting_parse(self, *args, **kwargs)` — [`L81`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_synapse_backfill.py#L81)
- `seeded_project(tmp_path: Path)` — [`L31`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_synapse_backfill.py#L31) — Build a real Python project on disk and index it once, normally.
- `test_backfill_no_reparse(seeded_project: Path, monkeypatch: pytest.MonkeyPatch)` — [`L62`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_synapse_backfill.py#L62) — resolve_only=True populates the columns without calling the parser.

