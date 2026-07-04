---
title: 'Module: tests/property/test_phase8_property_boost.py'
type: catalog
provenance: extracted
module: tests/property/test_phase8_property_boost.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.property.test_phase8_property_boost`/Test
symbols:
  TestQueryLoaderProperties.test_load_twice_same_result: QueryLoaderProperties#test_load_twice_same_result().
  TestQueryLoaderProperties.test_unknown_language_returns_empty: QueryLoaderProperties#test_unknown_language_returns_empty().
  TestQueryLoaderProperties.test_common_queries_present: QueryLoaderProperties#test_common_queries_present().
  TestEncodingProperties.test_utf8_roundtrip_preserves_content: EncodingProperties#test_utf8_roundtrip_preserves_content().
  TestEncodingProperties.test_safe_decode_preserves_length: EncodingProperties#test_safe_decode_preserves_length().
  TestEncodingProperties.test_detect_encoding_always_returns_string: EncodingProperties#test_detect_encoding_always_returns_string().
  TestQueryLoaderProperties: QueryLoaderProperties#
  TestEncodingProperties: EncodingProperties#
---
# Module: [`tests/property/test_phase8_property_boost.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_phase8_property_boost.py)

## Classes
### `TestEncodingProperties`
- def: [`tests/property/test_phase8_property_boost.py:57`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_phase8_property_boost.py#L57)
- doc: Property: safe_encode → safe_decode roundtrip preserves content.
- signature: `class TestEncodingProperties:`
- members:
  - `test_detect_encoding_always_returns_string(self, text)` — [`L94`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_phase8_property_boost.py#L94)
  - `test_safe_decode_preserves_length(self, text)` — [`L85`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_phase8_property_boost.py#L85)
  - `test_utf8_roundtrip_preserves_content(self, text)` — [`L68`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_phase8_property_boost.py#L68)
- uses (calls/refs, reference-scoped): [`EncodingManager`](../../tree_sitter_analyzer/encoding_utils.md#EncodingManager), [`safe_decode`](../../tree_sitter_analyzer/encoding_utils.md#EncodingManager.safe_decode), [`detect_encoding`](../../tree_sitter_analyzer/encoding_utils.md#EncodingManager.detect_encoding), [`safe_encode`](../../tree_sitter_analyzer/encoding_utils.md#EncodingManager.safe_encode)

### `TestQueryLoaderProperties`
- def: [`tests/property/test_phase8_property_boost.py:11`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_phase8_property_boost.py#L11)
- doc: Property: load_language_queries is deterministic and idempotent.
- signature: `class TestQueryLoaderProperties:`
- members:
  - `test_common_queries_present(self, query_name)` — [`L51`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_phase8_property_boost.py#L51)
  - `test_load_twice_same_result(self, language)` — [`L20`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_phase8_property_boost.py#L20)
  - `test_unknown_language_returns_empty(self, fake_lang)` — [`L34`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_phase8_property_boost.py#L34)
- uses (calls/refs, reference-scoped): [`load_language_queries`](../../tree_sitter_analyzer/query_loader.md#QueryLoader.load_language_queries), [`QueryLoader`](../../tree_sitter_analyzer/query_loader.md#QueryLoader), [`get_common_queries`](../../tree_sitter_analyzer/query_loader.md#QueryLoader.get_common_queries)

