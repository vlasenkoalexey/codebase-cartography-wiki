---
title: 'Module: tree_sitter_analyzer/languages/c_plugin.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/c_plugin.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.c_plugin`/
symbols:
  CPlugin.analyze_file: CPlugin#analyze_file().
  CElementExtractor: CElementExtractor#
  CElementExtractor.extract_functions: CElementExtractor#extract_functions().
  CElementExtractor.extract_classes: CElementExtractor#extract_classes().
  CPlugin: CPlugin#
  CElementExtractor._get_node_text_optimized: CElementExtractor#_get_node_text_optimized().
  CElementExtractor.extract_variables: CElementExtractor#extract_variables().
  CElementExtractor._extract_function_optimized: CElementExtractor#_extract_function_optimized().
  CElementExtractor._reset_caches: CElementExtractor#_reset_caches().
  CPlugin.extract_elements: CPlugin#extract_elements().
  CElementExtractor.extract_imports: CElementExtractor#extract_imports().
  CElementExtractor._extract_union_optimized: CElementExtractor#_extract_union_optimized().
  CElementExtractor._extract_struct_optimized: CElementExtractor#_extract_struct_optimized().
  CElementExtractor._traverse_and_extract_iterative: CElementExtractor#_traverse_and_extract_iterative().
  CElementExtractor.content_lines: CElementExtractor#content_lines.
  CElementExtractor._extract_enum_optimized: CElementExtractor#_extract_enum_optimized().
  CPlugin.create_extractor: CPlugin#create_extractor().
  CPlugin.get_tree_sitter_language: CPlugin#get_tree_sitter_language().
  CElementExtractor._extract_field_optimized: CElementExtractor#_extract_field_optimized().
  CElementExtractor._parse_function_signature: CElementExtractor#_parse_function_signature().
  CElementExtractor._extract_variable_declaration: CElementExtractor#_extract_variable_declaration().
  CElementExtractor._extract_macro_definition: CElementExtractor#_extract_macro_definition().
  CElementExtractor._extract_macro_function: CElementExtractor#_extract_macro_function().
  CElementExtractor._extract_include_info: CElementExtractor#_extract_include_info().
  CElementExtractor._extract_includes_fallback: CElementExtractor#_extract_includes_fallback().
  CElementExtractor.source_code: CElementExtractor#source_code.
  CElementExtractor._extract_parameters: CElementExtractor#_extract_parameters().
  CElementExtractor._extract_comment_for_line: CElementExtractor#_extract_comment_for_line().
  CElementExtractor._calculate_complexity_optimized: CElementExtractor#_calculate_complexity_optimized().
  CElementExtractor._file_encoding: CElementExtractor#_file_encoding.
  CPlugin._cached_language: CPlugin#_cached_language.
  CPlugin._count_tree_nodes: CPlugin#_count_tree_nodes().
  CElementExtractor._node_text_cache: CElementExtractor#_node_text_cache.
  CPlugin.extractor: CPlugin#extractor.
  _bind_c_parser_language: _bind_c_parser_language().
  CPlugin.supported_extensions: CPlugin#supported_extensions.
  CElementExtractor._processed_nodes: CElementExtractor#_processed_nodes.
  CElementExtractor._element_cache: CElementExtractor#_element_cache.
  CPlugin.get_file_extensions: CPlugin#get_file_extensions().
  CElementExtractor.current_file: CElementExtractor#current_file.
  _c_extract_multiline_text: _c_extract_multiline_text().
  CElementExtractor._comment_cache: CElementExtractor#_comment_cache.
  CElementExtractor._complexity_cache: CElementExtractor#_complexity_cache.
  CElementExtractor._innermost_conditional: CElementExtractor#_innermost_conditional().
  CPlugin.get_language_name: CPlugin#get_language_name().
  CElementExtractor.__init__: CElementExtractor#__init__().
  CElementExtractor.includes: CElementExtractor#includes.
  CPlugin.__init__: CPlugin#__init__().
  CPlugin.language: CPlugin#language.
---
# Module: [`tree_sitter_analyzer/languages/c_plugin.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/c_plugin.py)

