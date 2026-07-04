---
title: 'Module: tree_sitter_analyzer/languages/ruby_plugin.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/ruby_plugin.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.ruby_plugin`/
symbols:
  RubyPlugin: RubyPlugin#
  RubyPlugin.analyze_file: RubyPlugin#analyze_file().
  RubyElementExtractor._extract_method_element: RubyElementExtractor#_extract_method_element().
  RubyPlugin.create_extractor: RubyPlugin#create_extractor().
  RubyElementExtractor._extract_singleton_method_element: RubyElementExtractor#_extract_singleton_method_element().
  RubyElementExtractor._extract_class_element: RubyElementExtractor#_extract_class_element().
  RubyElementExtractor._extract_assignment_variable: RubyElementExtractor#_extract_assignment_variable().
  TREE_SITTER_AVAILABLE: TREE_SITTER_AVAILABLE.
  RubyElementExtractor: RubyElementExtractor#
  RubyElementExtractor.extract_functions: RubyElementExtractor#extract_functions().
  RubyElementExtractor.extract_variables: RubyElementExtractor#extract_variables().
  RubyElementExtractor._get_node_text_optimized: RubyElementExtractor#_get_node_text_optimized().
  RubyElementExtractor.extract_classes: RubyElementExtractor#extract_classes().
  RubyPlugin.get_tree_sitter_language: RubyPlugin#get_tree_sitter_language().
  _ruby_calculate_complexity: _ruby_calculate_complexity().
  RubyElementExtractor._reset_caches: RubyElementExtractor#_reset_caches().
  RubyElementExtractor.extract_imports: RubyElementExtractor#extract_imports().
  RubyElementExtractor._extract_attr_methods: RubyElementExtractor#_extract_attr_methods().
  RubyElementExtractor._extract_require_statement: RubyElementExtractor#_extract_require_statement().
  RubyElementExtractor._extract_ruby_parameters: RubyElementExtractor#_extract_ruby_parameters().
  RubyElementExtractor._node_text_cache: RubyElementExtractor#_node_text_cache.
  RubyElementExtractor._determine_visibility: RubyElementExtractor#_determine_visibility().
  RubyElementExtractor.source_code: RubyElementExtractor#source_code.
  RubyPlugin.extract_elements: RubyPlugin#extract_elements().
  RubyElementExtractor._find_ruby_superclass: RubyElementExtractor#_find_ruby_superclass().
  RubyElementExtractor._find_ruby_class_name: RubyElementExtractor#_find_ruby_class_name().
  RubyPlugin._count_nodes: RubyPlugin#_count_nodes().
  RubyElementExtractor.content_lines: RubyElementExtractor#content_lines.
  RubyElementExtractor._element_cache: RubyElementExtractor#_element_cache.
  RubyPlugin._load_file_safe: RubyPlugin#_load_file_safe().
  RubyElementExtractor._processed_nodes: RubyElementExtractor#_processed_nodes.
  RubyElementExtractor.current_module: RubyElementExtractor#current_module.
  RubyPlugin._language_instance: RubyPlugin#_language_instance.
  RubyPlugin.get_language_name: RubyPlugin#get_language_name().
  RubyElementExtractor.__init__: RubyElementExtractor#__init__().
  _ruby_case_has_subject: _ruby_case_has_subject().
  _safe_children: _safe_children().
  _ElementCacheKey: _ElementCacheKey.
  RubyElementExtractor._VISIBILITY_KEYWORDS: RubyElementExtractor#_VISIBILITY_KEYWORDS.
  RubyElementExtractor._RUBY_PARAMETER_NODE_TYPES: RubyElementExtractor#_RUBY_PARAMETER_NODE_TYPES.
  RubyPlugin.get_file_extensions: RubyPlugin#get_file_extensions().
  _RUBY_DECISION_STATEMENT_TYPES._RUBY_DECISION_STATEMENT_TYPES: _RUBY_DECISION_STATEMENT_TYPES._RUBY_DECISION_STATEMENT_TYPES.
  _RUBY_LOGIC_OP_TOKENS._RUBY_LOGIC_OP_TOKENS: _RUBY_LOGIC_OP_TOKENS._RUBY_LOGIC_OP_TOKENS.
