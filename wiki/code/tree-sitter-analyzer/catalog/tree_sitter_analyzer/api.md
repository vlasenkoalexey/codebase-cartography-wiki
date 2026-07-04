---
title: 'Module: tree_sitter_analyzer/api.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/api.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.api`/
symbols:
  analyze_file: analyze_file().
  analyze_code: analyze_code().
  get_engine: get_engine().
  _analyze_file_sync: _analyze_file_sync().
  execute_query: execute_query().
  validate_file: validate_file().
  extract_elements: extract_elements().
  detect_language: detect_language().
  get_framework_info: get_framework_info().
  get_supported_languages: get_supported_languages().
  get_file_extensions: get_file_extensions().
  _group_captures_by_main_node: _group_captures_by_main_node().
  get_available_queries: get_available_queries().
  is_language_supported: is_language_supported().
  _engine._engine: _engine._engine.
  analyze: analyze().
  get_languages: get_languages().
  logger: logger.
---
# Module: [`tree_sitter_analyzer/api.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/api.py)

## Functions
- `_analyze_file_sync(file_path: str | Path, language: str | None, queries: list[str] | None, include_elements: bool, include_queries: bool)` — [`L60`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/api.py#L60)
- `_group_captures_by_main_node(captures: list[dict[str, Any]])` — [`L40`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/api.py#L40) — Backward-compatible private alias used by legacy tests and callers.
- `analyze(file_path: str | Path, **kwargs: Any)` — [`L430`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/api.py#L430) — Convenience function that aliases to analyze_file.
- `analyze_code(source_code: str, language: str, queries: list[str] | None = None, include_elements: bool = True, include_queries: bool = True)` — [`L128`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/api.py#L128) — Analyze source code directly (without file).
- `analyze_file(file_path: str | Path, language: str | None = None, queries: list[str] | None = None, include_elements: bool = True, include_details: bool = False, include_queries: bool = True, include_complexity: bool = False)` — [`L85`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/api.py#L85) — Analyze a source code file.
- `detect_language(file_path: str | Path)` — [`L220`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/api.py#L220) — Detect programming language from file path.
- `execute_query(file_path: str | Path, query_name: str, language: str | None = None)` — [`L349`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/api.py#L349) — Execute a specific query against a file.
- `extract_elements(file_path: str | Path, language: str | None = None, element_types: list[str] | None = None)` — [`L385`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/api.py#L385) — Extract code elements from a file.
- `get_available_queries(language: str)` — [`L183`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/api.py#L183) — Get available queries for a specific language.
- `get_engine()` — [`L47`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/api.py#L47) — Get the global analysis engine instance.
- `get_file_extensions(language: str)` — [`L249`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/api.py#L249) — Get file extensions for a specific language.
- `get_framework_info()` — [`L312`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/api.py#L312) — Get information about the framework and its capabilities.
- `get_languages()` — [`L435`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/api.py#L435) — Convenience function that aliases to get_supported_languages.
- `get_supported_languages()` — [`L168`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/api.py#L168) — Get list of all supported programming languages.
- `is_language_supported(language: str)` — [`L201`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/api.py#L201) — Check if a programming language is supported.
- `validate_file(file_path: str | Path)` — [`L283`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/api.py#L283) — Validate a source code file without full analysis.

## Module values
- `_engine` — [`L37`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/api.py#L37)
- `logger` — [`L34`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/api.py#L34)

