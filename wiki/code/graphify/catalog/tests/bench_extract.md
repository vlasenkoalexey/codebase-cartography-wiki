---
title: 'Module: tests/bench_extract.py'
type: catalog
provenance: extracted
module: tests/bench_extract.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.bench_extract`/
symbols:
  main: main().
  _project_root: _project_root.
  _run_extraction: _run_extraction().
  _format_languages: _format_languages().
  _count_by_ext: _count_by_ext().
  _EXT_NAMES._EXT_NAMES: _EXT_NAMES._EXT_NAMES.
---
# Module: [`tests/bench_extract.py`](../../../../../raw/code/graphify/tests/bench_extract.py)

## Functions
- `_count_by_ext(paths: list[Path])` — [`L38`](../../../../../raw/code/graphify/tests/bench_extract.py#L38) — Count files by extension.
- `_format_languages(ext_counts: dict[str, int])` — [`L88`](../../../../../raw/code/graphify/tests/bench_extract.py#L88)
- `_run_extraction(paths: list[Path], cache_root: Path, parallel: bool, max_workers: int | None = None)` — [`L96`](../../../../../raw/code/graphify/tests/bench_extract.py#L96) — Run extraction, return (elapsed_seconds, node_count, edge_count).
- `main()` — [`L114`](../../../../../raw/code/graphify/tests/bench_extract.py#L114)

## Module values
- `_EXT_NAMES` — [`L47`](../../../../../raw/code/graphify/tests/bench_extract.py#L47)
- `_project_root` — [`L30`](../../../../../raw/code/graphify/tests/bench_extract.py#L30)

