---
title: 'Module: tree_sitter_analyzer/languages/go_plugin.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/go_plugin.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.go_plugin`/Go
symbols:
  GoPlugin.analyze_file: Plugin#analyze_file().
  GoElementExtractor: ElementExtractor#
  GoElementExtractor.extract_functions: ElementExtractor#extract_functions().
  GoElementExtractor.extract_variables: ElementExtractor#extract_variables().
  GoElementExtractor._get_node_text: ElementExtractor#_get_node_text().
  GoElementExtractor.extract_packages: ElementExtractor#extract_packages().
  GoPlugin: Plugin#
  GoElementExtractor.extract_imports: ElementExtractor#extract_imports().
  GoElementExtractor.extract_classes: ElementExtractor#extract_classes().
  GoPlugin.extract_elements: Plugin#extract_elements().
  GoElementExtractor.content_lines: ElementExtractor#content_lines.
  GoElementExtractor._reset_caches: ElementExtractor#_reset_caches().
  GoElementExtractor.source_code: ElementExtractor#source_code.
  GoElementExtractor._traverse_and_extract: ElementExtractor#_traverse_and_extract().
  GoElementExtractor._extract_function: ElementExtractor#_extract_function().
  GoElementExtractor._extract_method: ElementExtractor#_extract_method().
  GoElementExtractor._extract_interface_methods: ElementExtractor#_extract_interface_methods().
  GoElementExtractor._extract_type_spec: ElementExtractor#_extract_type_spec().
  GoElementExtractor._extract_type_declaration: ElementExtractor#_extract_type_declaration().
  GoPlugin.create_extractor: Plugin#create_extractor().
  GoElementExtractor._traverse_for_types: ElementExtractor#_traverse_for_types().
  GoElementExtractor._extract_var_or_const: ElementExtractor#_extract_var_or_const().
  GoPlugin.get_tree_sitter_language: Plugin#get_tree_sitter_language().
  GoElementExtractor._extract_package: ElementExtractor#_extract_package().
  GoElementExtractor._extract_struct_fields: ElementExtractor#_extract_struct_fields().
  GoElementExtractor._extract_goroutine: ElementExtractor#_extract_goroutine().
  GoElementExtractor._extract_channel_operation: ElementExtractor#_extract_channel_operation().
  GoElementExtractor._extract_defer: ElementExtractor#_extract_defer().
  GoElementExtractor._extract_import_declaration: ElementExtractor#_extract_import_declaration().
  GoElementExtractor._extract_import_spec: ElementExtractor#_extract_import_spec().
  GoElementExtractor._extract_var_spec: ElementExtractor#_extract_var_spec().
  GoPlugin._cached_language: Plugin#_cached_language.
  GoElementExtractor.goroutines: ElementExtractor#goroutines.
  GoElementExtractor.channels: ElementExtractor#channels.
  GoElementExtractor.defers: ElementExtractor#defers.
  GoElementExtractor._node_text_cache: ElementExtractor#_node_text_cache.
  GoElementExtractor._extract_const_declaration: ElementExtractor#_extract_const_declaration().
  GoElementExtractor._extract_var_declaration: ElementExtractor#_extract_var_declaration().
  GoElementExtractor._extract_parameters: ElementExtractor#_extract_parameters().
  GoElementExtractor._extract_return_type: ElementExtractor#_extract_return_type().
  GoElementExtractor._extract_embedded_types: ElementExtractor#_extract_embedded_types().
  GoElementExtractor._extract_docstring: ElementExtractor#_extract_docstring().
  GoPlugin._count_tree_nodes: Plugin#_count_tree_nodes().
  GoPlugin.get_queries: Plugin#get_queries().
  GoPlugin.extractor: Plugin#extractor.
  GoPlugin.supported_extensions: Plugin#supported_extensions.
  GoPlugin.get_file_extensions: Plugin#get_file_extensions().
  GoElementExtractor.current_package: ElementExtractor#current_package.
  GoPlugin.get_language_name: Plugin#get_language_name().
  GoPlugin.get_supported_element_types: Plugin#get_supported_element_types().
  GoElementExtractor.__init__: ElementExtractor#__init__().
  GoElementExtractor.current_file: ElementExtractor#current_file.
  GoPlugin.__init__: Plugin#__init__().
  GoPlugin.language: Plugin#language.
