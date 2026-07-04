---
title: 'Module: benchmarks/codegraph_compare/gauntlet_runner.py'
type: catalog
provenance: extracted
module: benchmarks/codegraph_compare/gauntlet_runner.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `benchmarks.codegraph_compare.gauntlet_runner`/
symbols:
  _audit_repo: _audit_repo().
  main: main().
  _render_table: _render_table().
  _run_audit: _run_audit().
  GauntletRow: GauntletRow#
  GauntletRow.error: GauntletRow#error.
  GauntletRow.display_name: GauntletRow#display_name.
  GauntletRow.languages: GauntletRow#languages.
  GauntletRow.call_edges: GauntletRow#call_edges.
  GauntletRow.naive_miswires: GauntletRow#naive_miswires.
  GauntletRow.naive_pct: GauntletRow#naive_pct.
  GauntletRow.tsa_miswires: GauntletRow#tsa_miswires.
  _build_parser: _build_parser().
  _GAUNTLET_REPOS._GAUNTLET_REPOS: _GAUNTLET_REPOS._GAUNTLET_REPOS.
  GauntletRow.id: GauntletRow#id.
  _update_gauntlet_md: _update_gauntlet_md().
  _THIS_DIR: _THIS_DIR.
  _BASE_DIR: _BASE_DIR.
---
# Module: [`benchmarks/codegraph_compare/gauntlet_runner.py`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/gauntlet_runner.py)

## Classes
### `GauntletRow`  ·  implements/extends NamedTuple
- def: [`benchmarks/codegraph_compare/gauntlet_runner.py:80`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/gauntlet_runner.py#L80)
- signature: `class GauntletRow(NamedTuple):`
- members:
  - `call_edges` — [`L84`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/gauntlet_runner.py#L84)
  - `display_name` — [`L82`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/gauntlet_runner.py#L82)
  - `error` — [`L88`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/gauntlet_runner.py#L88)
  - `id` — [`L81`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/gauntlet_runner.py#L81)
  - `languages` — [`L83`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/gauntlet_runner.py#L83)
  - `naive_miswires` — [`L85`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/gauntlet_runner.py#L85)
  - `naive_pct` — [`L86`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/gauntlet_runner.py#L86)
  - `tsa_miswires` — [`L87`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/gauntlet_runner.py#L87)
- used by: (3 test-only callers)

## Functions
- `_audit_repo(repo_id: str, display_name: str, url: str, commit: str, languages: str, base_dir: Path, *, reindex: bool = True)` — [`L114`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/gauntlet_runner.py#L114) — Clone (if needed) and audit a single repo. Returns a GauntletRow.
- `_build_parser()` — [`L247`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/gauntlet_runner.py#L247)
- `_render_table(rows: list[GauntletRow], timestamp: str)` — [`L182`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/gauntlet_runner.py#L182) — Render a markdown table from GauntletRows.
- `_run_audit(repo_path: str, *, reindex: bool = True)` — [`L96`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/gauntlet_runner.py#L96) — Return (call_edges, naive_miswires, naive_pct, tsa_miswires) for repo_path.
- `_update_gauntlet_md(table: str)` — [`L206`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/gauntlet_runner.py#L206) — Splice the new table into GAUNTLET.md, replacing the old summary table.
- `main(argv: list[str] | None = None)` — [`L294`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/gauntlet_runner.py#L294)

## Module values
- `_BASE_DIR` — [`L31`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/gauntlet_runner.py#L31)
- `_GAUNTLET_REPOS` — [`L36`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/gauntlet_runner.py#L36)
- `_THIS_DIR` — [`L30`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/gauntlet_runner.py#L30)

