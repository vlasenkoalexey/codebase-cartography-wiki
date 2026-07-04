---
title: 'Module: tests/test_extraction_spec_ids.py'
type: catalog
provenance: extracted
module: tests/test_extraction_spec_ids.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_extraction_spec_ids`/
symbols:
  _examples: _examples().
  _ast_symbol_id: _ast_symbol_id().
  test_spec_files_are_discoverable: test_spec_files_are_discoverable().
  test_spec_node_id_examples_match_ast_extractor: test_spec_node_id_examples_match_ast_extractor().
  test_cautionary_wrong_forms_are_actually_wrong: test_cautionary_wrong_forms_are_actually_wrong().
  _spec_files: _spec_files().
  REPO_ROOT: REPO_ROOT.
  _EXAMPLE_RE: _EXAMPLE_RE.
---
# Module: [`tests/test_extraction_spec_ids.py`](../../../../../raw/code/graphify/tests/test_extraction_spec_ids.py)

## Functions
- `_ast_symbol_id(path: str, entity: str)` — [`L56`](../../../../../raw/code/graphify/tests/test_extraction_spec_ids.py#L56) — Reproduce the symbol ID the AST extractor emits for a file + symbol, using
- `_examples()` — [`L47`](../../../../../raw/code/graphify/tests/test_extraction_spec_ids.py#L47)
- `_spec_files()` — [`L34`](../../../../../raw/code/graphify/tests/test_extraction_spec_ids.py#L34)
- `test_cautionary_wrong_forms_are_actually_wrong()` — [`L88`](../../../../../raw/code/graphify/tests/test_extraction_spec_ids.py#L88) — The canonical spec warns against the filename-only and full-path ID forms.
- `test_spec_files_are_discoverable()` — [`L62`](../../../../../raw/code/graphify/tests/test_extraction_spec_ids.py#L62) — Guard the guard: if the spec moves or the example format changes so nothing
- `test_spec_node_id_examples_match_ast_extractor(path, entity, expected)` — [`L79`](../../../../../raw/code/graphify/tests/test_extraction_spec_ids.py#L79)

## Module values
- `REPO_ROOT` — [`L27`](../../../../../raw/code/graphify/tests/test_extraction_spec_ids.py#L27)
- `_EXAMPLE_RE` — [`L31`](../../../../../raw/code/graphify/tests/test_extraction_spec_ids.py#L31)

