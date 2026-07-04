---
title: 'Module: tests/unit/test_lang_extension_map.py'
type: catalog
provenance: extracted
module: tests/unit/test_lang_extension_map.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_lang_extension_map`/
symbols:
  test_swiftinterface_resolves_in_all_known_ext_maps: test_swiftinterface_resolves_in_all_known_ext_maps().
  test_every_plugin_has_extension_wiring: test_every_plugin_has_extension_wiring().
  test_project_graph_alias_resolves_via_canonical: test_project_graph_alias_resolves_via_canonical().
  _discover_plugin_languages: _discover_plugin_languages().
  test_ast_cache_alias_matches_canonical: test_ast_cache_alias_matches_canonical().
  test_long_broken_extensions_stay_wired: test_long_broken_extensions_stay_wired().
  test_discover_plugin_languages_finds_known_set: test_discover_plugin_languages_finds_known_set().
  PLUGIN_DIR: PLUGIN_DIR.
  SCAFFOLDS_WITHOUT_EXT.SCAFFOLDS_WITHOUT_EXT: SCAFFOLDS_WITHOUT_EXT.SCAFFOLDS_WITHOUT_EXT.
---
# Module: [`tests/unit/test_lang_extension_map.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_lang_extension_map.py)

## Functions
- `_discover_plugin_languages()` — [`L61`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_lang_extension_map.py#L61) — Return the language tokens of every plugin under languages/.
- `test_ast_cache_alias_matches_canonical()` — [`L121`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_lang_extension_map.py#L121)
- `test_discover_plugin_languages_finds_known_set()` — [`L203`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_lang_extension_map.py#L203) — Sanity-check: discovery returns the expected languages.
- `test_every_plugin_has_extension_wiring()` — [`L101`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_lang_extension_map.py#L101) — Every plugin must be reachable via at least one file extension.
- `test_long_broken_extensions_stay_wired(ext: str, expected: str)` — [`L163`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_lang_extension_map.py#L163)
- `test_project_graph_alias_resolves_via_canonical()` — [`L132`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_lang_extension_map.py#L132)
- `test_swiftinterface_resolves_in_all_known_ext_maps()` — [`L173`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_lang_extension_map.py#L173) — ``.swiftinterface`` must map to swift across every ext-resolver.

## Module values
- `PLUGIN_DIR` — [`L31`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_lang_extension_map.py#L31)
- `SCAFFOLDS_WITHOUT_EXT` — [`L37`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_lang_extension_map.py#L37)

