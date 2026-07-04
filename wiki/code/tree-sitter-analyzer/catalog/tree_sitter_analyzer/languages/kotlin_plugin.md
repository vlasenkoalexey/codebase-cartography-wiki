---
title: 'Module: tree_sitter_analyzer/languages/kotlin_plugin.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/kotlin_plugin.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.kotlin_plugin`/Kotlin
symbols:
  KotlinElementExtractor: ElementExtractor#
  KotlinPlugin.analyze_file: Plugin#analyze_file().
  KotlinElementExtractor.extract_packages: ElementExtractor#extract_packages().
  KotlinElementExtractor._get_node_text: ElementExtractor#_get_node_text().
  KotlinPlugin: Plugin#
  KotlinElementExtractor.extract_classes: ElementExtractor#extract_classes().
  KotlinElementExtractor.extract_functions: ElementExtractor#extract_functions().
  KotlinElementExtractor.content_lines: ElementExtractor#content_lines.
  KotlinPlugin.extract_elements: Plugin#extract_elements().
  KotlinElementExtractor._extract_class_or_object: ElementExtractor#_extract_class_or_object().
  KotlinElementExtractor.extract_variables: ElementExtractor#extract_variables().
  KotlinElementExtractor.extract_imports: ElementExtractor#extract_imports().
  KotlinElementExtractor._extract_function: ElementExtractor#_extract_function().
  KotlinElementExtractor.current_package: ElementExtractor#current_package.
  KotlinElementExtractor._reset_caches: ElementExtractor#_reset_caches().
  KotlinElementExtractor._extract_primary_constructor: ElementExtractor#_extract_primary_constructor().
  KotlinElementExtractor._extract_property: ElementExtractor#_extract_property().
  KotlinElementExtractor._extract_import: ElementExtractor#_extract_import().
  KotlinElementExtractor._extract_package: ElementExtractor#_extract_package().
  KotlinPlugin.create_extractor: Plugin#create_extractor().
  KotlinElementExtractor._traverse_and_extract: ElementExtractor#_traverse_and_extract().
  KotlinElementExtractor.source_code: ElementExtractor#source_code.
  KotlinPlugin.get_tree_sitter_language: Plugin#get_tree_sitter_language().
  KotlinPlugin._cached_language: Plugin#_cached_language.
  KotlinElementExtractor._extract_class: ElementExtractor#_extract_class().
  KotlinElementExtractor._extract_object: ElementExtractor#_extract_object().
  KotlinElementExtractor._node_text_cache: ElementExtractor#_node_text_cache.
  KotlinPlugin._count_tree_nodes: Plugin#_count_tree_nodes().
  KotlinElementExtractor._kotlin_package_name_from_header: ElementExtractor#_kotlin_package_name_from_header().
  KotlinPlugin.extractor: Plugin#extractor.
  KotlinPlugin.supported_extensions: Plugin#supported_extensions.
  KotlinElementExtractor.current_file: ElementExtractor#current_file.
  KotlinElementExtractor._find_package_header_node: ElementExtractor#_find_package_header_node().
  KotlinPlugin.get_file_extensions: Plugin#get_file_extensions().
  KotlinElementExtractor.__init__: ElementExtractor#__init__().
  KotlinElementExtractor._extract_docstring: ElementExtractor#_extract_docstring().
  KotlinPlugin.__init__: Plugin#__init__().
  KotlinPlugin.language: Plugin#language.
  KotlinPlugin.get_language_name: Plugin#get_language_name().
---
# Module: [`tree_sitter_analyzer/languages/kotlin_plugin.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/kotlin_plugin.py)

