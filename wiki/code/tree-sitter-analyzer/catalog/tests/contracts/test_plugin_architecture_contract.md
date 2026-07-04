---
title: 'Module: tests/contracts/test_plugin_architecture_contract.py'
type: catalog
provenance: extracted
module: tests/contracts/test_plugin_architecture_contract.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.contracts.test_plugin_architecture_contract`/
symbols:
  PLUGINS_DIR: PLUGINS_DIR.
  _discover_plugin_files: _discover_plugin_files().
  test_every_plugin_class_inherits_language_plugin: test_every_plugin_class_inherits_language_plugin().
  test_extract_elements_returns_dict: test_extract_elements_returns_dict().
  test_plugin_has_required_abstract_methods: test_plugin_has_required_abstract_methods().
  PROJECT_ROOT: PROJECT_ROOT.
  test_no_new_single_file_plugins_in_languages_root: test_no_new_single_file_plugins_in_languages_root().
  test_analyze_file_uses_create_extractor: test_analyze_file_uses_create_extractor().
  SKIPPED_SCAN_DIRS: SKIPPED_SCAN_DIRS.
---
# Module: [`tests/contracts/test_plugin_architecture_contract.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/contracts/test_plugin_architecture_contract.py)

## Functions
- `_discover_plugin_files()` — [`L35`](../../../../../../raw/code/tree-sitter-analyzer/tests/contracts/test_plugin_architecture_contract.py#L35) — Return [(language_name, path), ...] for all plugin files.
- `test_analyze_file_uses_create_extractor()` — [`L151`](../../../../../../raw/code/tree-sitter-analyzer/tests/contracts/test_plugin_architecture_contract.py#L151) — All analyze_file methods must use create_extractor(), not self.extractor.
- `test_every_plugin_class_inherits_language_plugin()` — [`L50`](../../../../../../raw/code/tree-sitter-analyzer/tests/contracts/test_plugin_architecture_contract.py#L50) — All XxxPlugin classes must inherit from LanguagePlugin (not ElementExtractor).
- `test_extract_elements_returns_dict()` — [`L70`](../../../../../../raw/code/tree-sitter-analyzer/tests/contracts/test_plugin_architecture_contract.py#L70) — extract_elements on any class must return dict[str, list[Any]], not list.
- `test_no_new_single_file_plugins_in_languages_root()` — [`L116`](../../../../../../raw/code/tree-sitter-analyzer/tests/contracts/test_plugin_architecture_contract.py#L116) — Prevent adding new single-file plugins. New languages must use package structure.
- `test_plugin_has_required_abstract_methods()` — [`L89`](../../../../../../raw/code/tree-sitter-analyzer/tests/contracts/test_plugin_architecture_contract.py#L89) — Each plugin must implement: get_language_name, get_file_extensions, create_extractor, analyze_file.

## Module values
- `PLUGINS_DIR` — [`L33`](../../../../../../raw/code/tree-sitter-analyzer/tests/contracts/test_plugin_architecture_contract.py#L33)
- `PROJECT_ROOT` — [`L23`](../../../../../../raw/code/tree-sitter-analyzer/tests/contracts/test_plugin_architecture_contract.py#L23)
- `SKIPPED_SCAN_DIRS` — [`L24`](../../../../../../raw/code/tree-sitter-analyzer/tests/contracts/test_plugin_architecture_contract.py#L24)

