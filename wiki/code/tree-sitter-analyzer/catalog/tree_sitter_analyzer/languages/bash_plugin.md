---
title: 'Module: tree_sitter_analyzer/languages/bash_plugin.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/bash_plugin.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.bash_plugin`/
symbols:
  BashElementExtractor.extract_expressions: BashElementExtractor#extract_expressions().
  BashPlugin.analyze_file: BashPlugin#analyze_file().
  TREE_SITTER_AVAILABLE: TREE_SITTER_AVAILABLE.
  BashElementExtractor._extract_function: BashElementExtractor#_extract_function().
  BashElementExtractor._extract_control_flow: BashElementExtractor#_extract_control_flow().
  BashElementExtractor._extract_string_pattern: BashElementExtractor#_extract_string_pattern().
  BashElementExtractor._get_node_text_optimized: BashElementExtractor#_get_node_text_optimized().
  BashElementExtractor._extract_subscript: BashElementExtractor#_extract_subscript().
  BashElementExtractor._extract_redirect: BashElementExtractor#_extract_redirect().
  BashElementExtractor._extract_subshell: BashElementExtractor#_extract_subshell().
  BashElementExtractor._extract_array: BashElementExtractor#_extract_array().
  BashElementExtractor._extract_list: BashElementExtractor#_extract_list().
  BashElementExtractor._extract_process_substitution: BashElementExtractor#_extract_process_substitution().
  BashElementExtractor._extract_comment: BashElementExtractor#_extract_comment().
  BashPlugin: BashPlugin#
  BashElementExtractor._extract_variable: BashElementExtractor#_extract_variable().
  BashElementExtractor.extract_functions: BashElementExtractor#extract_functions().
  BashElementExtractor.extract_variables: BashElementExtractor#extract_variables().
  BashPlugin._analyze_sync: BashPlugin#_analyze_sync().
  BashElementExtractor: BashElementExtractor#
  BashPlugin.create_extractor: BashPlugin#create_extractor().
  BashElementExtractor._traverse_and_extract_iterative: BashElementExtractor#_traverse_and_extract_iterative().
  BashPlugin.get_extractor: BashPlugin#get_extractor().
  BashPlugin.get_tree_sitter_language: BashPlugin#get_tree_sitter_language().
  BashElementExtractor.extract_elements: BashElementExtractor#extract_elements().
  BashPlugin.get_plugin_info: BashPlugin#get_plugin_info().
  BashElementExtractor.content_lines: BashElementExtractor#content_lines.
  calculate_bash_complexity: calculate_bash_complexity().
  BashElementExtractor._reset_caches: BashElementExtractor#_reset_caches().
  BashElementExtractor.source_code: BashElementExtractor#source_code.
  BashElementExtractor._node_text_cache: BashElementExtractor#_node_text_cache.
  BashPlugin.get_language_name: BashPlugin#get_language_name().
  BashPlugin.extract_elements: BashPlugin#extract_elements().
  BashPlugin._extractor: BashPlugin#_extractor.
  BashPlugin.is_applicable: BashPlugin#is_applicable().
  BashElementExtractor._extract_multiline_text: BashElementExtractor#_extract_multiline_text().
  BashElementExtractor._try_extract_bash_node: BashElementExtractor#_try_extract_bash_node().
  BashElementExtractor._processed_nodes: BashElementExtractor#_processed_nodes.
  BashPlugin._language_cache: BashPlugin#_language_cache.
  BashPlugin.get_file_extensions: BashPlugin#get_file_extensions().
  BashPlugin.extractor: BashPlugin#extractor.
  _safe_children_bash: _safe_children_bash().
  _push_bash_children: _push_bash_children().
  BashElementExtractor._file_encoding: BashElementExtractor#_file_encoding.
  BashElementExtractor.extract_classes: BashElementExtractor#extract_classes().
  BashElementExtractor.extract_imports: BashElementExtractor#extract_imports().
  BashElementExtractor._extract_function_name: BashElementExtractor#_extract_function_name().
  BashPlugin.get_supported_queries: BashPlugin#get_supported_queries().
  _BASH_CONTAINER_NODE_TYPES._BASH_CONTAINER_NODE_TYPES: _BASH_CONTAINER_NODE_TYPES._BASH_CONTAINER_NODE_TYPES.
  _BASH_DECISION_TYPES._BASH_DECISION_TYPES: _BASH_DECISION_TYPES._BASH_DECISION_TYPES.
  _BASH_LOGIC_OP_TOKENS._BASH_LOGIC_OP_TOKENS: _BASH_LOGIC_OP_TOKENS._BASH_LOGIC_OP_TOKENS.
  BashElementExtractor.__init__: BashElementExtractor#__init__().
  BashPlugin.__init__: BashPlugin#__init__().
  BashPlugin.language: BashPlugin#language.