## Classes
### `KotlinElementExtractor`  ·  implements/extends ElementExtractor
- def: [`tree_sitter_analyzer/languages/kotlin_plugin.py:39`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/kotlin_plugin.py#L39)
- doc: Kotlin-specific element extractor
- signature: `class KotlinElementExtractor(ElementExtractor):`
- members:
  - `__init__(self)` — [`L42`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/kotlin_plugin.py#L42) — Initialize the Kotlin element extractor.
  - `_extract_class(self, node: tree_sitter.Node)` — [`L254`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/kotlin_plugin.py#L254) — Extract class declaration
  - `_extract_class_or_object(self, node: tree_sitter.Node, kind: str)` — [`L262`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/kotlin_plugin.py#L262) — Generic extraction for class/object/interface
  - `_extract_docstring(self, node: tree_sitter.Node)` — [`L306`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/kotlin_plugin.py#L306) — Extract KDoc
  - `_extract_function(self, node: tree_sitter.Node)` — [`L244`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/kotlin_plugin.py#L244) — Extract function information
  - `_extract_import(self, node: tree_sitter.Node)` — [`L285`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/kotlin_plugin.py#L285) — Extract import header
  - `_extract_object(self, node: tree_sitter.Node)` — [`L258`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/kotlin_plugin.py#L258) — Extract object declaration
  - `_extract_package(self, node: tree_sitter.Node)` — [`L214`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/kotlin_plugin.py#L214) — Extract package declaration.
  - `_extract_primary_constructor(self, node: tree_sitter.Node)` — [`L248`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/kotlin_plugin.py#L248) — Extract primary_constructor as Function(is_constructor=True).
  - `_extract_property(self, node: tree_sitter.Node)` — [`L270`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/kotlin_plugin.py#L270) — Extract property declaration.
  - `_find_package_header_node(root_node: tree_sitter.Node)` — [`L177`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/kotlin_plugin.py#L177) — Return the first ``package_header`` child or ``None``.
  - `_get_node_text(self, node: tree_sitter.Node)` — [`L289`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/kotlin_plugin.py#L289) — Get node text with caching using position-based keys
  - `_kotlin_package_name_from_header(self, package_header: tree_sitter.Node)` — [`L228`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/kotlin_plugin.py#L228) — Return the package name string from a ``package_header`` node.
  - `_reset_caches(self)` — [`L191`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/kotlin_plugin.py#L191) — Reset performance caches
  - `_traverse_and_extract(self, node: tree_sitter.Node, extractors: dict[str, Any], results: list[Any])` — [`L199`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/kotlin_plugin.py#L199) — Recursive traversal to find and extract elements
  - `extract_classes(self, tree: tree_sitter.Tree, source_code: str)` — [`L74`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/kotlin_plugin.py#L74) — Extract Kotlin class declarations
  - `extract_functions(self, tree: tree_sitter.Tree, source_code: str)` — [`L50`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/kotlin_plugin.py#L50) — Extract Kotlin function declarations
  - `extract_imports(self, tree: tree_sitter.Tree, source_code: str)` — [`L122`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/kotlin_plugin.py#L122) — Extract Kotlin imports
  - `extract_packages(self, tree: tree_sitter.Tree, source_code: str)` — [`L148`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/kotlin_plugin.py#L148) — Extract Kotlin package
  - `extract_variables(self, tree: tree_sitter.Tree, source_code: str)` — [`L99`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/kotlin_plugin.py#L99) — Extract Kotlin properties
  - `content_lines` — [`L47`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/kotlin_plugin.py#L47)
  - `current_file` — [`L45`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/kotlin_plugin.py#L45)
  - `current_package` — [`L44`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/kotlin_plugin.py#L44)
  - `source_code` — [`L46`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/kotlin_plugin.py#L46)
- protocol/private: `_node_text_cache`[`L48`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/kotlin_plugin.py#L48)
- uses (calls/refs, reference-scoped): [`name`](../models/base.md#CodeElement.name), [`start_line`](../models/base.md#CodeElement.start_line), [`end_line`](../models/base.md#CodeElement.end_line), [`log_debug`](../utils/logging.md#log_debug), [`language`](../models/base.md#CodeElement.language), [`Function`](../models/base.md#Function), [`raw_text`](../models/base.md#CodeElement.raw_text), [`Class`](../models/base.md#Class), [`Variable`](../models/base.md#Variable), [`Import`](../models/base.md#Import), [`ElementExtractor`](../plugins/base.md#ElementExtractor), [`extract_kotlin_function`](kotlin_helpers.md#extract_kotlin_function), [`Package`](../models/base.md#Package), [`safe_encode`](../encoding_utils.md#safe_encode), [`extract_kotlin_property`](kotlin_helpers.md#extract_kotlin_property), [`extract_kotlin_primary_constructor`](kotlin_helpers.md#extract_kotlin_primary_constructor), [`extract_text_slice`](../encoding_utils.md#extract_text_slice), [`extract_kotlin_class_or_object`](kotlin_helpers.md#extract_kotlin_class_or_object), [`extract_import`](kotlin_helpers.md#extract_import)
- used by: [`ElementExtractor`](../plugins/base.md#ElementExtractor), [`extract_functions`](../plugins/base.md#ElementExtractor.extract_functions), [`extract_classes`](../plugins/base.md#ElementExtractor.extract_classes), [`extract_variables`](../plugins/base.md#ElementExtractor.extract_variables), [`extract_imports`](../plugins/base.md#ElementExtractor.extract_imports), [`extract_packages`](../plugins/base.md#ElementExtractor.extract_packages), [`create_extractor`](kotlin_plugin.md#KotlinPlugin.create_extractor), [`extractor`](kotlin_plugin.md#KotlinPlugin.extractor)  (50 test-only)

### `KotlinPlugin`  ·  implements/extends LanguagePlugin
- def: [`tree_sitter_analyzer/languages/kotlin_plugin.py:312`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/kotlin_plugin.py#L312)
- doc: Kotlin language plugin implementation
- signature: `class KotlinPlugin(LanguagePlugin):`
- members:
  - `__init__(self)` — [`L315`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/kotlin_plugin.py#L315) — Initialize the Kotlin language plugin.
  - `_count_tree_nodes(self, node: Any)` — [`L405`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/kotlin_plugin.py#L405) — Recursively count nodes.
  - `analyze_file(self, file_path: str, request: AnalysisRequest)` — [`L335`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/kotlin_plugin.py#L335) — documented in [tree_sitter_analyzer-models-result](../../../concepts/tree_sitter_analyzer-models-result.md)
  - `create_extractor(self)` — [`L331`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/kotlin_plugin.py#L331) — Create a new element extractor instance.
  - `extract_elements(self, tree: Any | None, source_code: str)` — [`L445`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/kotlin_plugin.py#L445) — Extract all elements.
  - `get_file_extensions(self)` — [`L327`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/kotlin_plugin.py#L327) — Get supported file extensions.
  - `get_language_name(self)` — [`L323`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/kotlin_plugin.py#L323) — Get the language name.
  - `get_tree_sitter_language(self)` — [`L415`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/kotlin_plugin.py#L415) — Get the tree-sitter language for Kotlin.
  - `extractor` — [`L318`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/kotlin_plugin.py#L318)
  - `language` — [`L319`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/kotlin_plugin.py#L319)
  - `supported_extensions` — [`L320`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/kotlin_plugin.py#L320)
- protocol/private: `_cached_language`[`L321`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/kotlin_plugin.py#L321)
- uses (calls/refs, reference-scoped): [`AnalysisResult`](../models/result.md#AnalysisResult), [`log_error`](../utils/logging.md#log_error), [`AnalysisRequest`](../core/request.md#AnalysisRequest), [`elements`](../models/result.md#AnalysisResult.elements), [`language`](../models/result.md#AnalysisResult.language), [`LanguagePlugin`](../plugins/base.md#LanguagePlugin), [`file_path`](../models/result.md#AnalysisResult.file_path), [`success`](../models/result.md#AnalysisResult.success), [`ElementExtractor`](../plugins/base.md#ElementExtractor), [`extract_functions`](../plugins/base.md#ElementExtractor.extract_functions), [`extract_classes`](../plugins/base.md#ElementExtractor.extract_classes), [`line_count`](../models/result.md#AnalysisResult.line_count), [`extract_variables`](../plugins/base.md#ElementExtractor.extract_variables), [`error_message`](../models/result.md#AnalysisResult.error_message), [`extract_imports`](../plugins/base.md#ElementExtractor.extract_imports), [`source_code`](../models/result.md#AnalysisResult.source_code), [`KotlinElementExtractor`](kotlin_plugin.md#KotlinElementExtractor), [`read_file_safe`](../encoding_utils.md#read_file_safe), [`node_count`](../models/result.md#AnalysisResult.node_count), [`extract_packages`](../plugins/base.md#ElementExtractor.extract_packages), [`package`](../models/result.md#AnalysisResult.package)
- used by: [`LanguagePlugin`](../plugins/base.md#LanguagePlugin), [`get_language_name`](../plugins/base.md#LanguagePlugin.get_language_name), [`analyze_file`](../plugins/base.md#LanguagePlugin.analyze_file), [`get_file_extensions`](../plugins/base.md#LanguagePlugin.get_file_extensions), [`create_extractor`](../plugins/base.md#LanguagePlugin.create_extractor), [`get_tree_sitter_language`](../plugins/base.md#LanguagePlugin.get_tree_sitter_language)  (22 test-only)

