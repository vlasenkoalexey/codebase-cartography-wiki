---
title: 'Module: tests/unit/test_bash_language_wiring.py'
type: catalog
provenance: extracted
module: tests/unit/test_bash_language_wiring.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_bash_language_wiring`/
symbols:
  test_subscript_fallback_child_when_name_field_absent: test_subscript_fallback_child_when_name_field_absent().
  test_subscript_read_not_relabeled_to_base_variable: test_subscript_read_not_relabeled_to_base_variable().
  test_subscript_assignment_target_unwrapped_to_base_variable: test_subscript_assignment_target_unwrapped_to_base_variable().
  test_subscript_fallback_word_child_when_name_field_absent: test_subscript_fallback_word_child_when_name_field_absent().
  test_subscript_assignment_target_no_base_keeps_subscript_label: test_subscript_assignment_target_no_base_keeps_subscript_label().
  test_ast_cache_indexes_sh_file: test_ast_cache_indexes_sh_file().
  _FakeBashNode: _FakeBashNode#
  test_bash_corpus_extracts_functions: test_bash_corpus_extracts_functions().
  test_loader_provides_bash_language: test_loader_provides_bash_language().
  _make_subscript_extractor: _make_subscript_extractor().
  _FakeBashNode._name_field: _FakeBashNode#_name_field.
  _FakeBashNode.parent: _FakeBashNode#parent.
  test_extension_detects_bash: test_extension_detects_bash().
  test_lang_extension_map_has_bash: test_lang_extension_map_has_bash().
  _FakeBashNode.child_by_field_name: _FakeBashNode#child_by_field_name().
  CORPUS: CORPUS.
  _FakeBashNode.__init__: _FakeBashNode#__init__().
  _FakeBashNode.text: _FakeBashNode#text.
  _FakeBashNode.children: _FakeBashNode#children.
  _FakeBashNode.start_point: _FakeBashNode#start_point.
  _FakeBashNode.end_point: _FakeBashNode#end_point.
  _FakeBashNode.start_byte: _FakeBashNode#start_byte.
  _FakeBashNode.end_byte: _FakeBashNode#end_byte.
  _FakeBashNode.id: _FakeBashNode#id.
---
# Module: [`tests/unit/test_bash_language_wiring.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_bash_language_wiring.py)

## Classes
### `_FakeBashNode`
- def: [`tests/unit/test_bash_language_wiring.py:114`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_bash_language_wiring.py#L114)
- doc: Minimal tree-sitter node stand-in for `_extract_subscript` fallback.
- signature: `class _FakeBashNode:`
- members:
  - `child_by_field_name(self, field: str)` — [`L137`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_bash_language_wiring.py#L137)
  - `children` — [`L126`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_bash_language_wiring.py#L126)
  - `end_byte` — [`L130`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_bash_language_wiring.py#L130)
  - `end_point` — [`L128`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_bash_language_wiring.py#L128)
  - `id` — [`L135`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_bash_language_wiring.py#L135)
  - `parent` — [`L131`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_bash_language_wiring.py#L131)
  - `start_byte` — [`L129`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_bash_language_wiring.py#L129)
  - `start_point` — [`L127`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_bash_language_wiring.py#L127)
  - `text` — [`L125`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_bash_language_wiring.py#L125)
- protocol/private: `__init__`[`L123`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_bash_language_wiring.py#L123), `_name_field`[`L132`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_bash_language_wiring.py#L132)
- used by: (3 test-only callers)

## Functions
- `_make_subscript_extractor(monkeypatch)` — [`L141`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_bash_language_wiring.py#L141)
- `test_ast_cache_indexes_sh_file()` — [`L211`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_bash_language_wiring.py#L211) — The project indexer must index .sh files without errors.
- `test_bash_corpus_extracts_functions()` — [`L49`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_bash_language_wiring.py#L49) — The golden bash corpus must yield its function definitions.
- `test_extension_detects_bash(ext: str)` — [`L26`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_bash_language_wiring.py#L26)
- `test_lang_extension_map_has_bash()` — [`L32`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_bash_language_wiring.py#L32)
- `test_loader_provides_bash_language()` — [`L40`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_bash_language_wiring.py#L40)
- `test_subscript_assignment_target_no_base_keeps_subscript_label(monkeypatch)` — [`L192`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_bash_language_wiring.py#L192) — #949 — assignment target with neither a ``name`` field nor a
- `test_subscript_assignment_target_unwrapped_to_base_variable()` — [`L93`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_bash_language_wiring.py#L93) — #949 — an assignment target (``arr[0]=x``) DOES unwrap to the base
- `test_subscript_fallback_child_when_name_field_absent(monkeypatch)` — [`L155`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_bash_language_wiring.py#L155) — #949 — assignment target whose subscript lacks a ``name`` field falls
- `test_subscript_fallback_word_child_when_name_field_absent(monkeypatch)` — [`L175`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_bash_language_wiring.py#L175) — #949 — fallback also accepts a ``word`` child as the base name.
- `test_subscript_read_not_relabeled_to_base_variable()` — [`L70`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_bash_language_wiring.py#L70) — #949 Codex P2 — a subscript *read* (``echo ${arr[0]}``) must keep its

## Module values
- `CORPUS` — [`L22`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_bash_language_wiring.py#L22)

