---
title: 'Module: tree_sitter_analyzer/plugins/_base_traverse_mixin.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/plugins/_base_traverse_mixin.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.plugins._base_traverse_mixin`/
symbols:
  DefaultTraverseMixin._traverse_for_functions: DefaultTraverseMixin#_traverse_for_functions().
  DefaultTraverseMixin: DefaultTraverseMixin#
  DefaultNodeMixin: DefaultNodeMixin#
  DefaultNodeMixin._is_function_node: DefaultNodeMixin#_is_function_node.
  DefaultNodeMixin._is_class_node: DefaultNodeMixin#_is_class_node.
  DefaultNodeMixin._is_variable_node: DefaultNodeMixin#_is_variable_node.
  DefaultNodeMixin._is_import_node: DefaultNodeMixin#_is_import_node.
  DefaultNodeMixin._element_fields: DefaultNodeMixin#_element_fields().
  DefaultTraverseMixin._traverse_for_classes: DefaultTraverseMixin#_traverse_for_classes().
  DefaultTraverseMixin._traverse_for_imports: DefaultTraverseMixin#_traverse_for_imports().
  DefaultNodeMixin._extract_node_name: DefaultNodeMixin#_extract_node_name().
  DefaultTraverseMixin._traverse_for_variables: DefaultTraverseMixin#_traverse_for_variables().
  _node_type_matches: _node_type_matches().
  DefaultTraverseAppendMixin: DefaultTraverseAppendMixin#
  DefaultNodeMixin._extract_node_text: DefaultNodeMixin#_extract_node_text.
  _is_function_node: _is_function_node().
  _extract_node_text: _extract_node_text().
  DefaultTraverseAppendMixin._append_function: DefaultTraverseAppendMixin#_append_function().
  _is_class_node: _is_class_node().
  _is_variable_node: _is_variable_node().
  _is_import_node: _is_import_node().
  DefaultTraverseAppendMixin._append_class: DefaultTraverseAppendMixin#_append_class().
  DefaultTraverseAppendMixin._append_variable: DefaultTraverseAppendMixin#_append_variable().
  DefaultTraverseAppendMixin._append_import: DefaultTraverseAppendMixin#_append_import().
  CLASS_NODE_TYPES: CLASS_NODE_TYPES.
  _iter_children: _iter_children().
  DefaultNodeMixin._tree_root_node: DefaultNodeMixin#_tree_root_node.
  FUNCTION_NODE_TYPES: FUNCTION_NODE_TYPES.
  VARIABLE_NODE_TYPES: VARIABLE_NODE_TYPES.
  IMPORT_NODE_TYPES: IMPORT_NODE_TYPES.
  _find_identifier_child: _find_identifier_child().
  DefaultNodeMixin._get_language_hint: DefaultNodeMixin#_get_language_hint.
  _node_start_line: _node_start_line().
  _node_end_line: _node_end_line().
  _tree_root_node: _tree_root_node().
  DefaultNodeMixin._find_identifier_child: DefaultNodeMixin#_find_identifier_child.
  DefaultNodeMixin._format_fallback_node_name: DefaultNodeMixin#_format_fallback_node_name.
  _format_fallback_node_name: _format_fallback_node_name().
  _get_language_hint: _get_language_hint().
---
# Module: [`tree_sitter_analyzer/plugins/_base_traverse_mixin.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_base_traverse_mixin.py)

