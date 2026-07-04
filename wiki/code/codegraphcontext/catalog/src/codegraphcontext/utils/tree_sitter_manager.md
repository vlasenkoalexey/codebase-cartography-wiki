---
title: 'Module: src/codegraphcontext/utils/tree_sitter_manager.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/utils/tree_sitter_manager.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.utils.tree_sitter_manager`/
symbols:
  execute_query: execute_query().
  TreeSitterManager.get_language_safe: TreeSitterManager#get_language_safe().
  _load_tree_sitter_dependencies: _load_tree_sitter_dependencies().
  get_tree_sitter_manager: get_tree_sitter_manager().
  _manager_instance._manager_instance: _manager_instance._manager_instance.
  TreeSitterManager.create_parser: TreeSitterManager#create_parser().
  _Language: _Language.
  _Parser: _Parser.
  _get_language: _get_language.
  LANGUAGE_ALIASES: LANGUAGE_ALIASES.
  TreeSitterManager._language_cache: TreeSitterManager#_language_cache.
  get_language_safe: get_language_safe().
  create_parser: create_parser().
  TreeSitterManager._normalize_language_name: TreeSitterManager#_normalize_language_name().
  LANGUAGE_PACK_NAMES: LANGUAGE_PACK_NAMES.
  TreeSitterManager: TreeSitterManager#
  TreeSitterManager.is_language_available: TreeSitterManager#is_language_available().
  TreeSitterManager.get_supported_languages: TreeSitterManager#get_supported_languages().
  _missing_tree_sitter_error: _missing_tree_sitter_error().
  _tree_sitter_import_error._tree_sitter_import_error: _tree_sitter_import_error._tree_sitter_import_error.
  TreeSitterManager._cache_lock: TreeSitterManager#_cache_lock.
  _instance_lock: _instance_lock.
  TreeSitterManager.__init__: TreeSitterManager#__init__().
---
# Module: [`src/codegraphcontext/utils/tree_sitter_manager.py`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/utils/tree_sitter_manager.py)

## Classes
### `TreeSitterManager`
- def: [`src/codegraphcontext/utils/tree_sitter_manager.py:136`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/utils/tree_sitter_manager.py#L136)
- doc: Manages tree-sitter language loading and parser creation.
- signature: `class TreeSitterManager:`
- members:
  - `__init__(self)` — [`L147`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/utils/tree_sitter_manager.py#L147) — Initialize the tree-sitter manager.
  - `_normalize_language_name(self, lang: str)` — [`L152`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/utils/tree_sitter_manager.py#L152) — Normalize a language name to its canonical form.
  - `create_parser(self, lang: str)` — [`L220`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/utils/tree_sitter_manager.py#L220) — Create a new Parser instance for the specified language.
  - `get_language_safe(self, lang: str)` — [`L173`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/utils/tree_sitter_manager.py#L173) — Get a cached Language object for the specified language. — documented in [codegraphcontext-utils-tree_sitter_manager](../../../../concepts/codegraphcontext-utils-tree_sitter_manager.md)
  - `get_supported_languages(self)` — [`L271`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/utils/tree_sitter_manager.py#L271) — Get a list of all supported language names.
  - `is_language_available(self, lang: str)` — [`L255`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/utils/tree_sitter_manager.py#L255) — Check if a language is available without raising exceptions.
- protocol/private: `_cache_lock`[`L150`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/utils/tree_sitter_manager.py#L150), `_language_cache`[`L149`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/utils/tree_sitter_manager.py#L149)
- uses (calls/refs, reference-scoped): [`_load_tree_sitter_dependencies`](tree_sitter_manager.md#_load_tree_sitter_dependencies), [`LANGUAGE_ALIASES`](tree_sitter_manager.md#LANGUAGE_ALIASES), [`LANGUAGE_PACK_NAMES`](tree_sitter_manager.md#LANGUAGE_PACK_NAMES)
- used by: [`get_tree_sitter_manager`](tree_sitter_manager.md#get_tree_sitter_manager), [`_manager_instance`](tree_sitter_manager.md#_manager_instance._manager_instance), [`create_parser`](tree_sitter_manager.md#create_parser), [`get_language_safe`](tree_sitter_manager.md#get_language_safe), [`language`](../tools/tree_sitter_parser.md#TreeSitterParser.language), [`parser`](../tools/tree_sitter_parser.md#TreeSitterParser.parser)

## Functions
- `_load_tree_sitter_dependencies()` — [`L46`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/utils/tree_sitter_manager.py#L46) — Load optional tree-sitter dependencies only when parsing is used. — documented in [codegraphcontext-utils-tree_sitter_manager](../../../../concepts/codegraphcontext-utils-tree_sitter_manager.md)
- `_missing_tree_sitter_error(import_error: ImportError)` — [`L32`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/utils/tree_sitter_manager.py#L32) — Return an actionable error for optional tree-sitter dependencies. — documented in [codegraphcontext-tools-languages-typescript](../../../../concepts/codegraphcontext-tools-languages-typescript.md)
- `create_parser(lang: str)` — [`L310`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/utils/tree_sitter_manager.py#L310) — Create a new Parser for the language. Each call returns a new parser.
- `execute_query(language: Language, query_string: str, node)` — [`L315`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/utils/tree_sitter_manager.py#L315) — Execute a tree-sitter query and return captures in backward-compatible format. — documented in [codegraphcontext-tools-languages-kotlin](../../../../concepts/codegraphcontext-tools-languages-kotlin.md)
- `get_language_safe(lang: str)` — [`L305`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/utils/tree_sitter_manager.py#L305) — Get a cached Language object. Thread-safe.
- `get_tree_sitter_manager()` — [`L286`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/utils/tree_sitter_manager.py#L286) — Get the global TreeSitterManager instance (singleton pattern). — documented in [codegraphcontext-utils-tree_sitter_manager](../../../../concepts/codegraphcontext-utils-tree_sitter_manager.md)

## Module values
- `LANGUAGE_ALIASES` — [`L80`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/utils/tree_sitter_manager.py#L80)
- `LANGUAGE_PACK_NAMES` — [`L131`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/utils/tree_sitter_manager.py#L131)
- `_Language` — [`L27`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/utils/tree_sitter_manager.py#L27)
- `_Parser` — [`L28`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/utils/tree_sitter_manager.py#L28)
- `_get_language` — [`L29`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/utils/tree_sitter_manager.py#L29)
- `_instance_lock` — [`L283`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/utils/tree_sitter_manager.py#L283)
- `_manager_instance` — [`L282`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/utils/tree_sitter_manager.py#L282)
- `_tree_sitter_import_error` — [`L26`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/utils/tree_sitter_manager.py#L26)

