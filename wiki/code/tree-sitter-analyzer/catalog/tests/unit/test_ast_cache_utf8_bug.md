---
title: 'Module: tests/unit/test_ast_cache_utf8_bug.py'
type: catalog
provenance: extracted
module: tests/unit/test_ast_cache_utf8_bug.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_ast_cache_utf8_bug`/
symbols:
  test_indexed_class_name_is_not_byte_shifted: test_indexed_class_name_is_not_byte_shifted().
  test_node_text_helper_handles_bytes_attr.FakeNode.end_byte: test_node_text_helper_handles_bytes_attr().FakeNode#end_byte.
  test_node_text_helper_falls_back_to_bytes_slice.FakeNode.end_byte: test_node_text_helper_falls_back_to_bytes_slice().FakeNode#end_byte.
  test_node_text_helper_handles_multibyte_source: test_node_text_helper_handles_multibyte_source().
  test_node_text_helper_handles_bytes_attr.FakeNode: test_node_text_helper_handles_bytes_attr().FakeNode#
  test_node_text_helper_falls_back_to_bytes_slice.FakeNode: test_node_text_helper_falls_back_to_bytes_slice().FakeNode#
  test_node_text_helper_handles_multibyte_source.FakeNode: test_node_text_helper_handles_multibyte_source().FakeNode#
  utf8_project: utf8_project().
  test_node_text_helper_handles_bytes_attr: test_node_text_helper_handles_bytes_attr().
  test_node_text_helper_handles_bytes_attr.FakeNode.text: test_node_text_helper_handles_bytes_attr().FakeNode#text.
  test_node_text_helper_handles_bytes_attr.FakeNode.start_byte: test_node_text_helper_handles_bytes_attr().FakeNode#start_byte.
  test_node_text_helper_falls_back_to_bytes_slice: test_node_text_helper_falls_back_to_bytes_slice().
  test_node_text_helper_falls_back_to_bytes_slice.FakeNode.text: test_node_text_helper_falls_back_to_bytes_slice().FakeNode#text.
  test_node_text_helper_falls_back_to_bytes_slice.FakeNode.start_byte: test_node_text_helper_falls_back_to_bytes_slice().FakeNode#start_byte.
  test_node_text_helper_handles_multibyte_source.FakeNode.text: test_node_text_helper_handles_multibyte_source().FakeNode#text.
  test_node_text_helper_handles_multibyte_source.FakeNode.start_byte: test_node_text_helper_handles_multibyte_source().FakeNode#start_byte.
  test_node_text_helper_handles_multibyte_source.FakeNode.end_byte: test_node_text_helper_handles_multibyte_source().FakeNode#end_byte.
---
# Module: [`tests/unit/test_ast_cache_utf8_bug.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_utf8_bug.py)

## Classes
### `FakeNode`
- def: [`tests/unit/test_ast_cache_utf8_bug.py:114`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_utf8_bug.py#L114)
- signature: `class FakeNode:`
- members:
  - `end_byte` — [`L88`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_utf8_bug.py#L88)
  - `end_byte` — [`L100`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_utf8_bug.py#L100)
  - `end_byte` — [`L117`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_utf8_bug.py#L117)
  - `start_byte` — [`L87`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_utf8_bug.py#L87)
  - `start_byte` — [`L99`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_utf8_bug.py#L99)
  - `start_byte` — [`L116`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_utf8_bug.py#L116)
  - `text` — [`L86`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_utf8_bug.py#L86)
  - `text` — [`L98`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_utf8_bug.py#L98)
  - `text` — [`L115`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_utf8_bug.py#L115)
- uses (calls/refs, reference-scoped): [`_node_text`](../../tree_sitter_analyzer/_ast_extraction.md#_node_text)  (2 test-only)
- used by: (1 test-only callers)

## Functions
- `test_indexed_class_name_is_not_byte_shifted(utf8_project: Path)` — [`L56`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_utf8_bug.py#L56)
- `test_node_text_helper_falls_back_to_bytes_slice()` — [`L93`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_utf8_bug.py#L93) — When ``node.text`` is unavailable, the helper must slice on bytes
- `test_node_text_helper_handles_bytes_attr()` — [`L81`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_utf8_bug.py#L81) — ``_node_text`` should prefer ``node.text`` (bytes) when present.
- `test_node_text_helper_handles_multibyte_source()` — [`L105`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_utf8_bug.py#L105) — The fallback slice must use byte indices on the encoded source.
- `utf8_project()` — [`L35`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_utf8_bug.py#L35) — A project with a multi-byte glyph (``≤``) before a class def.

