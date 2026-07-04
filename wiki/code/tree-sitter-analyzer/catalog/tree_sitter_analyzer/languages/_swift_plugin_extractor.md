---
title: 'Module: tree_sitter_analyzer/languages/_swift_plugin_extractor.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/_swift_plugin_extractor.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages._swift_plugin_extractor`/
symbols:
  SwiftElementExtractor.extract_functions: SwiftElementExtractor#extract_functions().
  SwiftElementExtractor.extract_classes: SwiftElementExtractor#extract_classes().
  SwiftElementExtractor.extract_variables: SwiftElementExtractor#extract_variables().
  SwiftElementExtractor.extract_imports: SwiftElementExtractor#extract_imports().
  SwiftElementExtractor._prepare_source: SwiftElementExtractor#_prepare_source().
  SwiftElementExtractor: SwiftElementExtractor#
  SwiftElementExtractor.get_node_text: SwiftElementExtractor#get_node_text().
  SwiftElementExtractor._node_text_cache: SwiftElementExtractor#_node_text_cache.
  SwiftElementExtractor.__init__: SwiftElementExtractor#__init__().
  CLASS_NODE_TYPES: CLASS_NODE_TYPES.
  FUNCTION_NODE_TYPES: FUNCTION_NODE_TYPES.
  VARIABLE_NODE_TYPES: VARIABLE_NODE_TYPES.
  SwiftElementExtractor.source_code: SwiftElementExtractor#source_code.
  SwiftElementExtractor.content_lines: SwiftElementExtractor#content_lines.
---
# Module: [`tree_sitter_analyzer/languages/_swift_plugin_extractor.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_swift_plugin_extractor.py)

## Classes
### `SwiftElementExtractor`  ·  implements/extends ElementExtractor
- def: [`tree_sitter_analyzer/languages/_swift_plugin_extractor.py:30`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_swift_plugin_extractor.py#L30)
- doc: Swift-specific element extractor.
- signature: `class SwiftElementExtractor(ElementExtractor):`
- members:
  - `__init__(self)` — [`L33`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_swift_plugin_extractor.py#L33) — Initialize the Swift element extractor.
  - `extract_classes(self, tree: tree_sitter.Tree, source_code: str)` — [`L53`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_swift_plugin_extractor.py#L53) — Extract Swift classes, structs, enums, protocols, and extensions.
  - `extract_functions(self, tree: tree_sitter.Tree, source_code: str)` — [`L40`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_swift_plugin_extractor.py#L40) — Extract Swift functions, methods, initializers, and protocol methods.
  - `extract_imports(self, tree: tree_sitter.Tree, source_code: str)` — [`L77`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_swift_plugin_extractor.py#L77) — Extract Swift import declarations.
  - `extract_variables(self, tree: tree_sitter.Tree, source_code: str)` — [`L64`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_swift_plugin_extractor.py#L64) — Extract Swift let/var property declarations.
  - `get_node_text(self, node: tree_sitter.Node)` — [`L93`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_swift_plugin_extractor.py#L93) — Return cached text for a Swift AST node.
  - `content_lines` — [`L37`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_swift_plugin_extractor.py#L37)
  - `source_code` — [`L36`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_swift_plugin_extractor.py#L36)
- protocol/private: `_node_text_cache`[`L38`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_swift_plugin_extractor.py#L38), `_prepare_source`[`L88`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_swift_plugin_extractor.py#L88)
- uses (calls/refs, reference-scoped): [`log_debug`](../utils/logging.md#log_debug), [`Function`](../models/base.md#Function), [`Class`](../models/base.md#Class), [`Variable`](../models/base.md#Variable), [`Import`](../models/base.md#Import), [`ElementExtractor`](../plugins/base.md#ElementExtractor), [`extract_swift_variable`](_swift_plugin_elements.md#extract_swift_variable), [`extract_swift_class`](_swift_plugin_elements.md#extract_swift_class), [`extract_swift_function`](_swift_plugin_elements.md#extract_swift_function), [`extract_swift_import`](_swift_plugin_elements.md#extract_swift_import), [`decode_node_text`](_swift_plugin_nodes.md#decode_node_text), [`extract_matching_nodes`](_swift_plugin_nodes.md#extract_matching_nodes), [`__init__`](../plugins/base.md#ElementExtractor.__init__), [`CLASS_NODE_TYPES`](_swift_plugin_extractor.md#CLASS_NODE_TYPES), [`FUNCTION_NODE_TYPES`](_swift_plugin_extractor.md#FUNCTION_NODE_TYPES), [`VARIABLE_NODE_TYPES`](_swift_plugin_extractor.md#VARIABLE_NODE_TYPES)
- used by: [`ElementExtractor`](../plugins/base.md#ElementExtractor), [`extract_functions`](../plugins/base.md#ElementExtractor.extract_functions), [`extract_classes`](../plugins/base.md#ElementExtractor.extract_classes), [`extract_variables`](../plugins/base.md#ElementExtractor.extract_variables), [`extract_imports`](../plugins/base.md#ElementExtractor.extract_imports), [`create_extractor`](swift_plugin.md#SwiftPlugin.create_extractor)  (1 test-only)

## Module values
- `CLASS_NODE_TYPES` — [`L21`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_swift_plugin_extractor.py#L21)
- `FUNCTION_NODE_TYPES` — [`L22`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_swift_plugin_extractor.py#L22)
- `VARIABLE_NODE_TYPES` — [`L27`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_swift_plugin_extractor.py#L27)

