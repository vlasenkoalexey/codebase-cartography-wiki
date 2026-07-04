---
title: 'Module: tests/unit/test_scala_language_wiring.py'
type: catalog
provenance: extracted
module: tests/unit/test_scala_language_wiring.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_scala_language_wiring`/
symbols:
  _scala_node: _scala_node().
  test_ast_cache_indexes_scala_file: test_ast_cache_indexes_scala_file().
  test_scala_corpus_extracts_symbols: test_scala_corpus_extracts_symbols().
  test_loader_provides_scala_language: test_loader_provides_scala_language().
  test_ast_cache_path_excludes_method_local_given_and_type: test_ast_cache_path_excludes_method_local_given_and_type().
  test_ast_cache_symbol_name_degenerate_given_is_empty: test_ast_cache_symbol_name_degenerate_given_is_empty().
  test_sc_extension_stays_unknown: test_sc_extension_stays_unknown().
  test_ast_cache_symbol_from_node_object_is_class: test_ast_cache_symbol_from_node_object_is_class().
  test_ast_cache_symbol_from_node_enum_is_enum: test_ast_cache_symbol_from_node_enum_is_enum().
  test_ast_cache_symbol_from_node_rejects_non_class_like: test_ast_cache_symbol_from_node_rejects_non_class_like().
  test_ast_cache_symbol_name_uses_identifier_child_for_object: test_ast_cache_symbol_name_uses_identifier_child_for_object().
  test_ast_cache_symbol_name_named_given_via_type: test_ast_cache_symbol_name_named_given_via_type().
  test_ast_cache_given_type_text_resolves_tuple_type: test_ast_cache_given_type_text_resolves_tuple_type().
  test_ast_cache_given_type_text_resolves_generic_type: test_ast_cache_given_type_text_resolves_generic_type().
  _scala_node.find: _scala_node().find().
  test_extension_detects_scala: test_extension_detects_scala().
  test_lang_extension_map_has_scala: test_lang_extension_map_has_scala().
  CORPUS: CORPUS.
---
# Module: [`tests/unit/test_scala_language_wiring.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_scala_language_wiring.py)

## Functions
- `_scala_node(code: str, node_type: str)` — [`L144`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_scala_language_wiring.py#L144) — Return the first ``node_type`` node in a parsed Scala snippet.
- `find(node)` — [`L154`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_scala_language_wiring.py#L154)
- `test_ast_cache_given_type_text_resolves_generic_type()` — [`L241`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_scala_language_wiring.py#L241)
- `test_ast_cache_given_type_text_resolves_tuple_type()` — [`L233`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_scala_language_wiring.py#L233)
- `test_ast_cache_indexes_scala_file()` — [`L84`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_scala_language_wiring.py#L84) — The project indexer must index .scala files without errors.
- `test_ast_cache_path_excludes_method_local_given_and_type()` — [`L103`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_scala_language_wiring.py#L103) — #961: the shared ast_cache walk (``_extract_symbols``) must NOT emit a
- `test_ast_cache_symbol_from_node_enum_is_enum()` — [`L177`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_scala_language_wiring.py#L177)
- `test_ast_cache_symbol_from_node_object_is_class()` — [`L166`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_scala_language_wiring.py#L166)
- `test_ast_cache_symbol_from_node_rejects_non_class_like()` — [`L188`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_scala_language_wiring.py#L188) — A node outside ``_SCALA_CLASS_LIKE`` (e.g. the bare ``enum`` keyword)
- `test_ast_cache_symbol_name_degenerate_given_is_empty()` — [`L216`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_scala_language_wiring.py#L216) — ``given = 1`` parses with an empty ``type_identifier`` child, so the
- `test_ast_cache_symbol_name_named_given_via_type()` — [`L208`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_scala_language_wiring.py#L208)
- `test_ast_cache_symbol_name_uses_identifier_child_for_object()` — [`L198`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_scala_language_wiring.py#L198) — ``object_definition`` exposes no ``name`` field, so the identifier-child
- `test_extension_detects_scala()` — [`L25`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_scala_language_wiring.py#L25)
- `test_lang_extension_map_has_scala()` — [`L31`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_scala_language_wiring.py#L31)
- `test_loader_provides_scala_language()` — [`L49`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_scala_language_wiring.py#L49)
- `test_sc_extension_stays_unknown()` — [`L37`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_scala_language_wiring.py#L37) — ``.sc`` is deliberately NOT wired (ambiguous with SuperCollider) even
- `test_scala_corpus_extracts_symbols()` — [`L58`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_scala_language_wiring.py#L58) — The golden scala corpus must yield real symbols, not phantom-empty.

## Module values
- `CORPUS` — [`L22`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_scala_language_wiring.py#L22)