---
# Module: [`tree_sitter_analyzer/languages/ruby_plugin.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/ruby_plugin.py)

## Classes
### `RubyElementExtractor`  ·  implements/extends ElementExtractor
- def: [`tree_sitter_analyzer/languages/ruby_plugin.py:135`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/ruby_plugin.py#L135)
- doc: Ruby-specific element extractor.
- signature: `class RubyElementExtractor(ElementExtractor):`
- members:
  - `__init__(self)` — [`L153`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/ruby_plugin.py#L153) — Initialize the Ruby element extractor.
  - `_determine_visibility(self, node: tree_sitter.Node | None)` — [`L201`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/ruby_plugin.py#L201) — Determine visibility by scanning preceding siblings for private/protected/public.
  - `_extract_assignment_variable(self, node: tree_sitter.Node, parent_class: str)` — [`L568`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/ruby_plugin.py#L568) — Extract variable from assignment.
  - `_extract_attr_methods(self, node: tree_sitter.Node, parent_class: str)` — [`L504`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/ruby_plugin.py#L504) — Extract attr_accessor, attr_reader, attr_writer methods.
  - `_extract_class_element(self, node: tree_sitter.Node)` — [`L249`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/ruby_plugin.py#L249) — Extract a single class or module element.
  - `_extract_method_element(self, node: tree_sitter.Node, parent_class: str)` — [`L383`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/ruby_plugin.py#L383) — Extract a method element.
  - `_extract_require_statement(self, node: tree_sitter.Node)` — [`L657`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/ruby_plugin.py#L657) — Extract require statement.
  - `_extract_ruby_parameters(self, params_node: tree_sitter.Node | None)` — [`L439`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/ruby_plugin.py#L439) — Return a list of parameter texts from a Ruby ``parameters`` node.
  - `_extract_singleton_method_element(self, node: tree_sitter.Node, parent_class: str)` — [`L458`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/ruby_plugin.py#L458) — Extract a singleton (class) method element.
  - `_find_ruby_class_name(self, class_or_module_node: tree_sitter.Node)` — [`L367`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/ruby_plugin.py#L367) — Return the first ``constant``/``scope_resolution`` child's text.
  - `_find_ruby_superclass(self, class_node: tree_sitter.Node)` — [`L294`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/ruby_plugin.py#L294) — Find the superclass token under a Ruby ``class`` node.
  - `_get_node_text_optimized(self, node: tree_sitter.Node)` — [`L177`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/ruby_plugin.py#L177) — Get text content of a node with caching for performance.
  - `_reset_caches(self)` — [`L170`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/ruby_plugin.py#L170) — Reset all internal caches for a new file analysis.
  - `extract_classes(self, tree: tree_sitter.Tree, source_code: str)` — [`L215`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/ruby_plugin.py#L215) — Extract Ruby classes and modules.
  - `extract_functions(self, tree: tree_sitter.Tree, source_code: str)` — [`L317`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/ruby_plugin.py#L317) — Extract Ruby methods.
  - `extract_imports(self, tree: tree_sitter.Tree, source_code: str)` — [`L624`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/ruby_plugin.py#L624) — Extract Ruby require statements.
  - `extract_variables(self, tree: tree_sitter.Tree, source_code: str)` — [`L512`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/ruby_plugin.py#L512) — Extract Ruby constants and variables.
  - `content_lines` — [`L162`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/ruby_plugin.py#L162)
  - `current_module` — [`L163`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/ruby_plugin.py#L163)
  - `source_code` — [`L161`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/ruby_plugin.py#L161)
- protocol/private: `_RUBY_PARAMETER_NODE_TYPES`[`L430`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/ruby_plugin.py#L430), `_VISIBILITY_KEYWORDS`[`L199`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/ruby_plugin.py#L199), `_element_cache`[`L168`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/ruby_plugin.py#L168), `_node_text_cache`[`L166`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/ruby_plugin.py#L166), `_processed_nodes`[`L167`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/ruby_plugin.py#L167)
- uses (calls/refs, reference-scoped): [`name`](../models/base.md#CodeElement.name), [`start_line`](../models/base.md#CodeElement.start_line), [`end_line`](../models/base.md#CodeElement.end_line), [`Function`](../models/base.md#Function), [`log_error`](../utils/logging.md#log_error), [`Class`](../models/base.md#Class), [`Variable`](../models/base.md#Variable), [`Import`](../models/base.md#Import), [`ElementExtractor`](../plugins/base.md#ElementExtractor), [`complexity_score`](../models/base.md#Function.complexity_score), [`parameters`](../models/base.md#Function.parameters), [`return_type`](../models/base.md#Function.return_type), [`class_type`](../models/base.md#Class.class_type), [`visibility`](../models/base.md#Function.visibility), [`get_node_text_safe`](../utils/tree_sitter_compat.md#get_node_text_safe), [`receiver_type`](../models/base.md#Function.receiver_type), [`variable_type`](../models/base.md#Variable.variable_type), [`interfaces`](../models/base.md#Class.interfaces), [`is_async`](../models/base.md#Function.is_async), [`superclass`](../models/base.md#Class.superclass), [`full_qualified_name`](../models/base.md#Class.full_qualified_name), [`visibility`](../models/base.md#Variable.visibility), [`is_constant`](../models/base.md#Variable.is_constant), [`modifiers`](../models/base.md#Class.modifiers), [`modifiers`](../models/base.md#Function.modifiers), [`visibility`](../models/base.md#Class.visibility), [`is_static`](../models/base.md#Function.is_static), [`is_constructor`](../models/base.md#Function.is_constructor), [`is_abstract`](../models/base.md#Function.is_abstract), [`modifiers`](../models/base.md#Variable.modifiers), [`extract_require_statement`](ruby_helpers.md#extract_require_statement), [`is_static`](../models/base.md#Variable.is_static), [`_ruby_calculate_complexity`](ruby_plugin.md#_ruby_calculate_complexity), [`annotations`](../models/base.md#Class.annotations), [`annotations`](../models/base.md#Function.annotations), [`extract_attr_methods`](ruby_helpers.md#extract_attr_methods), [`is_abstract`](../models/base.md#Class.is_abstract), [`is_final`](../models/base.md#Variable.is_final), [`__init__`](../plugins/base.md#ElementExtractor.__init__), [`_ElementCacheKey`](ruby_plugin.md#_ElementCacheKey)
- used by: [`ElementExtractor`](../plugins/base.md#ElementExtractor), [`extract_functions`](../plugins/base.md#ElementExtractor.extract_functions), [`extract_classes`](../plugins/base.md#ElementExtractor.extract_classes), [`extract_variables`](../plugins/base.md#ElementExtractor.extract_variables), [`extract_imports`](../plugins/base.md#ElementExtractor.extract_imports), [`create_extractor`](ruby_plugin.md#RubyPlugin.create_extractor)  (16 test-only)

### `RubyPlugin`  ·  implements/extends LanguagePlugin
- def: [`tree_sitter_analyzer/languages/ruby_plugin.py:662`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/ruby_plugin.py#L662) — documented in [tree_sitter_analyzer-plugins-manager](../../../concepts/tree_sitter_analyzer-plugins-manager.md)
- doc: Ruby language plugin.
- signature: `class RubyPlugin(LanguagePlugin):`
- members:
  - `_count_nodes(self, node: tree_sitter.Node)` — [`L787`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/ruby_plugin.py#L787) — Count total nodes in the AST.
  - `_load_file_safe(self, file_path: str)` — [`L802`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/ruby_plugin.py#L802) — Load file content with encoding detection.
  - `analyze_file(self, file_path: str, request: AnalysisRequest)` — [`L734`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/ruby_plugin.py#L734) — Analyze a Ruby file. — documented in [tree_sitter_analyzer-models-result](../../../concepts/tree_sitter_analyzer-models-result.md)
  - `create_extractor(self)` — [`L719`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/ruby_plugin.py#L719) — Create a Ruby element extractor. — documented in [tree_sitter_analyzer-plugins-base](../../../concepts/tree_sitter_analyzer-plugins-base.md)
  - `extract_elements(self, tree: tree_sitter.Tree, source_code: str)` — [`L728`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/ruby_plugin.py#L728) — Unified extraction entry point — delegates to the extractor.
  - `get_file_extensions(self)` — [`L681`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/ruby_plugin.py#L681) — Get supported file extensions.
  - `get_language_name(self)` — [`L672`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/ruby_plugin.py#L672) — Get the name of the language.
  - `get_tree_sitter_language(self)` — [`L690`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/ruby_plugin.py#L690) — Get the tree-sitter language instance for Ruby.
- protocol/private: `_language_instance`[`L670`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/ruby_plugin.py#L670)
- uses (calls/refs, reference-scoped): [`AnalysisResult`](../models/result.md#AnalysisResult), [`log_error`](../utils/logging.md#log_error), [`AnalysisRequest`](../core/request.md#AnalysisRequest), [`elements`](../models/result.md#AnalysisResult.elements), [`language`](../models/result.md#AnalysisResult.language), [`LanguagePlugin`](../plugins/base.md#LanguagePlugin), [`file_path`](../models/result.md#AnalysisResult.file_path), [`success`](../models/result.md#AnalysisResult.success), [`ElementExtractor`](../plugins/base.md#ElementExtractor), [`extract_functions`](../plugins/base.md#ElementExtractor.extract_functions), [`extract_classes`](../plugins/base.md#ElementExtractor.extract_classes), [`line_count`](../models/result.md#AnalysisResult.line_count), [`extract_variables`](../plugins/base.md#ElementExtractor.extract_variables), [`error_message`](../models/result.md#AnalysisResult.error_message), [`extract_imports`](../plugins/base.md#ElementExtractor.extract_imports), [`node_count`](../models/result.md#AnalysisResult.node_count), [`extract_elements`](../plugins/base.md#ElementExtractor.extract_elements), [`TREE_SITTER_AVAILABLE`](ruby_plugin.md#TREE_SITTER_AVAILABLE), [`RubyElementExtractor`](ruby_plugin.md#RubyElementExtractor)
- used by: [`LanguagePlugin`](../plugins/base.md#LanguagePlugin), [`get_language_name`](../plugins/base.md#LanguagePlugin.get_language_name), [`analyze_file`](../plugins/base.md#LanguagePlugin.analyze_file), [`get_file_extensions`](../plugins/base.md#LanguagePlugin.get_file_extensions), [`create_extractor`](../plugins/base.md#LanguagePlugin.create_extractor), [`get_tree_sitter_language`](../plugins/base.md#LanguagePlugin.get_tree_sitter_language)  (53 test-only)

## Functions
- `_ruby_calculate_complexity(node: object)` — [`L80`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/ruby_plugin.py#L80) — Return cyclomatic complexity for a Ruby method node.
- `_ruby_case_has_subject(case_node: Any)` — [`L122`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/ruby_plugin.py#L122) — True for a valued ``case expr`` (switch); False for conditionless ``case``.
- `_safe_children(node: object)` — [`L69`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/ruby_plugin.py#L69) — Return children list from a tree-sitter node, empty list on any error.

## Module values
- `TREE_SITTER_AVAILABLE` — [`L22`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/ruby_plugin.py#L22)
- `_ElementCacheKey` — [`L132`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/ruby_plugin.py#L132)
- `_RUBY_DECISION_STATEMENT_TYPES` — [`L44`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/ruby_plugin.py#L44)
- `_RUBY_LOGIC_OP_TOKENS` — [`L66`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/ruby_plugin.py#L66)

