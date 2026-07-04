---
title: 'Module: tests/unit/core/test_query_service_helpers.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_query_service_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_query_service_helpers`/
symbols:
  TestPluginQueryNode.test_init_with_full_element: TestPluginQueryNode#test_init_with_full_element().
  TestPluginQueryNode.test_init_with_missing_attributes: TestPluginQueryNode#test_init_with_missing_attributes().
  TestPluginStrategyCaptures.test_multiple_valid_elements: TestPluginStrategyCaptures#test_multiple_valid_elements().
  TestElementToCapture.test_returns_capture_tuple: TestElementToCapture#test_returns_capture_tuple().
  FakeElement: FakeElement#
  TestPluginQueryNode.test_text_encoding: TestPluginQueryNode#test_text_encoding().
  TestElementToCapture.test_uses_query_key_as_fallback: TestElementToCapture#test_uses_query_key_as_fallback().
  TestElementToCapture.test_with_custom_query_key: TestElementToCapture#test_with_custom_query_key().
  TestPluginStrategyCaptures.test_returns_captures_from_plugin: TestPluginStrategyCaptures#test_returns_captures_from_plugin().
  TestPluginStrategyCaptures.test_skips_elements_without_line_attrs: TestPluginStrategyCaptures#test_skips_elements_without_line_attrs().
  TestPluginQueryNode.test_init_with_none_query_key: TestPluginQueryNode#test_init_with_none_query_key().
  TestPluginQueryNode.test_init_element_type_attribute: TestPluginQueryNode#test_init_element_type_attribute().
  TestElementToCapture.test_returns_none_without_start_line: TestElementToCapture#test_returns_none_without_start_line().
  TestElementToCapture.test_returns_none_without_end_line: TestElementToCapture#test_returns_none_without_end_line().
  TestElementToCapture.test_returns_none_with_no_line_attrs: TestElementToCapture#test_returns_none_with_no_line_attrs().
  TestPluginStrategyCaptures.test_returns_none_on_exception: TestPluginStrategyCaptures#test_returns_none_on_exception().
  TestPluginStrategyCaptures.test_returns_empty_for_none_elements: TestPluginStrategyCaptures#test_returns_empty_for_none_elements().
  TestPluginStrategyCaptures.test_uses_function_as_default_query_key: TestPluginStrategyCaptures#test_uses_function_as_default_query_key().
  TestWalkForPluginCategories.test_appends_matching_node: TestWalkForPluginCategories#test_appends_matching_node().
  TestWalkForPluginCategories.test_ignores_non_matching_node: TestWalkForPluginCategories#test_ignores_non_matching_node().
  TestWalkForPluginCategories.test_walks_children: TestWalkForPluginCategories#test_walks_children().
  TestWalkForPluginCategories.test_empty_node_types_list: TestWalkForPluginCategories#test_empty_node_types_list().
  TestWalkForPluginCategories.test_deeply_nested: TestWalkForPluginCategories#test_deeply_nested().
  TestPluginCategoryCaptures.test_returns_captures: TestPluginCategoryCaptures#test_returns_captures().
  TestPluginCategoryCaptures.test_returns_none_on_exception: TestPluginCategoryCaptures#test_returns_none_on_exception().
  TestPluginCategoryCaptures.test_returns_none_for_empty_categories: TestPluginCategoryCaptures#test_returns_none_for_empty_categories().
  TestPluginCategoryCaptures.test_returns_none_for_missing_key: TestPluginCategoryCaptures#test_returns_none_for_missing_key().
  TestPluginCategoryCaptures.test_returns_none_for_none_query_key: TestPluginCategoryCaptures#test_returns_none_for_none_query_key().
  TestPluginCategoryCaptures.test_no_matching_nodes: TestPluginCategoryCaptures#test_no_matching_nodes().
  TestNodeMatchesQuery.test_matching: TestNodeMatchesQuery#test_matching().
  TestFallbackQueryCaptures.test_captures_matching_nodes: TestFallbackQueryCaptures#test_captures_matching_nodes().
  TestFallbackQueryCaptures.test_empty_tree: TestFallbackQueryCaptures#test_empty_tree().
  TestFallbackQueryCaptures.test_nested_matches: TestFallbackQueryCaptures#test_nested_matches().
  TestFallbackQueryCaptures.test_multiple_matches: TestFallbackQueryCaptures#test_multiple_matches().
  TestFallbackQueryCaptures.test_none_query_key: TestFallbackQueryCaptures#test_none_query_key().
  TestFallbackQueryCaptures.test_non_string_node_type: TestFallbackQueryCaptures#test_non_string_node_type().
  TestFallbackQueryCaptures.test_deeply_nested_match: TestFallbackQueryCaptures#test_deeply_nested_match().
  TestFallbackQueryCaptures.test_mixed_matches_different_types: TestFallbackQueryCaptures#test_mixed_matches_different_types().
  TestFallbackQueryCaptures.test_import_match: TestFallbackQueryCaptures#test_import_match().
  TestFallbackQueryCaptures.test_element_key_for_none_query: TestFallbackQueryCaptures#test_element_key_for_none_query().
  FakeElement.start_line: FakeElement#start_line.
  FakeElement.end_line: FakeElement#end_line.
  FakeElement.element_type: FakeElement#element_type.
  FakeElement.raw_text: FakeElement#raw_text.
  TestPluginQueryNode: TestPluginQueryNode#
  TestElementToCapture: TestElementToCapture#
  TestPluginStrategyCaptures: TestPluginStrategyCaptures#
  TestWalkForPluginCategories: TestWalkForPluginCategories#
  TestPluginCategoryCaptures: TestPluginCategoryCaptures#
  TestNodeMatchesQuery: TestNodeMatchesQuery#
  TestFallbackQueryCaptures: TestFallbackQueryCaptures#
