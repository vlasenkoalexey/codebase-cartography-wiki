---
title: 'Module: tests/test_astro_extraction.py'
type: catalog
provenance: extracted
module: tests/test_astro_extraction.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_astro_extraction`/
symbols:
  _write: _write().
  test_extract_astro_picks_up_frontmatter_static_imports: test_extract_astro_picks_up_frontmatter_static_imports().
  test_extract_astro_handles_dynamic_import_in_frontmatter: test_extract_astro_handles_dynamic_import_in_frontmatter().
  test_extract_astro_picks_up_client_side_script_imports: test_extract_astro_picks_up_client_side_script_imports().
  test_extract_astro_handles_tsconfig_path_alias: test_extract_astro_handles_tsconfig_path_alias().
  test_extract_astro_no_frontmatter_does_not_crash: test_extract_astro_no_frontmatter_does_not_crash().
  _import_targets: _import_targets().
  test_astro_is_in_code_extensions: test_astro_is_in_code_extensions().
---
# Module: [`tests/test_astro_extraction.py`](../../../../../raw/code/graphify/tests/test_astro_extraction.py)

## Functions
- `_import_targets(result: dict, *, relation: str | None = None)` — [`L27`](../../../../../raw/code/graphify/tests/test_astro_extraction.py#L27)
- `_write(path: Path, body: str)` — [`L21`](../../../../../raw/code/graphify/tests/test_astro_extraction.py#L21)
- `test_astro_is_in_code_extensions()` — [`L35`](../../../../../raw/code/graphify/tests/test_astro_extraction.py#L35) — Without this, detect.py silently drops `.astro` from the AST pass (#850).
- `test_extract_astro_handles_dynamic_import_in_frontmatter(tmp_path)` — [`L64`](../../../../../raw/code/graphify/tests/test_astro_extraction.py#L64)
- `test_extract_astro_handles_tsconfig_path_alias(tmp_path)` — [`L119`](../../../../../raw/code/graphify/tests/test_astro_extraction.py#L119)
- `test_extract_astro_no_frontmatter_does_not_crash(tmp_path)` — [`L107`](../../../../../raw/code/graphify/tests/test_astro_extraction.py#L107) — Astro permits frontmatter-less files (pure-HTML pages). Must not raise.
- `test_extract_astro_picks_up_client_side_script_imports(tmp_path)` — [`L81`](../../../../../raw/code/graphify/tests/test_astro_extraction.py#L81)
- `test_extract_astro_picks_up_frontmatter_static_imports(tmp_path)` — [`L40`](../../../../../raw/code/graphify/tests/test_astro_extraction.py#L40)

