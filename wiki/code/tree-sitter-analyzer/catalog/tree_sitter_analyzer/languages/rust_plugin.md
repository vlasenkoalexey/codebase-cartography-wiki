---
title: 'Module: tree_sitter_analyzer/languages/rust_plugin.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/rust_plugin.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.rust_plugin`/
symbols:
  RustPlugin.analyze_file: RustPlugin#analyze_file().
  RustElementExtractor: RustElementExtractor#
  RustElementExtractor._extract_function: RustElementExtractor#_extract_function().
  RustElementExtractor._get_node_text: RustElementExtractor#_get_node_text().
  RustElementExtractor._extract_function_signature: RustElementExtractor#_extract_function_signature().
  RustElementExtractor._extract_type_def: RustElementExtractor#_extract_type_def().
  RustElementExtractor._extract_field: RustElementExtractor#_extract_field().
  RustPlugin: RustPlugin#
  RustElementExtractor.extract_classes: RustElementExtractor#extract_classes().
  RustElementExtractor._extract_enum_variants: RustElementExtractor#_extract_enum_variants().
  RustElementExtractor.extract_functions: RustElementExtractor#extract_functions().
  RustElementExtractor.extract_variables: RustElementExtractor#extract_variables().
  RustElementExtractor._extract_import: RustElementExtractor#_extract_import().
  RustElementExtractor._extract_mod_package: RustElementExtractor#_extract_mod_package().
  RustElementExtractor.extract_packages: RustElementExtractor#extract_packages().
  RustPlugin.extract_elements: RustPlugin#extract_elements().
  RustElementExtractor.extract_imports: RustElementExtractor#extract_imports().
  RustElementExtractor._reset_caches: RustElementExtractor#_reset_caches().
  RustElementExtractor._extract_module: RustElementExtractor#_extract_module().
  RustElementExtractor._collect_enum_variants: RustElementExtractor#_collect_enum_variants().
  RustElementExtractor._collect_struct_fields: RustElementExtractor#_collect_struct_fields().
  RustElementExtractor._extract_impl: RustElementExtractor#_extract_impl().
  RustElementExtractor._extract_visibility: RustElementExtractor#_extract_visibility().
  RustElementExtractor.source_code: RustElementExtractor#source_code.
  RustPlugin.create_extractor: RustPlugin#create_extractor().
  RustElementExtractor._traverse_and_extract: RustElementExtractor#_traverse_and_extract().
  RustElementExtractor._extract_modules: RustElementExtractor#_extract_modules().
  RustElementExtractor._extract_struct: RustElementExtractor#_extract_struct().
  RustElementExtractor._find_self_parameter: RustElementExtractor#_find_self_parameter().
  RustElementExtractor._content_bytes: RustElementExtractor#_content_bytes.
  RustElementExtractor.content_lines: RustElementExtractor#content_lines.
  RustElementExtractor._extract_enum: RustElementExtractor#_extract_enum().
  RustElementExtractor._extract_trait: RustElementExtractor#_extract_trait().
  RustPlugin.get_tree_sitter_language: RustPlugin#get_tree_sitter_language().
  RustPlugin._cached_language: RustPlugin#_cached_language.
  RustElementExtractor._extract_rust_parameters: RustElementExtractor#_extract_rust_parameters().
  RustElementExtractor._extract_docstring: RustElementExtractor#_extract_docstring().
  RustPlugin._count_tree_nodes: RustPlugin#_count_tree_nodes().
  RustElementExtractor._node_text_cache: RustElementExtractor#_node_text_cache.
  RustElementExtractor.impl_blocks: RustElementExtractor#impl_blocks.
  _rust_calculate_complexity: _rust_calculate_complexity().
  RustElementExtractor._find_impl_owner: RustElementExtractor#_find_impl_owner().
  RustElementExtractor._extract_derives: RustElementExtractor#_extract_derives().
  RustElementExtractor.modules: RustElementExtractor#modules.
  RustElementExtractor._inside_trait: RustElementExtractor#_inside_trait().
  RustPlugin.extractor: RustPlugin#extractor.
  RustPlugin.supported_extensions: RustPlugin#supported_extensions.
  _rust_function_is_async: _rust_function_is_async().
  RustPlugin.get_file_extensions: RustPlugin#get_file_extensions().
  _RUST_DECISION_NODE_TYPES._RUST_DECISION_NODE_TYPES: _RUST_DECISION_NODE_TYPES._RUST_DECISION_NODE_TYPES.
  RustElementExtractor.__init__: RustElementExtractor#__init__().
  RustElementExtractor.current_module: RustElementExtractor#current_module.
  RustElementExtractor.current_file: RustElementExtractor#current_file.
  RustPlugin.__init__: RustPlugin#__init__().
  RustPlugin.language: RustPlugin#language.
  RustPlugin.get_language_name: RustPlugin#get_language_name().
