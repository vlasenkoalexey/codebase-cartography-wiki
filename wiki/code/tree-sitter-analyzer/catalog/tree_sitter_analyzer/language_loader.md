---
title: 'Module: tree_sitter_analyzer/language_loader.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/language_loader.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.language_loader`/
symbols:
  LanguageLoader: LanguageLoader#
  loader: loader.
  LanguageLoader.load_language: LanguageLoader#load_language().
  LanguageLoader.is_language_available: LanguageLoader#is_language_available().
  LanguageLoader.create_parser_safely: LanguageLoader#create_parser_safely().
  get_loader: get_loader().
  LanguageLoader._unavailable_languages: LanguageLoader#_unavailable_languages.
  LanguageLoader._availability_cache: LanguageLoader#_availability_cache.
  LanguageLoader.LANGUAGE_MODULES: LanguageLoader#LANGUAGE_MODULES.
  grammar_install_hint: grammar_install_hint().
  create_parser_safely: create_parser_safely().
  LanguageLoader.clear_cache: LanguageLoader#clear_cache().
  LanguageLoader.get_supported_languages: LanguageLoader#get_supported_languages().
  LanguageLoader._loaded_languages: LanguageLoader#_loaded_languages.
  load_language: load_language().
  TREE_SITTER_AVAILABLE: TREE_SITTER_AVAILABLE.
  check_language_availability: check_language_availability().
  LanguageLoader._parser_cache: LanguageLoader#_parser_cache.
  LanguageLoader._loaded_modules: LanguageLoader#_loaded_modules.
  LanguageLoader.TYPESCRIPT_DIALECTS: LanguageLoader#TYPESCRIPT_DIALECTS.
  is_grammar_installed: is_grammar_installed().
  _try_wrap_language: _try_wrap_language().
  LanguageLoader.SUPPORTED_LANGUAGES: LanguageLoader#SUPPORTED_LANGUAGES().
  LanguageLoader.create_parser: LanguageLoader#create_parser().
  _loader_instance: _loader_instance.
  LanguageLoader._bind_parser_language: LanguageLoader#_bind_parser_language().
  _loader_instance_lock: _loader_instance_lock.
  _GRAMMAR_EXTRAS._GRAMMAR_EXTRAS: _GRAMMAR_EXTRAS._GRAMMAR_EXTRAS.
  LanguageLoader.__init__: LanguageLoader#__init__().
---
# Module: [`tree_sitter_analyzer/language_loader.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/language_loader.py)

