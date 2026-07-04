---
title: 'Module: tree_sitter_analyzer/query_loader.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/query_loader.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.query_loader`/
symbols:
  query_loader: query_loader.
  QueryLoader.load_language_queries: QueryLoader#load_language_queries().
  get_query_loader: get_query_loader().
  QueryLoader: QueryLoader#
  QueryLoader.get_query_description: QueryLoader#get_query_description().
  get_query: get_query().
  QueryLoader.get_query: QueryLoader#get_query().
  QueryLoader._loaded_queries: QueryLoader#_loaded_queries.
  QueryLoader.is_language_supported: QueryLoader#is_language_supported().
  list_queries: list_queries().
  is_language_supported: is_language_supported().
  QueryLoader.refresh_cache: QueryLoader#refresh_cache().
  QueryLoader._failed_languages: QueryLoader#_failed_languages.
  QueryLoader.list_queries_for_language: QueryLoader#list_queries_for_language().
  QueryLoader.list_supported_languages: QueryLoader#list_supported_languages().
  QueryLoader.list_queries: QueryLoader#list_queries().
  QueryLoader.get_all_queries_for_language: QueryLoader#get_all_queries_for_language().
  list_supported_languages: list_supported_languages().
  QueryLoader._query_modules: QueryLoader#_query_modules.
  QueryLoader.preload_languages: QueryLoader#preload_languages().
  _query_loader_instance: _query_loader_instance.
  QueryLoader._QUERY_DESCRIPTIONS: QueryLoader#_QUERY_DESCRIPTIONS.
  QueryLoader.get_common_queries: QueryLoader#get_common_queries().
  _populate_queries_from_module: _populate_queries_from_module().
  QueryLoader._PREDEFINED_QUERIES: QueryLoader#_PREDEFINED_QUERIES.
  _query_loader_instance_lock: _query_loader_instance_lock.
  QueryLoader.__init__: QueryLoader#__init__().
---
# Module: [`tree_sitter_analyzer/query_loader.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/query_loader.py)

## Classes
### `QueryLoader`
- def: [`tree_sitter_analyzer/query_loader.py:39`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/query_loader.py#L39)
- doc: Load and manage language-specific Tree-sitter queries with optimizations.
- signature: `class QueryLoader:`
- members:
  - `get_all_queries_for_language(self, language: str)` — [`L211`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/query_loader.py#L211) — Get all query information for a language including metadata.
  - `get_common_queries(self)` — [`L206`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/query_loader.py#L206) — Get commonly used queries across languages.
  - `get_query(self, language: str, query_name: str)` — [`L119`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/query_loader.py#L119) — Get a specific query for a language with optimized lookup.
  - `get_query_description(self, language: str, query_name: str)` — [`L136`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/query_loader.py#L136) — Get description for a specific query.
  - `is_language_supported(self, language: str)` — [`L239`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/query_loader.py#L239) — Check if a language has query support.
  - `list_queries(self, language: str)` — [`L160`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/query_loader.py#L160) — List all available queries for a language.
  - `list_queries_for_language(self, language: str)` — [`L151`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/query_loader.py#L151) — List all available queries for a language.
  - `list_supported_languages(self)` — [`L171`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/query_loader.py#L171) — List all languages that have query modules available.
  - `load_language_queries(self, language: str)` — [`L83`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/query_loader.py#L83) — Load queries for a specific language with optimized caching.
  - `preload_languages(self, languages: list[str])` — [`L245`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/query_loader.py#L245) — Preload queries for multiple languages efficiently.
  - `refresh_cache(self)` — [`L232`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/query_loader.py#L232) — Refresh the query cache.
- protocol/private: `_PREDEFINED_QUERIES`[`L43`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/query_loader.py#L43), `_QUERY_DESCRIPTIONS`[`L62`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/query_loader.py#L62), `__init__`[`L78`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/query_loader.py#L78), `_failed_languages`[`L81`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/query_loader.py#L81), `_loaded_queries`[`L79`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/query_loader.py#L79), `_query_modules`[`L80`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/query_loader.py#L80)
- uses (calls/refs, reference-scoped): [`log_error`](utils/logging.md#log_error), [`_populate_queries_from_module`](query_loader.md#_populate_queries_from_module)
- used by: [`execute`](cli/info_commands.md#DescribeQueryCommand.execute), [`get_query_loader`](query_loader.md#get_query_loader), [`get_query`](query_loader.md#get_query), [`get_available_queries`](core/query.md#QueryExecutor.get_available_queries), [`get_available_queries`](core/query.md#get_available_queries), [`_emit_text_query_block`](cli/info_commands.md#ListQueriesCommand._emit_text_query_block), [`get_available_queries`](core/query_service.md#QueryService.get_available_queries), [`is_language_supported`](query_loader.md#is_language_supported), [`list_queries`](query_loader.md#list_queries), [`get_query_description`](core/query.md#QueryExecutor.get_query_description), [`_emit_text_all_languages`](cli/info_commands.md#ListQueriesCommand._emit_text_all_languages), [`query_loader`](cli/__init__.md#query_loader), [`_collect_query_descriptions`](cli/info_commands.md#ListQueriesCommand._collect_query_descriptions), [`get_query_description`](core/query.md#get_query_description), [`_attach_available_queries`](mcp/tools/analyze_scale_helpers.md#_attach_available_queries), [`_build_all_languages_envelope`](cli/info_commands.md#ListQueriesCommand._build_all_languages_envelope), [`get_query_description`](core/query_service.md#QueryService.get_query_description), [`list_supported_languages`](query_loader.md#list_supported_languages), [`resolve_query_string`](core/query_executor.md#resolve_query_string)  (45 test-only)

## Functions
- `_populate_queries_from_module(module: Any, queries: dict[str, str])` — [`L14`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/query_loader.py#L14) — Extract queries from a language module into ``queries`` in-place.
- `get_query(language: str, query_name: str)` — [`L276`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/query_loader.py#L276) — Get a specific query.
- `get_query_loader()` — [`L262`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/query_loader.py#L262) — Get singleton query loader instance.
- `is_language_supported(language: str)` — [`L291`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/query_loader.py#L291) — Check if language is supported.
- `list_queries(language: str)` — [`L281`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/query_loader.py#L281) — List queries for a language.
- `list_supported_languages()` — [`L286`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/query_loader.py#L286) — List all supported languages.

## Module values
- `_query_loader_instance` — [`L258`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/query_loader.py#L258)
- `_query_loader_instance_lock` — [`L259`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/query_loader.py#L259)
- `query_loader` — [`L272`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/query_loader.py#L272)

