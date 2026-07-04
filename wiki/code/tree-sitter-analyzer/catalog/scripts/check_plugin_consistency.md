---
title: 'Module: scripts/check_plugin_consistency.py'
type: catalog
provenance: extracted
module: scripts/check_plugin_consistency.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `scripts.check_plugin_consistency`/
symbols:
  CHECKS: CHECKS.
  main: main().
  check_no_new_single_file_plugins: check_no_new_single_file_plugins().
  PLUGINS_DIR: PLUGINS_DIR.
  _discover_plugins: _discover_plugins().
  check_required_methods: check_required_methods().
  BASE_PLUGIN: BASE_PLUGIN.
  PROJECT_ROOT: PROJECT_ROOT.
  REQUIRED_PLUGIN_METHODS: REQUIRED_PLUGIN_METHODS.
  GRANDFATHERED_SINGLE_FILE: GRANDFATHERED_SINGLE_FILE.
  check_extract_elements_return_type: check_extract_elements_return_type().
  check_plugin_inheritance: check_plugin_inheritance().
  check_analyze_file_delegation: check_analyze_file_delegation().
---
# Module: [`scripts/check_plugin_consistency.py`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_plugin_consistency.py)

## Functions
- `_discover_plugins()` — [`L47`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_plugin_consistency.py#L47)
- `check_analyze_file_delegation(lang: str, path: Path)` — [`L134`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_plugin_consistency.py#L134)
- `check_extract_elements_return_type(lang: str, path: Path)` — [`L61`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_plugin_consistency.py#L61)
- `check_no_new_single_file_plugins()` — [`L119`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_plugin_consistency.py#L119)
- `check_plugin_inheritance(lang: str, path: Path)` — [`L82`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_plugin_consistency.py#L82)
- `check_required_methods(lang: str, path: Path)` — [`L100`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_plugin_consistency.py#L100)
- `main()` — [`L170`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_plugin_consistency.py#L170)

## Module values
- `BASE_PLUGIN` — [`L21`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_plugin_consistency.py#L21)
- `CHECKS` — [`L162`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_plugin_consistency.py#L162)
- `GRANDFATHERED_SINGLE_FILE` — [`L30`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_plugin_consistency.py#L30)
- `PLUGINS_DIR` — [`L20`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_plugin_consistency.py#L20)
- `PROJECT_ROOT` — [`L19`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_plugin_consistency.py#L19)
- `REQUIRED_PLUGIN_METHODS` — [`L23`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_plugin_consistency.py#L23)