## Classes
### `CElementExtractor`  ·  implements/extends ElementExtractor
- def: [`tree_sitter_analyzer/languages/c_plugin.py:90`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/c_plugin.py#L90)
- doc: C specific element extractor with advanced analysis support
- signature: `class CElementExtractor(ElementExtractor):`
- members:
  - `__init__(self)` — [`L93`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/c_plugin.py#L93) — Initialize the C element extractor.
  - `_calculate_complexity_optimized(self, node: tree_sitter.Node)` — [`L378`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/c_plugin.py#L378) — Calculate cyclomatic complexity
  - `_extract_comment_for_line(self, line: int)` — [`L383`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/c_plugin.py#L383) — Extract comment (documentation) for a specific line
  - `_extract_enum_optimized(self, node: tree_sitter.Node)` — [`L336`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/c_plugin.py#L336) — Extract enum information optimized
  - `_extract_field_optimized(self, node: tree_sitter.Node)` — [`L343`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/c_plugin.py#L343) — Extract field declaration
  - `_extract_function_optimized(self, node: tree_sitter.Node)` — [`L290`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/c_plugin.py#L290) — Extract function information optimized
  - `_extract_include_info(self, node: tree_sitter.Node, source_code: str)` — [`L353`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/c_plugin.py#L353) — Extract include directive information
  - `_extract_includes_fallback(self, source_code: str)` — [`L362`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/c_plugin.py#L362) — Fallback include extraction using regex
  - `_extract_macro_definition(self, node: tree_sitter.Node)` — [`L369`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/c_plugin.py#L369) — Extract macro definitions as constants
  - `_extract_macro_function(self, node: tree_sitter.Node)` — [`L374`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/c_plugin.py#L374) — Extract macro function definition
  - `_extract_parameters(self, params_node: tree_sitter.Node)` — [`L311`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/c_plugin.py#L311) — Extract function parameters
  - `_extract_struct_optimized(self, node: tree_sitter.Node)` — [`L316`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/c_plugin.py#L316) — Extract struct information optimized
  - `_extract_union_optimized(self, node: tree_sitter.Node)` — [`L323`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/c_plugin.py#L323) — Extract union information optimized
  - `_extract_variable_declaration(self, node: tree_sitter.Node)` — [`L348`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/c_plugin.py#L348) — Extract variable declarations (not struct members)
  - `_get_node_text_optimized(self, node: tree_sitter.Node)` — [`L253`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/c_plugin.py#L253) — Get node text with optimized caching using position-based keys
  - `_parse_function_signature(self, node: tree_sitter.Node)` — [`L302`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/c_plugin.py#L302) — Parse C function signature
  - `_reset_caches(self)` — [`L227`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/c_plugin.py#L227) — Reset performance caches
  - `_traverse_and_extract_iterative(self, root_node: tree_sitter.Node | None, extractors: dict[str, Any], results: list[Any], element_type: str)` — [`L236`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/c_plugin.py#L236) — Iterative node traversal and extraction with caching
  - `extract_classes(self, tree: tree_sitter.Tree, source_code: str)` — [`L171`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/c_plugin.py#L171) — Extract C struct/union/enum definitions as 'classes'
  - `extract_functions(self, tree: tree_sitter.Tree, source_code: str)` — [`L109`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/c_plugin.py#L109) — Extract C function definitions with comprehensive details
  - `extract_imports(self, tree: tree_sitter.Tree, source_code: str)` — [`L219`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/c_plugin.py#L219) — Extract C include directives
  - `extract_variables(self, tree: tree_sitter.Tree, source_code: str)` — [`L194`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/c_plugin.py#L194) — Extract C variable/field declarations
  - `content_lines` — [`L97`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/c_plugin.py#L97)
  - `current_file` — [`L95`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/c_plugin.py#L95)
  - `includes` — [`L98`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/c_plugin.py#L98)
  - `source_code` — [`L96`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/c_plugin.py#L96)
- protocol/private: `_comment_cache`[`L105`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/c_plugin.py#L105), `_complexity_cache`[`L106`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/c_plugin.py#L106), `_element_cache`[`L103`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/c_plugin.py#L103), `_file_encoding`[`L104`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/c_plugin.py#L104), `_innermost_conditional`[`L144`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/c_plugin.py#L144), `_node_text_cache`[`L101`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/c_plugin.py#L101), `_processed_nodes`[`L102`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/c_plugin.py#L102)
- uses (calls/refs, reference-scoped): [`name`](../models/base.md#CodeElement.name), [`start_line`](../models/base.md#CodeElement.start_line), [`log_debug`](../utils/logging.md#log_debug), [`Function`](../models/base.md#Function), [`log_error`](../utils/logging.md#log_error), [`Class`](../models/base.md#Class), [`Variable`](../models/base.md#Variable), [`Import`](../models/base.md#Import), [`ElementExtractor`](../plugins/base.md#ElementExtractor), [`return_type`](../models/base.md#Function.return_type), [`class_type`](../models/base.md#Class.class_type), [`safe_encode`](../encoding_utils.md#safe_encode), [`extract_text_slice`](../encoding_utils.md#extract_text_slice), [`full_qualified_name`](../models/base.md#Class.full_qualified_name), [`extract_macro_definition`](c_helpers.md#extract_macro_definition), [`extract_c_imports`](c_helpers.md#extract_c_imports), [`_extract_include_info`](c_helpers.md#_extract_include_info), [`_extract_includes_fallback`](c_helpers.md#_extract_includes_fallback), [`extract_c_function`](c_helpers.md#extract_c_function), [`extract_enum_definition`](c_helpers.md#extract_enum_definition), [`extract_field_declaration`](c_helpers.md#extract_field_declaration), [`extract_macro_function`](c_helpers.md#extract_macro_function), [`extract_struct_definition`](c_helpers.md#extract_struct_definition), [`extract_variable_declaration`](c_helpers.md#extract_variable_declaration), [`c_traverse_and_extract`](c_helpers.md#c_traverse_and_extract), [`calculate_complexity`](c_helpers.md#calculate_complexity), [`extract_comment_for_line`](c_helpers.md#extract_comment_for_line), [`parse_function_signature`](c_helpers.md#parse_function_signature), [`extract_parameters`](c_helpers.md#extract_parameters), [`_c_extract_multiline_text`](c_plugin.md#_c_extract_multiline_text)  (1 test-only)
- used by: [`ElementExtractor`](../plugins/base.md#ElementExtractor), [`extract_functions`](../plugins/base.md#ElementExtractor.extract_functions), [`extract_classes`](../plugins/base.md#ElementExtractor.extract_classes), [`extract_variables`](../plugins/base.md#ElementExtractor.extract_variables), [`extract_imports`](../plugins/base.md#ElementExtractor.extract_imports), [`create_extractor`](c_plugin.md#CPlugin.create_extractor), [`extractor`](c_plugin.md#CPlugin.extractor)  (39 test-only)

### `CPlugin`  ·  implements/extends LanguagePlugin
- def: [`tree_sitter_analyzer/languages/c_plugin.py:415`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/c_plugin.py#L415)
- doc: C language plugin implementation
- signature: `class CPlugin(LanguagePlugin):`
- members:
  - `__init__(self)` — [`L418`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/c_plugin.py#L418) — Initialize the C language plugin.
  - `_count_tree_nodes(self, node: Any)` — [`L514`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/c_plugin.py#L514) — Recursively count nodes in the AST tree.
  - `analyze_file(self, file_path: str, request: AnalysisRequest)` — [`L440`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/c_plugin.py#L440) — Analyze C code and return structured results. — documented in [tree_sitter_analyzer-core-request](../../../concepts/tree_sitter_analyzer-core-request.md)
  - `create_extractor(self)` — [`L435`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/c_plugin.py#L435) — Create a new element extractor instance.
  - `extract_elements(self, tree: Any | None, source_code: str)` — [`L556`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/c_plugin.py#L556) — Extract all elements from C code.
  - `get_file_extensions(self)` — [`L430`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/c_plugin.py#L430) — Get supported file extensions.
  - `get_language_name(self)` — [`L426`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/c_plugin.py#L426) — Get the language name.
  - `get_tree_sitter_language(self)` — [`L525`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/c_plugin.py#L525) — Get the tree-sitter language for C.
  - `extractor` — [`L421`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/c_plugin.py#L421)
  - `language` — [`L422`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/c_plugin.py#L422)
  - `supported_extensions` — [`L423`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/c_plugin.py#L423)
- protocol/private: `_cached_language`[`L424`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/c_plugin.py#L424)
- uses (calls/refs, reference-scoped): [`AnalysisResult`](../models/result.md#AnalysisResult), [`log_error`](../utils/logging.md#log_error), [`AnalysisRequest`](../core/request.md#AnalysisRequest), [`elements`](../models/result.md#AnalysisResult.elements), [`language`](../models/result.md#AnalysisResult.language), [`LanguagePlugin`](../plugins/base.md#LanguagePlugin), [`file_path`](../models/result.md#AnalysisResult.file_path), [`success`](../models/result.md#AnalysisResult.success), [`ElementExtractor`](../plugins/base.md#ElementExtractor), [`extract_functions`](../plugins/base.md#ElementExtractor.extract_functions), [`extract_classes`](../plugins/base.md#ElementExtractor.extract_classes), [`line_count`](../models/result.md#AnalysisResult.line_count), [`extract_variables`](../plugins/base.md#ElementExtractor.extract_variables), [`error_message`](../models/result.md#AnalysisResult.error_message), [`extract_imports`](../plugins/base.md#ElementExtractor.extract_imports), [`source_code`](../models/result.md#AnalysisResult.source_code), [`read_file_safe`](../encoding_utils.md#read_file_safe), [`node_count`](../models/result.md#AnalysisResult.node_count), [`CElementExtractor`](c_plugin.md#CElementExtractor), [`_bind_c_parser_language`](c_plugin.md#_bind_c_parser_language), [`set_file_encoding`](../plugins/base.md#ElementExtractor.set_file_encoding)
- used by: [`LanguagePlugin`](../plugins/base.md#LanguagePlugin), [`get_language_name`](../plugins/base.md#LanguagePlugin.get_language_name), [`analyze_file`](../plugins/base.md#LanguagePlugin.analyze_file), [`get_file_extensions`](../plugins/base.md#LanguagePlugin.get_file_extensions), [`create_extractor`](../plugins/base.md#LanguagePlugin.create_extractor), [`get_tree_sitter_language`](../plugins/base.md#LanguagePlugin.get_tree_sitter_language)  (20 test-only)

## Functions
- `_bind_c_parser_language(language: Any)` — [`L388`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/c_plugin.py#L388) — Create a ``tree_sitter.Parser`` bound to ``language``.
- `_c_extract_multiline_text(content_lines: list[str], start_point: tuple[int, int], end_point: tuple[int, int])` — [`L65`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/c_plugin.py#L65) — Slice multi-line node text from ``content_lines``.

