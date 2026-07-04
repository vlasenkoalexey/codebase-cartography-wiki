---
title: 'Module: tree_sitter_analyzer/languages/yaml_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/yaml_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.yaml_helpers`/
symbols:
  YAMLElement: YAMLElement#
  YAMLElement.key: YAMLElement#key.
  YAMLElement.__init__: YAMLElement#__init__().
  _yaml_failure_result: _yaml_failure_result().
  _extract_mapping_nodes: _extract_mapping_nodes().
  _yaml_success_result: _yaml_success_result().
  YAMLElement.document_index: YAMLElement#document_index.
  extract_value_info: extract_value_info().
  analyze_yaml_file: analyze_yaml_file().
  YAMLElement.value_type: YAMLElement#value_type.
  _assign_flow_or_block_mapping_node: _assign_flow_or_block_mapping_node().
  YAMLElement.value: YAMLElement#value.
  build_sequence_element: build_sequence_element().
  append_mapping_element: append_mapping_element().
  append_document_element: append_document_element().
  append_sequence_element: append_sequence_element().
  append_anchor_element: append_anchor_element().
  append_alias_element: append_alias_element().
  append_comment_element: append_comment_element().
  build_document_element: build_document_element().
  extract_mapping_key_and_value: extract_mapping_key_and_value().
  YAMLElement.child_count: YAMLElement#child_count.
  build_comment_element: build_comment_element().
  extract_sequence_key: extract_sequence_key().
  build_mapping_element: build_mapping_element().
  traverse_nodes: traverse_nodes().
  count_document_children: count_document_children().
  YAMLElement.nesting_level: YAMLElement#nesting_level.
  YAMLElement._Config.from_kwargs: YAMLElement#_Config#from_kwargs().
  _count_top_level_document_child: _count_top_level_document_child().
  iter_nodes_by_type: iter_nodes_by_type().
  _extract_mapping_value_info: _extract_mapping_value_info().
  _extract_yaml_file_elements: _extract_yaml_file_elements().
  YAMLElement.anchor_name: YAMLElement#anchor_name.
  YAMLElement.alias_target: YAMLElement#alias_target.
  build_anchor_element: build_anchor_element().
  build_alias_element: build_alias_element().
  extract_node_text: extract_node_text().
  _find_anchor_name: _find_anchor_name().
  calculate_nesting_level: calculate_nesting_level().
  get_document_index: get_document_index().
  iter_document_nodes: iter_document_nodes().
  iter_mapping_nodes: iter_mapping_nodes().
  iter_sequence_nodes: iter_sequence_nodes().
  _count_block_node_child: _count_block_node_child().
  _extract_scalar_value_info: _extract_scalar_value_info().
  _find_sequence_key_node: _find_sequence_key_node().
  YAMLElement._Config: YAMLElement#_Config#
  _MappingNodeContext.anchor_name: _MappingNodeContext#anchor_name.
  count_sequence_children: count_sequence_children().
  _truncate_raw_text: _truncate_raw_text().
  is_number: is_number().
  YAMLElement.from_legacy_kwargs: YAMLElement#from_legacy_kwargs().
  _MappingNodeContext: _MappingNodeContext#
  _MappingNodeContext.found_colon: _MappingNodeContext#found_colon.
  _MappingNodeContext.key_node: _MappingNodeContext#key_node.
  _MappingNodeContext.value_node: _MappingNodeContext#value_node.
  _MappingNodeContext.get_node_text: _MappingNodeContext#get_node_text.
  _count_mapping_pairs: _count_mapping_pairs().
  _drill_to_scalar: _drill_to_scalar().
  _first_child_or_self: _first_child_or_self().
  _anchor_name: _anchor_name().
  YAMLElement._Config.name: YAMLElement#_Config#name.
  YAMLElement._Config.start_line: YAMLElement#_Config#start_line.
  YAMLElement._Config.end_line: YAMLElement#_Config#end_line.
  YAMLElement._Config.raw_text: YAMLElement#_Config#raw_text.
  YAMLElement._Config.language: YAMLElement#_Config#language.
  YAMLElement._Config.element_type: YAMLElement#_Config#element_type.
  YAMLElement._Config.key: YAMLElement#_Config#key.
  YAMLElement._Config.value: YAMLElement#_Config#value.
  YAMLElement._Config.value_type: YAMLElement#_Config#value_type.
  YAMLElement._Config.anchor_name: YAMLElement#_Config#anchor_name.
  YAMLElement._Config.alias_target: YAMLElement#_Config#alias_target.
  YAMLElement._Config.nesting_level: YAMLElement#_Config#nesting_level.
  YAMLElement._Config.document_index: YAMLElement#_Config#document_index.
  YAMLElement._Config.child_count: YAMLElement#_Config#child_count.
  YAMLElement._Config.docstring: YAMLElement#_Config#docstring.
  _count_value_mapping_children: _count_value_mapping_children().
  _count_value_sequence_children: _count_value_sequence_children().
  _extract_alias_value_info: _extract_alias_value_info().
  _find_inner_node: _find_inner_node().
  _find_parent_mapping_pair: _find_parent_mapping_pair().
  _is_sequence_key_child: _is_sequence_key_child().
  _parse_yaml_content: _parse_yaml_content().