---
# Module: [`tree_sitter_analyzer/languages/go_plugin.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/go_plugin.py)

## Classes
### `GoElementExtractor`  ·  implements/extends ElementExtractor
- def: [`tree_sitter_analyzer/languages/go_plugin.py:62`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/go_plugin.py#L62)
- doc: Go-specific element extractor
- signature: `class GoElementExtractor(ElementExtractor):`
- members:
  - `__init__(self)` — [`L65`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/go_plugin.py#L65) — Initialize the Go element extractor.
  - `_extract_channel_operation(self, node: tree_sitter.Node, op_type: str)` — [`L329`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/go_plugin.py#L329) — Extract channel operation
  - `_extract_const_declaration(self, node: tree_sitter.Node)` — [`L282`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/go_plugin.py#L282) — Extract const declaration
  - `_extract_defer(self, node: tree_sitter.Node)` — [`L343`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/go_plugin.py#L343) — Extract defer statement
  - `_extract_docstring(self, node: tree_sitter.Node)` — [`L356`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/go_plugin.py#L356) — Extract doc comments preceding the node
  - `_extract_embedded_types(self, struct_node: tree_sitter.Node)` — [`L277`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/go_plugin.py#L277) — Extract embedded types from struct
  - `_extract_function(self, node: tree_sitter.Node)` — [`L236`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/go_plugin.py#L236) — Extract function declaration
  - `_extract_goroutine(self, node: tree_sitter.Node)` — [`L316`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/go_plugin.py#L316) — Extract goroutine invocation
  - `_extract_import_declaration(self, node: tree_sitter.Node)` — [`L221`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/go_plugin.py#L221) — Extract import declaration (may contain multiple imports)
  - `_extract_import_spec(self, node: tree_sitter.Node)` — [`L231`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/go_plugin.py#L231) — Extract single import spec
  - `_extract_interface_methods(self, node: tree_sitter.Node)` — [`L246`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/go_plugin.py#L246) — Extract interface method signatures owned by the interface (#588)
  - `_extract_method(self, node: tree_sitter.Node)` — [`L241`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/go_plugin.py#L241) — Extract method declaration (function with receiver)
  - `_extract_package(self, node: tree_sitter.Node)` — [`L214`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/go_plugin.py#L214) — Extract package declaration
  - `_extract_parameters(self, node: tree_sitter.Node)` — [`L253`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/go_plugin.py#L253) — Extract function/method parameters
  - `_extract_return_type(self, node: tree_sitter.Node)` — [`L258`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/go_plugin.py#L258) — Extract function/method return type
  - `_extract_struct_fields(self, node: tree_sitter.Node)` — [`L311`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/go_plugin.py#L311) — Extract struct field declarations from a type_declaration node.
  - `_extract_type_declaration(self, node: tree_sitter.Node)` — [`L263`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/go_plugin.py#L263) — Extract type declaration (struct, interface, type alias)
  - `_extract_type_spec(self, node: tree_sitter.Node)` — [`L270`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/go_plugin.py#L270) — Extract single type spec
  - `_extract_var_declaration(self, node: tree_sitter.Node)` — [`L289`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/go_plugin.py#L289) — Extract var declaration
  - `_extract_var_or_const(self, node: tree_sitter.Node, is_const: bool)` — [`L294`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/go_plugin.py#L294) — Extract var or const declaration
  - `_extract_var_spec(self, node: tree_sitter.Node, is_const: bool)` — [`L304`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/go_plugin.py#L304) — Extract single var/const spec
  - `_get_node_text(self, node: tree_sitter.Node)` — [`L360`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/go_plugin.py#L360) — Get node text with caching using position-based keys
  - `_reset_caches(self)` — [`L169`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/go_plugin.py#L169) — Reset performance caches
  - `_traverse_and_extract(self, node: tree_sitter.Node, extractors: dict[str, Any], results: list[Any])` — [`L177`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/go_plugin.py#L177) — Recursive traversal to find and extract elements
  - `_traverse_for_types(self, node: tree_sitter.Node, results: list[Class])` — [`L203`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/go_plugin.py#L203) — Traverse to find type declarations
  - `extract_classes(self, tree: tree_sitter.Tree, source_code: str)` — [`L101`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/go_plugin.py#L101) — Extract Go struct and interface definitions
  - `extract_functions(self, tree: tree_sitter.Tree, source_code: str)` — [`L77`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/go_plugin.py#L77) — Extract Go function and method declarations
  - `extract_imports(self, tree: tree_sitter.Tree, source_code: str)` — [`L138`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/go_plugin.py#L138) — Extract Go import declarations
  - `extract_packages(self, tree: tree_sitter.Tree, source_code: str)` — [`L148`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/go_plugin.py#L148) — Extract Go package declaration
  - `extract_variables(self, tree: tree_sitter.Tree, source_code: str)` — [`L116`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/go_plugin.py#L116) — Extract Go const and var declarations
  - `channels` — [`L74`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/go_plugin.py#L74)
  - `content_lines` — [`L70`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/go_plugin.py#L70)
  - `current_file` — [`L68`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/go_plugin.py#L68)
  - `current_package` — [`L67`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/go_plugin.py#L67)
  - `defers` — [`L75`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/go_plugin.py#L75)
  - `goroutines` — [`L73`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/go_plugin.py#L73)
  - `source_code` — [`L69`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/go_plugin.py#L69)
- protocol/private: `_node_text_cache`[`L71`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/go_plugin.py#L71)
- uses (calls/refs, reference-scoped): [`name`](../models/base.md#CodeElement.name), [`log_debug`](../utils/logging.md#log_debug), [`Function`](../models/base.md#Function), [`log_error`](../utils/logging.md#log_error), [`Class`](../models/base.md#Class), [`Variable`](../models/base.md#Variable), [`Import`](../models/base.md#Import), [`ElementExtractor`](../plugins/base.md#ElementExtractor), [`Package`](../models/base.md#Package), [`safe_encode`](../encoding_utils.md#safe_encode), [`extract_text_slice`](../encoding_utils.md#extract_text_slice), [`extract_go_method`](_go_function_helpers.md#extract_go_method), [`extract_go_package`](_go_package_helpers.md#extract_go_package), [`extract_go_interface_methods`](_go_function_helpers.md#extract_go_interface_methods), [`extract_go_function`](_go_function_helpers.md#extract_go_function), [`extract_type_declaration`](_go_type_helpers.md#extract_type_declaration), [`_extract_import_declaration`](_go_import_helpers.md#_extract_import_declaration), [`extract_go_type_spec`](_go_type_helpers.md#extract_go_type_spec), [`extract_import_spec`](_go_import_helpers.md#extract_import_spec), [`extract_docstring`](_go_common_helpers.md#extract_docstring), [`extract_var_spec`](_go_variable_helpers.md#extract_var_spec), [`extract_parameters`](_go_common_helpers.md#extract_parameters), [`extract_var_or_const`](_go_variable_helpers.md#extract_var_or_const), [`extract_embedded_types`](_go_type_helpers.md#extract_embedded_types), [`extract_struct_fields`](_go_variable_helpers.md#extract_struct_fields), [`extract_imports_from_tree`](_go_import_helpers.md#extract_imports_from_tree), [`extract_return_type`](_go_common_helpers.md#extract_return_type)
- used by: [`ElementExtractor`](../plugins/base.md#ElementExtractor), [`extract_functions`](../plugins/base.md#ElementExtractor.extract_functions), [`extract_classes`](../plugins/base.md#ElementExtractor.extract_classes), [`extract_variables`](../plugins/base.md#ElementExtractor.extract_variables), [`extract_imports`](../plugins/base.md#ElementExtractor.extract_imports), [`analyze_file`](go_plugin.md#GoPlugin.analyze_file), [`extract_packages`](../plugins/base.md#ElementExtractor.extract_packages), [`create_extractor`](go_plugin.md#GoPlugin.create_extractor), [`extractor`](go_plugin.md#GoPlugin.extractor)  (31 test-only)

### `GoPlugin`  ·  implements/extends LanguagePlugin
- def: [`tree_sitter_analyzer/languages/go_plugin.py:378`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/go_plugin.py#L378)
- doc: Go language plugin implementation
- signature: `class GoPlugin(LanguagePlugin):`
- members:
  - `__init__(self)` — [`L381`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/go_plugin.py#L381) — Initialize the Go language plugin.
  - `_count_tree_nodes(self, node: Any)` — [`L502`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/go_plugin.py#L502) — Recursively count nodes.
  - `analyze_file(self, file_path: str, request: AnalysisRequest)` — [`L425`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/go_plugin.py#L425) — Analyze Go code and return structured results. — documented in [tree_sitter_analyzer-core-request](../../../concepts/tree_sitter_analyzer-core-request.md)
  - `create_extractor(self)` — [`L398`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/go_plugin.py#L398) — Create a new element extractor instance.
  - `extract_elements(self, tree: Any | None, source_code: str)` — [`L543`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/go_plugin.py#L543) — Extract all elements from Go source code.
  - `get_file_extensions(self)` — [`L393`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/go_plugin.py#L393) — Get supported file extensions.
  - `get_language_name(self)` — [`L389`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/go_plugin.py#L389) — Get the language name.
  - `get_queries(self)` — [`L418`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/go_plugin.py#L418) — Get Go-specific tree-sitter queries.
  - `get_supported_element_types(self)` — [`L402`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/go_plugin.py#L402) — Get supported element types for Go.
  - `get_tree_sitter_language(self)` — [`L512`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/go_plugin.py#L512) — Get the tree-sitter language for Go.
  - `extractor` — [`L384`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/go_plugin.py#L384)
  - `language` — [`L385`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/go_plugin.py#L385)
  - `supported_extensions` — [`L386`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/go_plugin.py#L386)
- protocol/private: `_cached_language`[`L387`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/go_plugin.py#L387)
- uses (calls/refs, reference-scoped): [`AnalysisResult`](../models/result.md#AnalysisResult), [`log_error`](../utils/logging.md#log_error), [`AnalysisRequest`](../core/request.md#AnalysisRequest), [`elements`](../models/result.md#AnalysisResult.elements), [`language`](../models/result.md#AnalysisResult.language), [`LanguagePlugin`](../plugins/base.md#LanguagePlugin), [`file_path`](../models/result.md#AnalysisResult.file_path), [`success`](../models/result.md#AnalysisResult.success), [`ElementExtractor`](../plugins/base.md#ElementExtractor), [`extract_functions`](../plugins/base.md#ElementExtractor.extract_functions), [`extract_classes`](../plugins/base.md#ElementExtractor.extract_classes), [`line_count`](../models/result.md#AnalysisResult.line_count), [`extract_variables`](../plugins/base.md#ElementExtractor.extract_variables), [`error_message`](../models/result.md#AnalysisResult.error_message), [`extract_imports`](../plugins/base.md#ElementExtractor.extract_imports), [`source_code`](../models/result.md#AnalysisResult.source_code), [`read_file_safe`](../encoding_utils.md#read_file_safe), [`node_count`](../models/result.md#AnalysisResult.node_count), [`GO_QUERIES`](../queries/go.md#GO_QUERIES.GO_QUERIES), [`GoElementExtractor`](go_plugin.md#GoElementExtractor), [`extract_packages`](../plugins/base.md#ElementExtractor.extract_packages), [`channels`](go_plugin.md#GoElementExtractor.channels), [`defers`](go_plugin.md#GoElementExtractor.defers), [`goroutines`](go_plugin.md#GoElementExtractor.goroutines), [`goroutines`](../models/result.md#AnalysisResult.goroutines), [`channels`](../models/result.md#AnalysisResult.channels), [`defers`](../models/result.md#AnalysisResult.defers)
- used by: [`LanguagePlugin`](../plugins/base.md#LanguagePlugin), [`get_language_name`](../plugins/base.md#LanguagePlugin.get_language_name), [`analyze_file`](../plugins/base.md#LanguagePlugin.analyze_file), [`get_file_extensions`](../plugins/base.md#LanguagePlugin.get_file_extensions), [`create_extractor`](../plugins/base.md#LanguagePlugin.create_extractor), [`get_tree_sitter_language`](../plugins/base.md#LanguagePlugin.get_tree_sitter_language), [`get_queries`](../plugins/base.md#LanguagePlugin.get_queries), [`get_supported_element_types`](../plugins/base.md#LanguagePlugin.get_supported_element_types)  (15 test-only)