## Classes
### `DefaultNodeMixin`
- def: [`tree_sitter_analyzer/plugins/_base_traverse_mixin.py:124`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_base_traverse_mixin.py#L124)
- doc: Node classification and text helpers used by the default extractor.
- signature: `class DefaultNodeMixin:`
- members:
  - `_extract_node_name(self, node: tree_sitter.Node, source_code: str)` — [`L137`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_base_traverse_mixin.py#L137) — Extract name from a tree-sitter node.
- protocol/private: `_element_fields`[`L149`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_base_traverse_mixin.py#L149), `_extract_node_text`[`L134`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_base_traverse_mixin.py#L134), `_find_identifier_child`[`L132`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_base_traverse_mixin.py#L132), `_format_fallback_node_name`[`L133`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_base_traverse_mixin.py#L133), `_get_language_hint`[`L135`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_base_traverse_mixin.py#L135), `_is_class_node`[`L129`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_base_traverse_mixin.py#L129), `_is_function_node`[`L128`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_base_traverse_mixin.py#L128), `_is_import_node`[`L131`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_base_traverse_mixin.py#L131), `_is_variable_node`[`L130`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_base_traverse_mixin.py#L130), `_tree_root_node`[`L127`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_base_traverse_mixin.py#L127)
- uses (calls/refs, reference-scoped): [`DefaultTraverseAppendMixin`](_base_traverse_mixin.md#DefaultTraverseAppendMixin), [`_is_function_node`](_base_traverse_mixin.md#_is_function_node), [`_extract_node_text`](_base_traverse_mixin.md#_extract_node_text), [`_is_class_node`](_base_traverse_mixin.md#_is_class_node), [`_is_import_node`](_base_traverse_mixin.md#_is_import_node), [`_is_variable_node`](_base_traverse_mixin.md#_is_variable_node), [`_find_identifier_child`](_base_traverse_mixin.md#_find_identifier_child), [`_node_end_line`](_base_traverse_mixin.md#_node_end_line), [`_node_start_line`](_base_traverse_mixin.md#_node_start_line), [`_tree_root_node`](_base_traverse_mixin.md#_tree_root_node), [`_format_fallback_node_name`](_base_traverse_mixin.md#_format_fallback_node_name), [`_get_language_hint`](_base_traverse_mixin.md#_get_language_hint)
- used by: [`_traverse_for_functions`](_base_traverse_mixin.md#DefaultTraverseMixin._traverse_for_functions), [`_traverse_for_classes`](_base_traverse_mixin.md#DefaultTraverseMixin._traverse_for_classes), [`_traverse_for_imports`](_base_traverse_mixin.md#DefaultTraverseMixin._traverse_for_imports), [`_traverse_for_variables`](_base_traverse_mixin.md#DefaultTraverseMixin._traverse_for_variables), [`extract_functions`](base.md#DefaultExtractor.extract_functions), [`extract_classes`](base.md#DefaultExtractor.extract_classes), [`extract_imports`](base.md#DefaultExtractor.extract_imports), [`extract_variables`](base.md#DefaultExtractor.extract_variables), [`DefaultTraverseAppendMixin`](_base_traverse_mixin.md#DefaultTraverseAppendMixin), [`_append_function`](_base_traverse_mixin.md#DefaultTraverseAppendMixin._append_function), [`_append_class`](_base_traverse_mixin.md#DefaultTraverseAppendMixin._append_class), [`_append_import`](_base_traverse_mixin.md#DefaultTraverseAppendMixin._append_import), [`_append_variable`](_base_traverse_mixin.md#DefaultTraverseAppendMixin._append_variable)  (39 test-only)

### `DefaultTraverseAppendMixin`  ·  implements/extends DefaultNodeMixin
- def: [`tree_sitter_analyzer/plugins/_base_traverse_mixin.py:161`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_base_traverse_mixin.py#L161)
- doc: Build model elements from matched AST nodes.
- signature: `class DefaultTraverseAppendMixin(DefaultNodeMixin):`
- protocol/private: `_append_class`[`L175`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_base_traverse_mixin.py#L175), `_append_function`[`L164`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_base_traverse_mixin.py#L164), `_append_import`[`L197`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_base_traverse_mixin.py#L197), `_append_variable`[`L186`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_base_traverse_mixin.py#L186)
- uses (calls/refs, reference-scoped): [`log_debug`](../utils/logging.md#log_debug), [`Function`](../models/base.md#Function), [`Class`](../models/base.md#Class), [`Variable`](../models/base.md#Variable), [`Import`](../models/base.md#Import), [`DefaultTraverseMixin`](_base_traverse_mixin.md#DefaultTraverseMixin), [`DefaultNodeMixin`](_base_traverse_mixin.md#DefaultNodeMixin), [`_element_fields`](_base_traverse_mixin.md#DefaultNodeMixin._element_fields)
- used by: [`_traverse_for_functions`](_base_traverse_mixin.md#DefaultTraverseMixin._traverse_for_functions), [`DefaultTraverseMixin`](_base_traverse_mixin.md#DefaultTraverseMixin), [`DefaultNodeMixin`](_base_traverse_mixin.md#DefaultNodeMixin), [`_traverse_for_classes`](_base_traverse_mixin.md#DefaultTraverseMixin._traverse_for_classes), [`_traverse_for_imports`](_base_traverse_mixin.md#DefaultTraverseMixin._traverse_for_imports), [`_traverse_for_variables`](_base_traverse_mixin.md#DefaultTraverseMixin._traverse_for_variables)  (5 test-only)

### `DefaultTraverseMixin`  ·  implements/extends DefaultTraverseAppendMixin
- def: [`tree_sitter_analyzer/plugins/_base_traverse_mixin.py:209`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_base_traverse_mixin.py#L209)
- doc: Recursive traversal methods used by the default extractor.
- signature: `class DefaultTraverseMixin(DefaultTraverseAppendMixin):`
- members:
  - `_traverse_for_classes(self, node: tree_sitter.Node, classes: list[ModelClass], lines: list[str], source_code: str)` — [`L226`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_base_traverse_mixin.py#L226) — Traverse tree to find class-like nodes.
  - `_traverse_for_functions(self, node: tree_sitter.Node, functions: list[ModelFunction], lines: list[str], source_code: str)` — [`L212`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_base_traverse_mixin.py#L212) — Traverse tree to find function-like nodes.
  - `_traverse_for_imports(self, node: tree_sitter.Node, imports: list[ModelImport], lines: list[str], source_code: str)` — [`L254`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_base_traverse_mixin.py#L254) — Traverse tree to find import statements.
  - `_traverse_for_variables(self, node: tree_sitter.Node, variables: list[ModelVariable], lines: list[str], source_code: str)` — [`L240`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_base_traverse_mixin.py#L240) — Traverse tree to find variable declarations.
- uses (calls/refs, reference-scoped): [`Function`](../models/base.md#Function), [`Class`](../models/base.md#Class), [`Variable`](../models/base.md#Variable), [`Import`](../models/base.md#Import), [`DefaultExtractor`](base.md#DefaultExtractor), [`_is_class_node`](_base_traverse_mixin.md#DefaultNodeMixin._is_class_node), [`_is_function_node`](_base_traverse_mixin.md#DefaultNodeMixin._is_function_node), [`_is_import_node`](_base_traverse_mixin.md#DefaultNodeMixin._is_import_node), [`_is_variable_node`](_base_traverse_mixin.md#DefaultNodeMixin._is_variable_node), [`DefaultTraverseAppendMixin`](_base_traverse_mixin.md#DefaultTraverseAppendMixin), [`_append_function`](_base_traverse_mixin.md#DefaultTraverseAppendMixin._append_function), [`_append_class`](_base_traverse_mixin.md#DefaultTraverseAppendMixin._append_class), [`_append_import`](_base_traverse_mixin.md#DefaultTraverseAppendMixin._append_import), [`_append_variable`](_base_traverse_mixin.md#DefaultTraverseAppendMixin._append_variable), [`_iter_children`](_base_traverse_mixin.md#_iter_children)
- used by: [`DefaultExtractor`](base.md#DefaultExtractor), [`extract_functions`](base.md#DefaultExtractor.extract_functions), [`extract_classes`](base.md#DefaultExtractor.extract_classes), [`extract_imports`](base.md#DefaultExtractor.extract_imports), [`extract_variables`](base.md#DefaultExtractor.extract_variables), [`DefaultTraverseAppendMixin`](_base_traverse_mixin.md#DefaultTraverseAppendMixin)  (14 test-only)

## Functions
- `_extract_node_text(node: tree_sitter.Node, source_code: str)` — [`L108`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_base_traverse_mixin.py#L108)
- `_find_identifier_child(node: tree_sitter.Node)` — [`L93`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_base_traverse_mixin.py#L93)
- `_format_fallback_node_name(node: tree_sitter.Node)` — [`L104`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_base_traverse_mixin.py#L104)
- `_get_language_hint()` — [`L120`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_base_traverse_mixin.py#L120)
- `_is_class_node(node_type: str)` — [`L81`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_base_traverse_mixin.py#L81)
- `_is_function_node(node_type: str)` — [`L77`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_base_traverse_mixin.py#L77)
- `_is_import_node(node_type: str)` — [`L89`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_base_traverse_mixin.py#L89)
- `_is_variable_node(node_type: str)` — [`L85`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_base_traverse_mixin.py#L85)
- `_iter_children(node: tree_sitter.Node)` — [`L64`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_base_traverse_mixin.py#L64)
- `_node_end_line(node: tree_sitter.Node)` — [`L58`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_base_traverse_mixin.py#L58)
- `_node_start_line(node: tree_sitter.Node)` — [`L52`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_base_traverse_mixin.py#L52)
- `_node_type_matches(node_type: str, candidates: tuple[str, ...])` — [`L72`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_base_traverse_mixin.py#L72)
- `_tree_root_node(tree: tree_sitter.Tree)` — [`L68`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_base_traverse_mixin.py#L68)

## Module values
- `CLASS_NODE_TYPES` — [`L23`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_base_traverse_mixin.py#L23)
- `FUNCTION_NODE_TYPES` — [`L14`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_base_traverse_mixin.py#L14)
- `IMPORT_NODE_TYPES` — [`L41`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_base_traverse_mixin.py#L41)
- `VARIABLE_NODE_TYPES` — [`L32`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/_base_traverse_mixin.py#L32)