---
# Module: [`tree_sitter_analyzer/languages/yaml_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py)

## Classes
### `YAMLElement`  ·  implements/extends CodeElement
- def: [`tree_sitter_analyzer/languages/yaml_helpers.py:12`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L12)
- doc: YAML-specific code element.
- signature: `class YAMLElement(CodeElement):`
- members:
  - `__init__(self, *args: Any, **kwargs: Any)` — [`L55`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L55) — Initialize a YAML element with YAML-specific metadata.
  - `from_legacy_kwargs(cls, **kwargs: Any)` — [`L101`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L101) — Build a YAMLElement from the historical named-argument constructor.
  - `alias_target` — [`L95`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L95)
  - `anchor_name` — [`L94`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L94)
  - `child_count` — [`L98`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L98)
  - `document_index` — [`L97`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L97)
  - `key` — [`L91`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L91)
  - `nesting_level` — [`L96`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L96)
  - `value` — [`L92`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L92)
  - `value_type` — [`L93`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L93)
- uses (calls/refs, reference-scoped): [`CodeElement`](../models/base.md#CodeElement), [`element_type`](../models/base.md#CodeElement.element_type), [`from_kwargs`](yaml_helpers.md#YAMLElement._Config.from_kwargs), [`_Config`](yaml_helpers.md#YAMLElement._Config), [`alias_target`](yaml_helpers.md#YAMLElement._Config.alias_target), [`anchor_name`](yaml_helpers.md#YAMLElement._Config.anchor_name), [`child_count`](yaml_helpers.md#YAMLElement._Config.child_count), [`docstring`](yaml_helpers.md#YAMLElement._Config.docstring), [`document_index`](yaml_helpers.md#YAMLElement._Config.document_index), [`element_type`](yaml_helpers.md#YAMLElement._Config.element_type), [`end_line`](yaml_helpers.md#YAMLElement._Config.end_line), [`key`](yaml_helpers.md#YAMLElement._Config.key), [`language`](yaml_helpers.md#YAMLElement._Config.language), [`name`](yaml_helpers.md#YAMLElement._Config.name), [`nesting_level`](yaml_helpers.md#YAMLElement._Config.nesting_level), [`raw_text`](yaml_helpers.md#YAMLElement._Config.raw_text), [`start_line`](yaml_helpers.md#YAMLElement._Config.start_line), [`value`](yaml_helpers.md#YAMLElement._Config.value), [`value_type`](yaml_helpers.md#YAMLElement._Config.value_type)
- used by: [`CodeElement`](../models/base.md#CodeElement), [`extract_yaml_elements`](yaml_plugin.md#YAMLElementExtractor.extract_yaml_elements), [`_extract_aliases`](yaml_plugin.md#YAMLElementExtractor._extract_aliases), [`_extract_anchors`](yaml_plugin.md#YAMLElementExtractor._extract_anchors), [`_extract_mappings`](yaml_plugin.md#YAMLElementExtractor._extract_mappings), [`_extract_sequences`](yaml_plugin.md#YAMLElementExtractor._extract_sequences), [`_extract_comments`](yaml_plugin.md#YAMLElementExtractor._extract_comments), [`_extract_documents`](yaml_plugin.md#YAMLElementExtractor._extract_documents), [`build_sequence_element`](yaml_helpers.md#build_sequence_element), [`append_mapping_element`](yaml_helpers.md#append_mapping_element), [`append_alias_element`](yaml_helpers.md#append_alias_element), [`append_anchor_element`](yaml_helpers.md#append_anchor_element), [`append_comment_element`](yaml_helpers.md#append_comment_element), [`append_document_element`](yaml_helpers.md#append_document_element), [`append_sequence_element`](yaml_helpers.md#append_sequence_element), [`build_document_element`](yaml_helpers.md#build_document_element), [`build_comment_element`](yaml_helpers.md#build_comment_element), [`build_mapping_element`](yaml_helpers.md#build_mapping_element), [`from_kwargs`](yaml_helpers.md#YAMLElement._Config.from_kwargs), [`build_alias_element`](yaml_helpers.md#build_alias_element), [`build_anchor_element`](yaml_helpers.md#build_anchor_element)  (34 test-only)

### `_Config`
- def: [`tree_sitter_analyzer/languages/yaml_helpers.py:16`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L16)
- doc: Configuration carrier for YAMLElement construction.
- signature: `class _Config:`
- members:
  - `from_kwargs(cls, **kwargs: Any)` — [`L36`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L36)
  - `alias_target` — [`L29`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L29)
  - `anchor_name` — [`L28`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L28)
  - `child_count` — [`L32`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L32)
  - `docstring` — [`L33`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L33)
  - `document_index` — [`L31`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L31)
  - `element_type` — [`L24`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L24)
  - `end_line` — [`L21`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L21)
  - `key` — [`L25`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L25)
  - `language` — [`L23`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L23)
  - `name` — [`L19`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L19)
  - `nesting_level` — [`L30`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L30)
  - `raw_text` — [`L22`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L22)
  - `start_line` — [`L20`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L20)
  - `value` — [`L26`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L26)
  - `value_type` — [`L27`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L27)
- uses (calls/refs, reference-scoped): [`YAMLElement`](yaml_helpers.md#YAMLElement)
- used by: [`key`](yaml_helpers.md#YAMLElement.key), [`__init__`](yaml_helpers.md#YAMLElement.__init__), [`document_index`](yaml_helpers.md#YAMLElement.document_index), [`value_type`](yaml_helpers.md#YAMLElement.value_type), [`value`](yaml_helpers.md#YAMLElement.value), [`child_count`](yaml_helpers.md#YAMLElement.child_count), [`nesting_level`](yaml_helpers.md#YAMLElement.nesting_level), [`alias_target`](yaml_helpers.md#YAMLElement.alias_target), [`anchor_name`](yaml_helpers.md#YAMLElement.anchor_name)

### `_MappingNodeContext`
- def: [`tree_sitter_analyzer/languages/yaml_helpers.py:107`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L107)
- doc: State carried when assigning flow or block mapping nodes.
- signature: `class _MappingNodeContext:`
- members:
  - `anchor_name` — [`L113`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L113)
  - `found_colon` — [`L110`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L110)
  - `get_node_text` — [`L114`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L114)
  - `key_node` — [`L111`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L111)
  - `value_node` — [`L112`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L112)
- used by: [`_extract_mapping_nodes`](yaml_helpers.md#_extract_mapping_nodes), [`_assign_flow_or_block_mapping_node`](yaml_helpers.md#_assign_flow_or_block_mapping_node)

## Functions
- `_anchor_name(node: Any, get_node_text: Callable[..., str])` — [`L662`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L662)
- `_assign_flow_or_block_mapping_node(child: Any, state: _MappingNodeContext)` — [`L626`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L626)
- `_count_block_node_child(node: Any)` — [`L192`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L192)
- `_count_mapping_pairs(node: Any)` — [`L200`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L200)
- `_count_top_level_document_child(node: Any)` — [`L184`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L184)
- `_count_value_mapping_children(node: Any)` — [`L533`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L533)
- `_count_value_sequence_children(node: Any)` — [`L541`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L541)
- `_drill_to_scalar(node: Any, get_node_text: Callable[..., str])` — [`L553`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L553) — Drill down through flow_node/block_node wrappers to get scalar text.
- `_extract_alias_value_info(text: str)` — [`L548`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L548)
- `_extract_mapping_nodes(children: list[Any], get_node_text: Callable[..., str])` — [`L585`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L585)
- `_extract_mapping_value_info(value_node: Any | None, get_node_text: Callable[..., str])` — [`L638`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L638)
- `_extract_scalar_value_info(text: str)` — [`L522`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L522)
- `_extract_yaml_file_elements(*, file_path: str, create_extractor: Callable[[], Any], parser: Any, parser_lock: Any)` — [`L750`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L750)
- `_find_anchor_name(children: list[Any], get_node_text: Callable[..., str])` — [`L653`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L653)
- `_find_inner_node(node: Any)` — [`L668`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L668) — Find the inner content node by drilling through wrappers.
- `_find_parent_mapping_pair(node: Any)` — [`L692`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L692)
- `_find_sequence_key_node(parent: Any)` — [`L701`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L701)
- `_first_child_or_self(node: Any)` — [`L647`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L647)
- `_is_sequence_key_child(child: Any, parent: Any, found_colon: bool)` — [`L711`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L711)
- `_parse_yaml_content(content: str, parser: Any, parser_lock: Any)` — [`L763`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L763) — Parse YAML content while respecting the shared parser lock.
- `_truncate_raw_text(raw_text: str, limit: int = 200)` — [`L478`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L478)
- `_yaml_failure_result(file_path: str, error_message: str)` — [`L789`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L789) — Build a consistent YAML analysis failure result.
- `_yaml_success_result(file_path: str, content: str, elements: list[Any])` — [`L771`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L771)
- `analyze_yaml_file(*, file_path: str, create_extractor: Callable[[], Any], yaml_available: bool, parser: Any, parser_lock: Any)` — [`L719`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L719) — Analyze a YAML file using the shared parser and extractor factory.
- `append_alias_element(elements: list[YAMLElement], node: Any, get_node_text: Callable[[Any], str], get_document_index_func: Callable[[Any], int], calculate_nesting_level_func: Callable[[Any], int])` — [`L400`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L400) — Append a YAML alias element, preserving extractor fault tolerance.
- `append_anchor_element(elements: list[YAMLElement], node: Any, get_node_text: Callable[[Any], str], get_document_index_func: Callable[[Any], int], calculate_nesting_level_func: Callable[[Any], int])` — [`L358`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L358) — Append a YAML anchor element, preserving extractor fault tolerance.
- `append_comment_element(elements: list[YAMLElement], node: Any, get_node_text: Callable[[Any], str], get_document_index_func: Callable[[Any], int])` — [`L442`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L442) — Append a YAML comment element, preserving extractor fault tolerance.
- `append_document_element(elements: list[YAMLElement], node: Any, get_node_text: Callable[[Any], str], get_document_index_func: Callable[[Any], int])` — [`L238`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L238) — Append a YAML document element, preserving extractor fault tolerance.
- `append_mapping_element(elements: list[YAMLElement], node: Any, get_node_text: Callable[[Any], str], get_document_index_func: Callable[[Any], int], calculate_nesting_level_func: Callable[[Any], int])` — [`L258`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L258) — Append a YAML mapping element, preserving extractor fault tolerance.
- `append_sequence_element(elements: list[YAMLElement], node: Any, get_node_text: Callable[[Any], str], get_document_index_func: Callable[[Any], int], calculate_nesting_level_func: Callable[[Any], int])` — [`L311`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L311) — Append a YAML sequence element, preserving extractor fault tolerance.
- `build_alias_element(node: Any, get_node_text: Callable[[Any], str], get_document_index_func: Callable[[Any], int], calculate_nesting_level_func: Callable[[Any], int])` — [`L421`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L421) — Build a YAML alias element from a tree-sitter alias node.
- `build_anchor_element(node: Any, get_node_text: Callable[[Any], str], get_document_index_func: Callable[[Any], int], calculate_nesting_level_func: Callable[[Any], int])` — [`L379`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L379) — Build a YAML anchor element from a tree-sitter anchor node.
- `build_comment_element(node: Any, get_node_text: Callable[[Any], str], get_document_index_func: Callable[[Any], int])` — [`L457`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L457) — Build a YAML comment element from a tree-sitter comment node.
- `build_document_element(node: Any, get_node_text: Callable[[Any], str], get_document_index_func: Callable[[Any], int])` — [`L213`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L213) — Build a YAML document element from a tree-sitter document node.
- `build_mapping_element(node: Any, get_node_text: Callable[[Any], str], get_document_index_func: Callable[[Any], int], calculate_nesting_level_func: Callable[[Any], int])` — [`L279`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L279) — Build a YAML mapping element from a tree-sitter mapping pair node.
- `build_sequence_element(node: Any, get_node_text: Callable[[Any], str], get_document_index_func: Callable[[Any], int], calculate_nesting_level_func: Callable[[Any], int])` — [`L332`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L332) — Build a YAML sequence element from a tree-sitter sequence node.
- `calculate_nesting_level(node: Any)` — [`L130`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L130) — Calculate AST-based logical nesting level.
- `count_document_children(document_node: Any)` — [`L174`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L174) — Count meaningful top-level YAML document children.
- `count_sequence_children(sequence_node: Any)` — [`L204`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L204) — Count meaningful YAML sequence children.
- `extract_mapping_key_and_value(node: Any, get_node_text: Callable[..., str])` — [`L563`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L563) — Extract key, value, value_type, child_count, and anchor from a mapping pair node.
- `extract_node_text(node: Any, source_code: str)` — [`L117`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L117) — Extract text content from a tree-sitter node.
- `extract_sequence_key(node: Any, get_node_text: Callable[..., str])` — [`L677`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L677) — Try to find the key for a sequence by checking parent mapping.
- `extract_value_info(node: Any, get_node_text: Callable[..., str])` — [`L493`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L493) — Extract value information from a node.
- `get_document_index(node: Any)` — [`L148`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L148) — Get document index for a node.
- `is_number(text: str)` — [`L484`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L484) — Check if text represents a number.
- `iter_document_nodes(nodes: list[Any])` — [`L233`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L233) — Return YAML document nodes from a traversed node list.
- `iter_mapping_nodes(nodes: list[Any])` — [`L253`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L253) — Return YAML mapping pair nodes from a traversed node list.
- `iter_nodes_by_type(nodes: list[Any], node_type: str)` — [`L353`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L353) — Return nodes with the requested tree-sitter type.
- `iter_sequence_nodes(nodes: list[Any])` — [`L306`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L306) — Return YAML sequence nodes from a traversed node list.
- `traverse_nodes(node: Any)` — [`L166`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_helpers.py#L166) — Traverse all nodes in the tree.

