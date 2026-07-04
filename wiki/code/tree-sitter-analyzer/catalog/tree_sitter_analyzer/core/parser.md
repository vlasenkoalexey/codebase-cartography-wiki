---
title: 'Module: tree_sitter_analyzer/core/parser.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/core/parser.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.core.parser`/
symbols:
  Parser: Parser#
  ParseResult.tree: ParseResult#tree.
  Parser.parse_code: Parser#parse_code().
  ParseResult.success: ParseResult#success.
  Parser.parse_file: Parser#parse_file().
  ParseResult: ParseResult#
  ParseResult.error_message: ParseResult#error_message.
  ParseResult.source_code: ParseResult#source_code.
  _failed_parse: _failed_parse().
  Parser._cache_lookup: Parser#_cache_lookup().
  ParseResult.language: ParseResult#language.
  Parser.cache_info: Parser#cache_info().
  Parser.cache_clear: Parser#cache_clear().
  ParseResult.file_path: ParseResult#file_path.
  Parser.is_language_supported: Parser#is_language_supported().
  Parser._cache: Parser#_cache.
  Parser._read_source_code: Parser#_read_source_code().
  Parser._loader: Parser#_loader.
  logger: logger.
  Parser.get_supported_languages: Parser#get_supported_languages().
  Parser._encoding_manager: Parser#_encoding_manager.
  Parser.get_parse_errors: Parser#get_parse_errors().
  Parser._lookup_or_record_stat_key: Parser#_lookup_or_record_stat_key().
  Parser.validate_ast: Parser#validate_ast().
  _collect_error_nodes: _collect_error_nodes().
  loader: loader.
  Parser._stat_cache: Parser#_stat_cache.
  Parser._hits: Parser#_hits.
  Parser._misses: Parser#_misses.
  Parser._stat_hits: Parser#_stat_hits.
  _error_node_payload: _error_node_payload().
  _PARSER_CACHE_SIZE: _PARSER_CACHE_SIZE.
  Parser.__init__: Parser#__init__().
---
# Module: [`tree_sitter_analyzer/core/parser.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/parser.py)