---
# Module: [`tree_sitter_analyzer/languages/bash_plugin.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/bash_plugin.py)

## Classes
### `BashElementExtractor`  ·  implements/extends ElementExtractor
- def: [`tree_sitter_analyzer/languages/bash_plugin.py:165`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/bash_plugin.py#L165)
- doc: Bash-specific element extractor for shell scripts
- signature: `class BashElementExtractor(ElementExtractor):`
- members:
  - `__init__(self)` — [`L168`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/bash_plugin.py#L168) — Initialize the Bash element extractor.
  - `_extract_array(self, node: tree_sitter.Node)` — [`L592`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/bash_plugin.py#L592) — Extract array expressions
  - `_extract_comment(self, node: tree_sitter.Node)` — [`L738`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/bash_plugin.py#L738) — Extract comment nodes, skipping shebang lines (#!).
  - `_extract_control_flow(self, node: tree_sitter.Node)` — [`L538`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/bash_plugin.py#L538) — Extract control flow statements (while, for, case, if branches)
  - `_extract_function(self, node: tree_sitter.Node)` — [`L498`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/bash_plugin.py#L498) — Extract Bash function information
  - `_extract_function_name(self, node: tree_sitter.Node)` — [`L526`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/bash_plugin.py#L526) — Extract function name from function_definition node
  - `_extract_list(self, node: tree_sitter.Node)` — [`L664`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/bash_plugin.py#L664) — Extract list expressions (command lists with && or ||)
  - `_extract_multiline_text(self, start_point: tuple[int, int], end_point: tuple[int, int])` — [`L396`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/bash_plugin.py#L396) — Slice multi-line node text from ``self.content_lines``.
  - `_extract_process_substitution(self, node: tree_sitter.Node)` — [`L715`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/bash_plugin.py#L715) — Extract process substitution expressions
  - `_extract_redirect(self, node: tree_sitter.Node)` — [`L685`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/bash_plugin.py#L685) — Extract redirection expressions
  - `_extract_string_pattern(self, node: tree_sitter.Node)` — [`L770`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/bash_plugin.py#L770) — Extract string and pattern expressions
  - `_extract_subscript(self, node: tree_sitter.Node)` — [`L613`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/bash_plugin.py#L613) — Extract subscript/array indexing expressions.
  - `_extract_subshell(self, node: tree_sitter.Node)` — [`L571`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/bash_plugin.py#L571) — Extract subshell expressions
  - `_extract_variable(self, node: tree_sitter.Node)` — [`L297`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/bash_plugin.py#L297) — Extract a Bash variable from a ``variable_assignment`` node.
  - `_get_node_text_optimized(self, node: tree_sitter.Node)` — [`L451`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/bash_plugin.py#L451) — Get node text with optimized caching
  - `_reset_caches(self)` — [`L341`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/bash_plugin.py#L341) — Reset performance caches
  - `_traverse_and_extract_iterative(self, root_node: tree_sitter.Node | None, extractors: dict[str, Any], results: list[Any], element_type: str)` — [`L346`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/bash_plugin.py#L346) — Iterative node traversal and extraction.
  - `_try_extract_bash_node(self, current_node: tree_sitter.Node, node_type: str, extractors: dict[str, Any], results: list[Any])` — [`L423`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/bash_plugin.py#L423) — Look up the extractor for a node type and append its result.
  - `extract_classes(self, tree: tree_sitter.Tree, source_code: str)` — [`L260`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/bash_plugin.py#L260) — Bash does not have classes
  - `extract_elements(self, tree: tree_sitter.Tree, source_code: str)` — [`L330`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/bash_plugin.py#L330) — Unified extraction entry point grouped by type.
  - `extract_expressions(self, tree: tree_sitter.Tree, source_code: str)` — [`L205`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/bash_plugin.py#L205) — Extract Bash expressions (control flow, arrays, redirects, etc.)
  - `extract_functions(self, tree: tree_sitter.Tree, source_code: str)` — [`L178`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/bash_plugin.py#L178) — Extract Bash function definitions
  - `extract_imports(self, tree: tree_sitter.Tree, source_code: str)` — [`L326`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/bash_plugin.py#L326) — Bash does not have traditional imports (source statements are handled separately)
  - `extract_variables(self, tree: tree_sitter.Tree, source_code: str)` — [`L264`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/bash_plugin.py#L264) — Extract Bash variable assignments.
  - `content_lines` — [`L171`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/bash_plugin.py#L171)
  - `source_code` — [`L170`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/bash_plugin.py#L170)
- protocol/private: `_file_encoding`[`L176`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/bash_plugin.py#L176), `_node_text_cache`[`L174`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/bash_plugin.py#L174), `_processed_nodes`[`L175`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/bash_plugin.py#L175)
- uses (calls/refs, reference-scoped): [`name`](../models/base.md#CodeElement.name), [`start_line`](../models/base.md#CodeElement.start_line), [`end_line`](../models/base.md#CodeElement.end_line), [`log_debug`](../utils/logging.md#log_debug), [`language`](../models/base.md#CodeElement.language), [`Function`](../models/base.md#Function), [`raw_text`](../models/base.md#CodeElement.raw_text), [`log_error`](../utils/logging.md#log_error), [`Variable`](../models/base.md#Variable), [`ElementExtractor`](../plugins/base.md#ElementExtractor), [`complexity_score`](../models/base.md#Function.complexity_score), [`parameters`](../models/base.md#Function.parameters), [`return_type`](../models/base.md#Function.return_type), [`safe_encode`](../encoding_utils.md#safe_encode), [`Expression`](../models/base.md#Expression), [`extract_text_slice`](../encoding_utils.md#extract_text_slice), [`expression_kind`](../models/base.md#Expression.expression_kind), [`preview`](../models/base.md#Expression.preview), [`calculate_bash_complexity`](bash_plugin.md#calculate_bash_complexity), [`initializer`](../models/base.md#Variable.initializer), [`_BASH_CONTAINER_NODE_TYPES`](bash_plugin.md#_BASH_CONTAINER_NODE_TYPES._BASH_CONTAINER_NODE_TYPES), [`_push_bash_children`](bash_plugin.md#_push_bash_children)
- used by: [`ElementExtractor`](../plugins/base.md#ElementExtractor), [`extract_functions`](../plugins/base.md#ElementExtractor.extract_functions), [`extract_classes`](../plugins/base.md#ElementExtractor.extract_classes), [`extract_variables`](../plugins/base.md#ElementExtractor.extract_variables), [`extract_imports`](../plugins/base.md#ElementExtractor.extract_imports), [`extract_elements`](../plugins/base.md#ElementExtractor.extract_elements), [`create_extractor`](bash_plugin.md#BashPlugin.create_extractor), [`get_extractor`](bash_plugin.md#BashPlugin.get_extractor), [`_extractor`](bash_plugin.md#BashPlugin._extractor), [`extract_expressions`](../plugins/base.md#ElementExtractor.extract_expressions)  (7 test-only)

### `BashPlugin`  ·  implements/extends LanguagePlugin
- def: [`tree_sitter_analyzer/languages/bash_plugin.py:803`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/bash_plugin.py#L803)
- doc: Bash language plugin
- signature: `class BashPlugin(LanguagePlugin):`
- members:
  - `__init__(self)` — [`L806`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/bash_plugin.py#L806) — Initialize the Bash plugin
  - `analyze_file(self, file_path: str, request: AnalysisRequest)` — [`L896`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/bash_plugin.py#L896) — Analyze a Bash file and return the analysis results — documented in [tree_sitter_analyzer-models-result](../../../concepts/tree_sitter_analyzer-models-result.md)
  - `create_extractor(self)` — [`L824`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/bash_plugin.py#L824) — Create and return an element extractor for this language
  - `extract_elements(self, tree: tree_sitter.Tree, source_code: str)` — [`L834`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/bash_plugin.py#L834) — Unified extraction entry point — delegates to the extractor.
  - `get_extractor(self)` — [`L828`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/bash_plugin.py#L828) — Get the cached extractor instance
  - `get_file_extensions(self)` — [`L820`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/bash_plugin.py#L820) — Return list of file extensions this plugin supports
  - `get_language_name(self)` — [`L816`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/bash_plugin.py#L816) — Return the name of the programming language this plugin supports
  - `get_plugin_info(self)` — [`L877`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/bash_plugin.py#L877) — Get information about this plugin
  - `get_supported_queries(self)` — [`L857`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/bash_plugin.py#L857) — Get list of supported query names for this language
  - `get_tree_sitter_language(self)` — [`L840`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/bash_plugin.py#L840) — Get the Tree-sitter language object for Bash
  - `is_applicable(self, file_path: str)` — [`L870`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/bash_plugin.py#L870) — Check if this plugin is applicable for the given file
  - `extractor` — [`L814`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/bash_plugin.py#L814)
  - `language` — [`L813`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/bash_plugin.py#L813)
- protocol/private: `_analyze_sync`[`L924`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/bash_plugin.py#L924), `_extractor`[`L810`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/bash_plugin.py#L810), `_language_cache`[`L809`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/bash_plugin.py#L809)
- uses (calls/refs, reference-scoped): [`AnalysisResult`](../models/result.md#AnalysisResult), [`log_error`](../utils/logging.md#log_error), [`AnalysisRequest`](../core/request.md#AnalysisRequest), [`elements`](../models/result.md#AnalysisResult.elements), [`language`](../models/result.md#AnalysisResult.language), [`CodeElement`](../models/base.md#CodeElement), [`LanguagePlugin`](../plugins/base.md#LanguagePlugin), [`file_path`](../models/result.md#AnalysisResult.file_path), [`success`](../models/result.md#AnalysisResult.success), [`ElementExtractor`](../plugins/base.md#ElementExtractor), [`extract_functions`](../plugins/base.md#ElementExtractor.extract_functions), [`line_count`](../models/result.md#AnalysisResult.line_count), [`extract_variables`](../plugins/base.md#ElementExtractor.extract_variables), [`error_message`](../models/result.md#AnalysisResult.error_message), [`node_count`](../models/result.md#AnalysisResult.node_count), [`TREE_SITTER_AVAILABLE`](bash_plugin.md#TREE_SITTER_AVAILABLE), [`extract_elements`](../plugins/base.md#ElementExtractor.extract_elements), [`read_file_safe_async`](../encoding_utils.md#read_file_safe_async), [`BashElementExtractor`](bash_plugin.md#BashElementExtractor), [`count_nodes_iterative`](../utils/tree_sitter_compat.md#count_nodes_iterative), [`extract_expressions`](../plugins/base.md#ElementExtractor.extract_expressions)
- used by: [`LanguagePlugin`](../plugins/base.md#LanguagePlugin), [`get_language_name`](../plugins/base.md#LanguagePlugin.get_language_name), [`analyze_file`](../plugins/base.md#LanguagePlugin.analyze_file), [`get_file_extensions`](../plugins/base.md#LanguagePlugin.get_file_extensions), [`create_extractor`](../plugins/base.md#LanguagePlugin.create_extractor), [`get_tree_sitter_language`](../plugins/base.md#LanguagePlugin.get_tree_sitter_language), [`is_applicable`](../plugins/base.md#LanguagePlugin.is_applicable), [`get_plugin_info`](../plugins/base.md#LanguagePlugin.get_plugin_info)  (19 test-only)

## Functions
- `_push_bash_children(node_stack: list[tuple[tree_sitter.Node, int]], current_node: tree_sitter.Node, depth: int)` — [`L137`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/bash_plugin.py#L137) — Append ``current_node.children`` to ``node_stack`` in reversed order.
- `_safe_children_bash(node: Any)` — [`L103`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/bash_plugin.py#L103) — Return children list from a tree-sitter node, empty list on any error.
- `calculate_bash_complexity(node: Any)` — [`L114`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/bash_plugin.py#L114) — Return cyclomatic complexity for a Bash function node.

## Module values
- `TREE_SITTER_AVAILABLE` — [`L26`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/bash_plugin.py#L26)
- `_BASH_CONTAINER_NODE_TYPES` — [`L47`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/bash_plugin.py#L47)
- `_BASH_DECISION_TYPES` — [`L86`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/bash_plugin.py#L86)
- `_BASH_LOGIC_OP_TOKENS` — [`L100`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/bash_plugin.py#L100)