---
# Module: [`tests/unit/core/test_query_service_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_helpers.py)

## Classes
### `FakeElement`
- def: [`tests/unit/core/test_query_service_helpers.py:21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_helpers.py#L21)
- signature: `class FakeElement:`
- members:
  - `element_type` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_helpers.py#L22)
  - `end_line` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_helpers.py#L24)
  - `raw_text` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_helpers.py#L25)
  - `start_line` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_helpers.py#L23)
- used by: (7 test-only callers)

### `TestElementToCapture`
- def: [`tests/unit/core/test_query_service_helpers.py:61`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_helpers.py#L61)
- signature: `class TestElementToCapture:`
- members:
  - `test_returns_capture_tuple(self)` — [`L62`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_helpers.py#L62)
  - `test_returns_none_with_no_line_attrs(self)` — [`L78`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_helpers.py#L78)
  - `test_returns_none_without_end_line(self)` — [`L74`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_helpers.py#L74)
  - `test_returns_none_without_start_line(self)` — [`L70`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_helpers.py#L70)
  - `test_uses_query_key_as_fallback(self)` — [`L82`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_helpers.py#L82)
  - `test_with_custom_query_key(self)` — [`L89`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_helpers.py#L89)
- uses (calls/refs, reference-scoped): [`_element_to_capture`](../../../tree_sitter_analyzer/core/_query_service_helpers.md#_element_to_capture), [`PluginQueryNode`](../../../tree_sitter_analyzer/core/_query_service_helpers.md#PluginQueryNode)  (1 test-only)

### `TestFallbackQueryCaptures`
- def: [`tests/unit/core/test_query_service_helpers.py:266`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_helpers.py#L266)
- signature: `class TestFallbackQueryCaptures:`
- members:
  - `test_captures_matching_nodes(self)` — [`L267`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_helpers.py#L267)
  - `test_deeply_nested_match(self)` — [`L308`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_helpers.py#L308)
  - `test_element_key_for_none_query(self)` — [`L331`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_helpers.py#L331)
  - `test_empty_tree(self)` — [`L274`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_helpers.py#L274)
  - `test_import_match(self)` — [`L325`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_helpers.py#L325)
  - `test_mixed_matches_different_types(self)` — [`L316`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_helpers.py#L316)
  - `test_multiple_matches(self)` — [`L287`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_helpers.py#L287)
  - `test_nested_matches(self)` — [`L279`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_helpers.py#L279)
  - `test_non_string_node_type(self)` — [`L302`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_helpers.py#L302)
  - `test_none_query_key(self)` — [`L296`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_helpers.py#L296)
- uses (calls/refs, reference-scoped): [`fallback_query_captures`](../../../tree_sitter_analyzer/core/_query_service_helpers.md#fallback_query_captures)

### `TestNodeMatchesQuery`
- def: [`tests/unit/core/test_query_service_helpers.py:238`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_helpers.py#L238)
- signature: `class TestNodeMatchesQuery:`
- members:
  - `test_matching(self, node_type, query_key, expected)` — [`L262`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_helpers.py#L262)
- uses (calls/refs, reference-scoped): [`_node_matches_query`](../../../tree_sitter_analyzer/core/_query_service_helpers.md#_node_matches_query)

### `TestPluginCategoryCaptures`
- def: [`tests/unit/core/test_query_service_helpers.py:187`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_helpers.py#L187)
- signature: `class TestPluginCategoryCaptures:`
- members:
  - `test_no_matching_nodes(self)` — [`L225`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_helpers.py#L225)
  - `test_returns_captures(self)` — [`L188`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_helpers.py#L188)
  - `test_returns_none_for_empty_categories(self)` — [`L207`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_helpers.py#L207)
  - `test_returns_none_for_missing_key(self)` — [`L213`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_helpers.py#L213)
  - `test_returns_none_for_none_query_key(self)` — [`L219`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_helpers.py#L219)
  - `test_returns_none_on_exception(self)` — [`L201`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_helpers.py#L201)
- uses (calls/refs, reference-scoped): [`plugin_category_captures`](../../../tree_sitter_analyzer/core/_query_service_helpers.md#plugin_category_captures)

### `TestPluginQueryNode`
- def: [`tests/unit/core/test_query_service_helpers.py:28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_helpers.py#L28)
- signature: `class TestPluginQueryNode:`
- members:
  - `test_init_element_type_attribute(self)` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_helpers.py#L50)
  - `test_init_with_full_element(self)` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_helpers.py#L29)
  - `test_init_with_missing_attributes(self)` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_helpers.py#L37)
  - `test_init_with_none_query_key(self)` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_helpers.py#L45)
  - `test_text_encoding(self)` — [`L55`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_helpers.py#L55)
- uses (calls/refs, reference-scoped): [`PluginQueryNode`](../../../tree_sitter_analyzer/core/_query_service_helpers.md#PluginQueryNode), [`text`](../../../tree_sitter_analyzer/core/_query_service_helpers.md#PluginQueryNode.text), [`end_point`](../../../tree_sitter_analyzer/core/_query_service_helpers.md#PluginQueryNode.end_point), [`start_point`](../../../tree_sitter_analyzer/core/_query_service_helpers.md#PluginQueryNode.start_point)  (1 test-only)

### `TestPluginStrategyCaptures`
- def: [`tests/unit/core/test_query_service_helpers.py:97`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_helpers.py#L97)
- signature: `class TestPluginStrategyCaptures:`
- members:
  - `test_multiple_valid_elements(self)` — [`L132`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_helpers.py#L132)
  - `test_returns_captures_from_plugin(self)` — [`L98`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_helpers.py#L98)
  - `test_returns_empty_for_none_elements(self)` — [`L112`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_helpers.py#L112)
  - `test_returns_none_on_exception(self)` — [`L106`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_helpers.py#L106)
  - `test_skips_elements_without_line_attrs(self)` — [`L118`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_helpers.py#L118)
  - `test_uses_function_as_default_query_key(self)` — [`L126`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_helpers.py#L126)
- uses (calls/refs, reference-scoped): [`plugin_strategy_captures`](../../../tree_sitter_analyzer/core/_query_service_helpers.md#plugin_strategy_captures)  (3 test-only)

### `TestWalkForPluginCategories`
- def: [`tests/unit/core/test_query_service_helpers.py:140`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_helpers.py#L140)
- signature: `class TestWalkForPluginCategories:`
- members:
  - `test_appends_matching_node(self)` — [`L141`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_helpers.py#L141)
  - `test_deeply_nested(self)` — [`L175`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_helpers.py#L175)
  - `test_empty_node_types_list(self)` — [`L169`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_helpers.py#L169)
  - `test_ignores_non_matching_node(self)` — [`L150`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_helpers.py#L150)
  - `test_walks_children(self)` — [`L158`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_helpers.py#L158)
- uses (calls/refs, reference-scoped): [`_walk_for_plugin_categories`](../../../tree_sitter_analyzer/core/_query_service_helpers.md#_walk_for_plugin_categories)