## Classes
### `ParseResult`
- def: [`tree_sitter_analyzer/core/parser.py:84`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/parser.py#L84) — documented in [tree_sitter_analyzer-ast_diff](../../../concepts/tree_sitter_analyzer-ast_diff.md)
- members:
  - `error_message` — [`L102`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/parser.py#L102) — documented in [tree_sitter_analyzer-ast_diff](../../../concepts/tree_sitter_analyzer-ast_diff.md)
  - `file_path` — [`L100`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/parser.py#L100)
  - `language` — [`L99`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/parser.py#L99)
  - `source_code` — [`L98`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/parser.py#L98)
  - `success` — [`L101`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/parser.py#L101) — documented in [tree_sitter_analyzer-ast_diff](../../../concepts/tree_sitter_analyzer-ast_diff.md)
  - `tree` — [`L97`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/parser.py#L97) — documented in [tree_sitter_analyzer-ast_cache](../../../concepts/tree_sitter_analyzer-ast_cache.md)
- used by: [`build`](../call_graph.md#CallGraph.build), [`parse_code`](parser.md#Parser.parse_code), [`execute_query`](query_service.md#QueryService.execute_query), [`diff_strings`](../ast_diff.md#ASTDiffer.diff_strings), [`analyze_file_complexity`](../complexity_heatmap.md#analyze_file_complexity), [`parse_file`](parser.md#Parser.parse_file), [`detect_structural_clones_cached`](../code_similarity.md#detect_structural_clones_cached), [`analyze_file`](../languages/sql_plugin/plugin.md#SQLPlugin.analyze_file), [`detect_structural_clones`](../code_similarity.md#detect_structural_clones), [`find_unused_imports`](../dead_code_analyzer.md#find_unused_imports), [`extract_imports_from_file`](../project_graph.md#extract_imports_from_file), [`find_unreferenced_variables`](../dead_code_analyzer.md#find_unreferenced_variables), [`_worker_index_file`](../_ast_extraction.md#_worker_index_file), [`extract_top_level_defs_from_file`](../symbol_extractors.md#extract_top_level_defs_from_file), [`is_file_parse_broken`](../mcp/tools/utils/parse_validity.md#is_file_parse_broken), [`_parse`](../ast_path.md#ASTPathNavigator._parse), [`_extract_function_bodies`](../code_similarity.md#_extract_function_bodies), [`_failed_parse`](parser.md#_failed_parse), [`_parse_file_for_state`](../uml_state.md#_parse_file_for_state), [`_cache_lookup`](parser.md#Parser._cache_lookup), [`score_structure`](../health_scorer.md#score_structure), [`_parse_file_for_activity`](../uml_activity.md#_parse_file_for_activity), [`_parse_tree`](../route_detector.md#RouteDetector._parse_tree), [`_is_null_byte_false_positive`](../mcp/tools/utils/parse_validity.md#_is_null_byte_false_positive), [`_read_source_code`](parser.md#Parser._read_source_code), [`_parse_tree`](../middleware_detector.md#MiddlewareDetector._parse_tree), [`_parse_tree`](../unreachable_code.md#_parse_tree)  (53 test-only)

### `Parser`
- def: [`tree_sitter_analyzer/core/parser.py:105`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/parser.py#L105) — documented in [tree_sitter_analyzer-ast_cache](../../../concepts/tree_sitter_analyzer-ast_cache.md)
- members:
  - `__init__(self)` — [`L125`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/parser.py#L125) — Initialize the Parser with language loader.
  - `_cache_lookup(self, file_path_str: str, language: str)` — [`L190`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/parser.py#L190) — Return ``(cache_key, cached_result_or_None)`` for the cache layer. — documented in [tree_sitter_analyzer-core-parser](../../../concepts/tree_sitter_analyzer-core-parser.md)
  - `_lookup_or_record_stat_key(self, file_path_str: str, mtime_ns: int, size: int, language: str)` — [`L217`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/parser.py#L217) — Return the cache key, reusing a prior stat hit when possible.
  - `_read_source_code(self, path_obj: Path, language: str)` — [`L236`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/parser.py#L236) — Read the file via the encoding manager, returning either source or a failed ParseResult.
  - `cache_clear(cls)` — [`L144`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/parser.py#L144) — Clear the parser cache. Used by tests and by tooling that knows
  - `cache_info(cls)` — [`L132`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/parser.py#L132) — Return cache occupancy and hit/miss counters for diagnostics.
  - `get_parse_errors(self, tree: Tree)` — [`L376`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/parser.py#L376) — Extract parse errors from a tree.
  - `get_supported_languages(self)` — [`L342`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/parser.py#L342) — Get list of supported programming languages.
  - `is_language_supported(self, language: str)` — [`L326`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/parser.py#L326) — Check if a programming language is supported.
  - `parse_code(self, source_code: str, language: str, filename: str | None = None)` — [`L256`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/parser.py#L256) — Parse source code string. — documented in [tree_sitter_analyzer-ast_cache](../../../concepts/tree_sitter_analyzer-ast_cache.md)
  - `parse_file(self, file_path: str | Path, language: str)` — [`L154`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/parser.py#L154) — Parse a source code file. — documented in [tree_sitter_analyzer-ast_cache](../../../concepts/tree_sitter_analyzer-ast_cache.md)
  - `validate_ast(self, tree: Tree | None)` — [`L355`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/parser.py#L355) — Validate an AST tree.
- protocol/private: `_cache`[`L115`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/parser.py#L115), `_encoding_manager`[`L128`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/parser.py#L128), `_hits`[`L121`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/parser.py#L121), `_loader`[`L127`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/parser.py#L127), `_misses`[`L122`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/parser.py#L122), `_stat_cache`[`L119`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/parser.py#L119), `_stat_hits`[`L123`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/parser.py#L123)
- uses (calls/refs, reference-scoped): [`tree`](parser.md#ParseResult.tree), [`EncodingManager`](../encoding_utils.md#EncodingManager), [`success`](parser.md#ParseResult.success), [`is_language_available`](../language_loader.md#LanguageLoader.is_language_available), [`ParseResult`](parser.md#ParseResult), [`error_message`](parser.md#ParseResult.error_message), [`create_parser_safely`](../language_loader.md#LanguageLoader.create_parser_safely), [`source_code`](parser.md#ParseResult.source_code), [`get_loader`](../language_loader.md#get_loader), [`_failed_parse`](parser.md#_failed_parse), [`read_file_safe`](../encoding_utils.md#EncodingManager.read_file_safe), [`safe_encode`](../encoding_utils.md#EncodingManager.safe_encode), [`language`](parser.md#ParseResult.language), [`file_path`](parser.md#ParseResult.file_path), [`grammar_install_hint`](../language_loader.md#grammar_install_hint), [`get_supported_languages`](../language_loader.md#LanguageLoader.get_supported_languages), [`logger`](parser.md#logger), [`_collect_error_nodes`](parser.md#_collect_error_nodes), [`is_grammar_installed`](../language_loader.md#is_grammar_installed), [`_PARSER_CACHE_SIZE`](parser.md#_PARSER_CACHE_SIZE)
- used by: [`build`](../call_graph.md#CallGraph.build), [`execute_query`](query_service.md#QueryService.execute_query), [`diff_strings`](../ast_diff.md#ASTDiffer.diff_strings), [`analyze_file_complexity`](../complexity_heatmap.md#analyze_file_complexity), [`detect_structural_clones_cached`](../code_similarity.md#detect_structural_clones_cached), [`analyze_file`](../languages/sql_plugin/plugin.md#SQLPlugin.analyze_file), [`detect_structural_clones`](../code_similarity.md#detect_structural_clones), [`find_unused_imports`](../dead_code_analyzer.md#find_unused_imports), [`_ensure_initialized`](analysis_engine.md#UnifiedAnalysisEngine._ensure_initialized), [`extract_imports_from_file`](../project_graph.md#extract_imports_from_file), [`find_unreferenced_variables`](../dead_code_analyzer.md#find_unreferenced_variables), [`_worker_index_file`](../_ast_extraction.md#_worker_index_file), [`extract_top_level_defs_from_file`](../symbol_extractors.md#extract_top_level_defs_from_file), [`is_file_parse_broken`](../mcp/tools/utils/parse_validity.md#is_file_parse_broken), [`_parse`](../ast_path.md#ASTPathNavigator._parse), [`_extract_function_bodies`](../code_similarity.md#_extract_function_bodies), [`_parse_file_for_state`](../uml_state.md#_parse_file_for_state), [`score_structure`](../health_scorer.md#score_structure), [`_parse_file_for_activity`](../uml_activity.md#_parse_file_for_activity), [`_parse_tree`](../route_detector.md#RouteDetector._parse_tree), [`_is_null_byte_false_positive`](../mcp/tools/utils/parse_validity.md#_is_null_byte_false_positive), [`_parse_tree`](../middleware_detector.md#MiddlewareDetector._parse_tree), [`parser`](query_service.md#QueryService.parser), [`_parse_tree`](../unreachable_code.md#_parse_tree), [`_worker_parser`](../_ast_extraction.md#_worker_parser._worker_parser), [`_init_worker_parser`](../_ast_extraction.md#_init_worker_parser), [`parser`](../ast_cache.md#ASTCache.parser), [`_parser`](../ast_cache.md#ASTCache._parser), [`_parser`](../ast_path.md#ASTPathNavigator._parser), [`_parser`](../middleware_detector.md#MiddlewareDetector._parser), [`_parser`](../route_detector.md#RouteDetector._parser), [`__init__`](../ast_diff.md#ASTDiffer.__init__)  (70 test-only)

## Functions
- `_collect_error_nodes(node: Any, errors: list[dict[str, Any]])` — [`L25`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/parser.py#L25) — Recursively walk a tree-sitter node, appending ERROR nodes to ``errors``.
- `_error_node_payload(node: Any)` — [`L39`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/parser.py#L39) — Build the canonical ``{type, start_point, end_point, text}`` dict.
- `_failed_parse(language: str, file_path: str, error_message: str)` — [`L52`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/parser.py#L52) — Return a ParseResult representing a failed parse — keeps callers terse.

## Module values
- `_PARSER_CACHE_SIZE` — [`L81`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/parser.py#L81)
- `loader` — [`L396`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/parser.py#L396)
- `logger` — [`L22`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/parser.py#L22)