## Classes
### `LanguageLoader`
- def: [`tree_sitter_analyzer/language_loader.py:42`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/language_loader.py#L42) — documented in [tree_sitter_analyzer-core-parser](../../concepts/tree_sitter_analyzer-core-parser.md)
- doc: Optimized language loader with enhanced caching
- signature: `class LanguageLoader:`
- members:
  - `SUPPORTED_LANGUAGES(self)` — [`L79`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/language_loader.py#L79) — サポートされている言語のリストを取得するプロパティ
  - `__init__(self)` — [`L83`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/language_loader.py#L83) — ローダーを初期化（最適化：事前キャッシュ容量指定）
  - `_bind_parser_language(parser: Any, tree_sitter_language: Any, language: str)` — [`L243`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/language_loader.py#L243) — Set the language on ``parser`` using whichever API the build exposes.
  - `clear_cache(self)` — [`L288`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/language_loader.py#L288) — キャッシュをクリア（メモリ管理用）
  - `create_parser(self, language: str)` — [`L238`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/language_loader.py#L238) — Create a parser for the specified language (alias for create_parser_safely)
  - `create_parser_safely(self, language: str)` — [`L194`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/language_loader.py#L194) — Create a parser for the specified language with error handling — documented in [tree_sitter_analyzer-core-parser](../../concepts/tree_sitter_analyzer-core-parser.md)
  - `get_supported_languages(self)` — [`L273`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/language_loader.py#L273) — サポートされている言語のリストを取得（最適化：結果キャッシュ）
  - `is_language_available(self, language: str)` — [`L91`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/language_loader.py#L91) — 指定された言語のライブラリが利用可能かチェック — documented in [tree_sitter_analyzer-core-parser](../../concepts/tree_sitter_analyzer-core-parser.md)
  - `load_language(self, language: str)` — [`L128`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/language_loader.py#L128) — Load and return a tree-sitter Language object for the specified language — documented in [tree_sitter_analyzer-core-parser](../../concepts/tree_sitter_analyzer-core-parser.md)
  - `LANGUAGE_MODULES` — [`L46`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/language_loader.py#L46)
  - `TYPESCRIPT_DIALECTS` — [`L76`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/language_loader.py#L76)
- protocol/private: `_availability_cache`[`L87`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/language_loader.py#L87), `_loaded_languages`[`L85`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/language_loader.py#L85), `_loaded_modules`[`L86`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/language_loader.py#L86), `_parser_cache`[`L88`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/language_loader.py#L88), `_unavailable_languages`[`L89`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/language_loader.py#L89)
- uses (calls/refs, reference-scoped): [`log_warning`](utils/logging.md#log_warning), [`TREE_SITTER_AVAILABLE`](language_loader.md#TREE_SITTER_AVAILABLE), [`_try_wrap_language`](language_loader.md#_try_wrap_language)
- used by: [`_get_covered_node_types_from_plugin`](grammar_coverage/validator.md#_get_covered_node_types_from_plugin), [`parse_code`](core/parser.md#Parser.parse_code), [`get_loader`](language_loader.md#get_loader), [`enumerate_syntax_paths`](grammar_coverage/auto_discovery.md#AutoDiscoveryEngine.enumerate_syntax_paths), [`is_language_supported`](core/parser.md#Parser.is_language_supported), [`create_parser_safely`](language_loader.md#create_parser_safely), [`get_tree_sitter_language`](languages/typescript_plugin/plugin.md#TypeScriptPlugin.get_tree_sitter_language), [`get_all_field_names`](grammar_coverage/auto_discovery.md#AutoDiscoveryEngine.get_all_field_names), [`validate_query`](core/query.md#QueryExecutor.validate_query), [`_parse_corpus_file`](grammar_coverage/validator.md#_parse_corpus_file), [`get_tree_sitter_language`](languages/javascript_plugin/plugin.md#JavaScriptPlugin.get_tree_sitter_language), [`_load_language_objects`](grammar_coverage/auto_discovery.md#_load_language_objects), [`load_language`](language_loader.md#load_language), [`check_language_availability`](language_loader.md#check_language_availability), [`get_supported_languages`](core/parser.md#Parser.get_supported_languages), [`_collect_loader_modules`](cli/parser_readiness_sources.md#_collect_loader_modules), [`_grammar_install_state`](cli/info_commands.md#_grammar_install_state), [`is_grammar_installed`](language_loader.md#is_grammar_installed), [`_get_package_version`](grammar_coverage/grammar_snapshot.md#_get_package_version)  (67 test-only)

## Functions
- `_try_wrap_language(caps_or_lang: Any, language: str)` — [`L27`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/language_loader.py#L27) — Wrap a PyCapsule in tree_sitter.Language; return None on failure.
- `check_language_availability(language: str)` — [`L317`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/language_loader.py#L317) — 言語の利用可能性をチェック
- `create_parser_safely(language: str)` — [`L322`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/language_loader.py#L322) — 安全にパーサーを作成
- `get_loader()` — [`L304`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/language_loader.py#L304) — Get singleton loader instance
- `grammar_install_hint(language: str)` — [`L365`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/language_loader.py#L365) — Return a pip-install instruction for a language's grammar, or None.
- `is_grammar_installed(language: str)` — [`L385`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/language_loader.py#L385) — Return True if the grammar module for *language* can be found.
- `load_language(language: str)` — [`L327`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/language_loader.py#L327) — 言語をロード

## Module values
- `TREE_SITTER_AVAILABLE` — [`L20`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/language_loader.py#L20)
- `_GRAMMAR_EXTRAS` — [`L337`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/language_loader.py#L337)
- `_loader_instance` — [`L300`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/language_loader.py#L300)
- `_loader_instance_lock` — [`L301`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/language_loader.py#L301)
- `loader` — [`L314`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/language_loader.py#L314)