---
# Module: [`tree_sitter_analyzer/languages/rust_plugin.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/rust_plugin.py)

## Classes
### `RustElementExtractor`  ·  implements/extends ElementExtractor
- def: [`tree_sitter_analyzer/languages/rust_plugin.py:74`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/rust_plugin.py#L74) — documented in [tree_sitter_analyzer-plugins-base](../../../concepts/tree_sitter_analyzer-plugins-base.md)
- doc: Rust-specific element extractor
- signature: `class RustElementExtractor(ElementExtractor):`
- members:
  - `__init__(self)` — [`L77`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/rust_plugin.py#L77) — Initialize the Rust element extractor.
  - `_collect_enum_variants(self, node: tree_sitter.Node, results: list[Variable])` — [`L181`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/rust_plugin.py#L181) — Walk the AST and extract enum variants from every ``enum_item``.
  - `_collect_struct_fields(self, node: tree_sitter.Node, results: list[Variable])` — [`L201`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/rust_plugin.py#L201) — Walk the AST for real struct fields, skipping enum variant bodies.
  - `_extract_derives(self, node: tree_sitter.Node)` — [`L802`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/rust_plugin.py#L802) — Extract derived traits from attributes.
  - `_extract_docstring(self, node: tree_sitter.Node)` — [`L767`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/rust_plugin.py#L767) — Extract doc comments (/// or /** ... */)
  - `_extract_enum(self, node: tree_sitter.Node)` — [`L574`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/rust_plugin.py#L574) — Extract enum information
  - `_extract_enum_variants(self, node: tree_sitter.Node)` — [`L677`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/rust_plugin.py#L677) — Extract each enum variant from an ``enum_item`` node as a Variable.
  - `_extract_field(self, node: tree_sitter.Node)` — [`L645`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/rust_plugin.py#L645) — Extract struct field
  - `_extract_function(self, node: tree_sitter.Node)` — [`L375`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/rust_plugin.py#L375) — Extract function information — documented in [tree_sitter_analyzer-models-base](../../../concepts/tree_sitter_analyzer-models-base.md)
  - `_extract_function_signature(self, node: tree_sitter.Node)` — [`L512`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/rust_plugin.py#L512) — Extract a trait abstract method (``function_signature_item``).
  - `_extract_impl(self, node: tree_sitter.Node)` — [`L620`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/rust_plugin.py#L620) — Extract impl block information
  - `_extract_import(self, node: tree_sitter.Node)` — [`L278`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/rust_plugin.py#L278) — Extract import statement (use declaration)
  - `_extract_mod_package(self, node: tree_sitter.Node)` — [`L261`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/rust_plugin.py#L261) — Build a Package element from a ``mod_item`` node.
  - `_extract_module(self, node: tree_sitter.Node)` — [`L352`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/rust_plugin.py#L352) — Extract single module
  - `_extract_modules(self, node: tree_sitter.Node)` — [`L344`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/rust_plugin.py#L344) — Extract module information
  - `_extract_rust_parameters(self, params_node: tree_sitter.Node | None)` — [`L736`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/rust_plugin.py#L736) — Return parameter texts from a Rust function ``parameters`` node.
  - `_extract_struct(self, node: tree_sitter.Node)` — [`L570`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/rust_plugin.py#L570) — Extract struct information
  - `_extract_trait(self, node: tree_sitter.Node)` — [`L578`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/rust_plugin.py#L578) — Extract trait information
  - `_extract_type_def(self, node: tree_sitter.Node, type_name: str)` — [`L582`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/rust_plugin.py#L582) — Generic type definition extractor
  - `_extract_visibility(self, node: tree_sitter.Node)` — [`L760`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/rust_plugin.py#L760) — Extract visibility modifier
  - `_find_impl_owner(self, node: tree_sitter.Node)` — [`L467`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/rust_plugin.py#L467) — Return the impl target type name for a fn nested in an impl block.
  - `_find_self_parameter(self, node: tree_sitter.Node)` — [`L493`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/rust_plugin.py#L493) — Return the self-parameter text (``&self`` / ``&mut self`` / ...).
  - `_get_node_text(self, node: tree_sitter.Node)` — [`L822`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/rust_plugin.py#L822) — Get node text with caching using position-based keys
  - `_inside_trait(self, node: tree_sitter.Node)` — [`L449`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/rust_plugin.py#L449) — True when *node* sits inside a ``trait_item`` body.
  - `_reset_caches(self)` — [`L303`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/rust_plugin.py#L303) — Reset performance caches
  - `_traverse_and_extract(self, node: tree_sitter.Node, extractors: dict[str, Any], results: list[Any])` — [`L315`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/rust_plugin.py#L315) — Recursive traversal to find and extract elements.
  - `extract_classes(self, tree: tree_sitter.Tree, source_code: str)` — [`L112`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/rust_plugin.py#L112) — Extract Rust struct, enum, trait, and impl definitions
  - `extract_functions(self, tree: tree_sitter.Tree, source_code: str)` — [`L88`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/rust_plugin.py#L88) — Extract Rust function declarations
  - `extract_imports(self, tree: tree_sitter.Tree, source_code: str)` — [`L215`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/rust_plugin.py#L215) — Extract Rust use declarations
  - `extract_packages(self, tree: tree_sitter.Tree, source_code: str)` — [`L237`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/rust_plugin.py#L237) — Extract Rust ``mod`` blocks as Package containers (issue #589).
  - `extract_variables(self, tree: tree_sitter.Tree, source_code: str)` — [`L146`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/rust_plugin.py#L146) — Extract Rust struct fields and enum variants.
  - `content_lines` — [`L82`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/rust_plugin.py#L82)
  - `current_file` — [`L80`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/rust_plugin.py#L80)
  - `current_module` — [`L79`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/rust_plugin.py#L79)
  - `impl_blocks` — [`L85`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/rust_plugin.py#L85)
  - `modules` — [`L86`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/rust_plugin.py#L86)
  - `source_code` — [`L81`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/rust_plugin.py#L81)
- protocol/private: `_content_bytes`[`L84`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/rust_plugin.py#L84), `_node_text_cache`[`L83`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/rust_plugin.py#L83)
- uses (calls/refs, reference-scoped): [`name`](../models/base.md#CodeElement.name), [`start_line`](../models/base.md#CodeElement.start_line), [`end_line`](../models/base.md#CodeElement.end_line), [`log_debug`](../utils/logging.md#log_debug), [`language`](../models/base.md#CodeElement.language), [`Function`](../models/base.md#Function), [`raw_text`](../models/base.md#CodeElement.raw_text), [`log_error`](../utils/logging.md#log_error), [`Class`](../models/base.md#Class), [`Variable`](../models/base.md#Variable), [`Import`](../models/base.md#Import), [`ElementExtractor`](../plugins/base.md#ElementExtractor), [`complexity_score`](../models/base.md#Function.complexity_score), [`parameters`](../models/base.md#Function.parameters), [`return_type`](../models/base.md#Function.return_type), [`class_type`](../models/base.md#Class.class_type), [`visibility`](../models/base.md#Function.visibility), [`receiver_type`](../models/base.md#Function.receiver_type), [`Package`](../models/base.md#Package), [`docstring`](../models/base.md#CodeElement.docstring), [`variable_type`](../models/base.md#Variable.variable_type), [`safe_encode`](../encoding_utils.md#safe_encode), [`is_method`](../models/base.md#Function.is_method), [`extract_text_slice`](../encoding_utils.md#extract_text_slice), [`is_async`](../models/base.md#Function.is_async), [`visibility`](../models/base.md#Variable.visibility), [`visibility`](../models/base.md#Class.visibility), [`is_abstract`](../models/base.md#Function.is_abstract), [`receiver`](../models/base.md#Function.receiver), [`import_statement`](../models/base.md#Import.import_statement), [`receiver_type`](../models/base.md#Variable.receiver_type), [`implements_interfaces`](../models/base.md#Class.implements_interfaces), [`_rust_calculate_complexity`](rust_plugin.md#_rust_calculate_complexity), [`_rust_function_is_async`](rust_plugin.md#_rust_function_is_async)
- used by: [`ElementExtractor`](../plugins/base.md#ElementExtractor), [`extract_functions`](../plugins/base.md#ElementExtractor.extract_functions), [`extract_classes`](../plugins/base.md#ElementExtractor.extract_classes), [`extract_variables`](../plugins/base.md#ElementExtractor.extract_variables), [`extract_imports`](../plugins/base.md#ElementExtractor.extract_imports), [`analyze_file`](rust_plugin.md#RustPlugin.analyze_file), [`extract_packages`](../plugins/base.md#ElementExtractor.extract_packages), [`create_extractor`](rust_plugin.md#RustPlugin.create_extractor), [`extractor`](rust_plugin.md#RustPlugin.extractor)  (39 test-only)

### `RustPlugin`  ·  implements/extends LanguagePlugin
- def: [`tree_sitter_analyzer/languages/rust_plugin.py:849`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/rust_plugin.py#L849) — documented in [tree_sitter_analyzer-plugins-manager](../../../concepts/tree_sitter_analyzer-plugins-manager.md)
- doc: Rust language plugin implementation
- signature: `class RustPlugin(LanguagePlugin):`
- members:
  - `__init__(self)` — [`L852`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/rust_plugin.py#L852) — Initialize the Rust language plugin.
  - `_count_tree_nodes(self, node: Any)` — [`L949`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/rust_plugin.py#L949) — Recursively count nodes.
  - `analyze_file(self, file_path: str, request: AnalysisRequest)` — [`L872`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/rust_plugin.py#L872) — Analyze Rust code and return structured results. — documented in [tree_sitter_analyzer-core-request](../../../concepts/tree_sitter_analyzer-core-request.md)
  - `create_extractor(self)` — [`L868`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/rust_plugin.py#L868) — Create a new element extractor instance.
  - `extract_elements(self, tree: Any | None, source_code: str)` — [`L989`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/rust_plugin.py#L989) — Extract all elements.
  - `get_file_extensions(self)` — [`L864`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/rust_plugin.py#L864) — Get supported file extensions.
  - `get_language_name(self)` — [`L860`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/rust_plugin.py#L860) — Get the language name.
  - `get_tree_sitter_language(self)` — [`L959`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/rust_plugin.py#L959) — Get the tree-sitter language for Rust.
  - `extractor` — [`L855`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/rust_plugin.py#L855)
  - `language` — [`L856`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/rust_plugin.py#L856)
  - `supported_extensions` — [`L857`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/rust_plugin.py#L857)
- protocol/private: `_cached_language`[`L858`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/rust_plugin.py#L858)
- uses (calls/refs, reference-scoped): [`AnalysisResult`](../models/result.md#AnalysisResult), [`log_error`](../utils/logging.md#log_error), [`AnalysisRequest`](../core/request.md#AnalysisRequest), [`elements`](../models/result.md#AnalysisResult.elements), [`language`](../models/result.md#AnalysisResult.language), [`LanguagePlugin`](../plugins/base.md#LanguagePlugin), [`file_path`](../models/result.md#AnalysisResult.file_path), [`success`](../models/result.md#AnalysisResult.success), [`ElementExtractor`](../plugins/base.md#ElementExtractor), [`extract_functions`](../plugins/base.md#ElementExtractor.extract_functions), [`extract_classes`](../plugins/base.md#ElementExtractor.extract_classes), [`line_count`](../models/result.md#AnalysisResult.line_count), [`extract_variables`](../plugins/base.md#ElementExtractor.extract_variables), [`error_message`](../models/result.md#AnalysisResult.error_message), [`extract_imports`](../plugins/base.md#ElementExtractor.extract_imports), [`RustElementExtractor`](rust_plugin.md#RustElementExtractor), [`source_code`](../models/result.md#AnalysisResult.source_code), [`read_file_safe`](../encoding_utils.md#read_file_safe), [`node_count`](../models/result.md#AnalysisResult.node_count), [`extract_packages`](../plugins/base.md#ElementExtractor.extract_packages), [`impl_blocks`](rust_plugin.md#RustElementExtractor.impl_blocks), [`modules`](rust_plugin.md#RustElementExtractor.modules), [`modules`](../models/result.md#AnalysisResult.modules), [`impls`](../models/result.md#AnalysisResult.impls)
- used by: [`LanguagePlugin`](../plugins/base.md#LanguagePlugin), [`get_language_name`](../plugins/base.md#LanguagePlugin.get_language_name), [`analyze_file`](../plugins/base.md#LanguagePlugin.analyze_file), [`get_file_extensions`](../plugins/base.md#LanguagePlugin.get_file_extensions), [`create_extractor`](../plugins/base.md#LanguagePlugin.create_extractor), [`get_tree_sitter_language`](../plugins/base.md#LanguagePlugin.get_tree_sitter_language)  (23 test-only)

## Functions
- `_rust_calculate_complexity(node: Any)` — [`L40`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/rust_plugin.py#L40) — Return cyclomatic complexity (1 + decision points) for a Rust fn node.
- `_rust_function_is_async(node: tree_sitter.Node)` — [`L56`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/rust_plugin.py#L56) — Return ``True`` when ``node`` carries an ``async`` modifier.

## Module values
- `_RUST_DECISION_NODE_TYPES` — [`L27`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/rust_plugin.py#L27)

