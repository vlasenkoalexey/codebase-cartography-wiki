---
title: 'Module: scripts/update_language_parsers.py'
type: catalog
provenance: extracted
module: scripts/update_language_parsers.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `scripts.update_language_parsers`/
symbols:
  update_language_file: update_language_file().
  main: main().
  LANGUAGE_FILES: LANGUAGE_FILES.
  LANGUAGES_DIR: LANGUAGES_DIR.
  update_imports: update_imports().
  remove_query_dict_init: remove_query_dict_init().
  replace_query_usage: replace_query_usage().
  get_query_dict_name: get_query_dict_name().
---
# Module: [`scripts/update_language_parsers.py`](../../../../../raw/code/codegraphcontext/scripts/update_language_parsers.py)

## Functions
- `get_query_dict_name(content: str)` — [`L108`](../../../../../raw/code/codegraphcontext/scripts/update_language_parsers.py#L108) — Detect the query dictionary name (e.g., PY_QUERIES, JS_QUERIES, etc.).
- `main()` — [`L140`](../../../../../raw/code/codegraphcontext/scripts/update_language_parsers.py#L140) — Update all language parser files.
- `remove_query_dict_init(content: str)` — [`L49`](../../../../../raw/code/codegraphcontext/scripts/update_language_parsers.py#L49) — Remove self.queries dictionary initialization.
- `replace_query_usage(content: str, query_dict_name: str)` — [`L57`](../../../../../raw/code/codegraphcontext/scripts/update_language_parsers.py#L57) — Replace query.captures() with execute_query().
- `update_imports(content: str)` — [`L32`](../../../../../raw/code/codegraphcontext/scripts/update_language_parsers.py#L32) — Add execute_query import if not present.
- `update_language_file(path: Path)` — [`L116`](../../../../../raw/code/codegraphcontext/scripts/update_language_parsers.py#L116) — Update a single language file.

## Module values
- `LANGUAGES_DIR` — [`L29`](../../../../../raw/code/codegraphcontext/scripts/update_language_parsers.py#L29)
- `LANGUAGE_FILES` — [`L15`](../../../../../raw/code/codegraphcontext/scripts/update_language_parsers.py#L15)

