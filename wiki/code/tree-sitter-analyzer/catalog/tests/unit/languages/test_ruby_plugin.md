---
title: 'Module: tests/unit/languages/test_ruby_plugin.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_ruby_plugin.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_ruby_plugin`/
symbols:
  get_tree_for_code: get_tree_for_code().
  SIMPLE_CLASS_CODE: SIMPLE_CLASS_CODE.
  TestRubyFunctionExtraction.test_extract_splat_parameters: TestRubyFunctionExtraction#test_extract_splat_parameters().
  TestRubyIntegration.test_full_extraction_workflow: TestRubyIntegration#test_full_extraction_workflow().
  TestRubyIntegration.test_inheritance_chain: TestRubyIntegration#test_inheritance_chain().
  TestRubyMethodNameClean.test_singleton_method_name_is_bare: TestRubyMethodNameClean#test_singleton_method_name_is_bare().
  TestRubyMethodNameClean.test_attr_method_name_is_bare: TestRubyMethodNameClean#test_attr_method_name_is_bare().
  TestRubyClassExtraction.test_extract_simple_class: TestRubyClassExtraction#test_extract_simple_class().
  TestRubyClassExtraction.test_extract_class_with_inheritance: TestRubyClassExtraction#test_extract_class_with_inheritance().
  TestRubyClassExtraction.test_class_line_numbers: TestRubyClassExtraction#test_class_line_numbers().
  TestRubyFunctionExtraction.test_extract_method_parameters: TestRubyFunctionExtraction#test_extract_method_parameters().
  TestRubyVariableExtraction.test_variable_line_numbers: TestRubyVariableExtraction#test_variable_line_numbers().
  TestRubyImportExtraction.test_import_line_numbers: TestRubyImportExtraction#test_import_line_numbers().
  TestRubyPluginAnalyzeFile.test_analyze_file_with_temp_file: TestRubyPluginAnalyzeFile#test_analyze_file_with_temp_file().
  TestRubyMethodNameClean.test_instance_method_receiver_type_is_owner: TestRubyMethodNameClean#test_instance_method_receiver_type_is_owner().
  TestRubyOptionalParamExtraction.test_optional_parameter_included_with_default: TestRubyOptionalParamExtraction#test_optional_parameter_included_with_default().
  TestRubyOptionalParamExtraction.test_keyword_parameter_included_with_default: TestRubyOptionalParamExtraction#test_keyword_parameter_included_with_default().
  TestRubyClassExtraction.test_extract_module: TestRubyClassExtraction#test_extract_module().
  TestRubyClassExtraction.test_extract_multiple_classes: TestRubyClassExtraction#test_extract_multiple_classes().
  TestRubyFunctionExtraction.test_extract_instance_methods: TestRubyFunctionExtraction#test_extract_instance_methods().
  TestRubyFunctionExtraction.test_extract_singleton_methods: TestRubyFunctionExtraction#test_extract_singleton_methods().
  TestRubyFunctionExtraction.test_extract_attr_accessor: TestRubyFunctionExtraction#test_extract_attr_accessor().
  TestRubyFunctionExtraction.test_singleton_method_is_static: TestRubyFunctionExtraction#test_singleton_method_is_static().
  TestRubyVariableExtraction.test_extract_constants: TestRubyVariableExtraction#test_extract_constants().
  TestRubyVariableExtraction.test_constant_is_marked_constant: TestRubyVariableExtraction#test_constant_is_marked_constant().
  TestRubyVariableExtraction.test_extract_class_variables: TestRubyVariableExtraction#test_extract_class_variables().
  TestRubyVariableExtraction.test_scoped_constant_assignment_not_dropped: TestRubyVariableExtraction#test_scoped_constant_assignment_not_dropped().
  TestRubyImportExtraction.test_extract_require: TestRubyImportExtraction#test_extract_require().
  TestRubyImportExtraction.test_extract_require_relative: TestRubyImportExtraction#test_extract_require_relative().
  TestRubyImportExtraction.test_extract_load: TestRubyImportExtraction#test_extract_load().
  TestRubyImportExtraction.test_extract_simple_require: TestRubyImportExtraction#test_extract_simple_require().
  TestRubyExtractorHelpers.test_determine_visibility_private: TestRubyExtractorHelpers#test_determine_visibility_private().
  TestRubyExtractorHelpers.test_determine_visibility_protected: TestRubyExtractorHelpers#test_determine_visibility_protected().
  TestRubyExtractorHelpers.test_determine_visibility_restores_public: TestRubyExtractorHelpers#test_determine_visibility_restores_public().
  TestRubyIntegration.test_module_extraction: TestRubyIntegration#test_module_extraction().
  TestRubyMethodNameClean.test_instance_method_name_is_bare: TestRubyMethodNameClean#test_instance_method_name_is_bare().
  TestRubyMethodNameClean.test_user_contains_initialize: TestRubyMethodNameClean#test_user_contains_initialize().
  TestRubyExtractorHelpers.test_reset_caches: TestRubyExtractorHelpers#test_reset_caches().
  TestRubyClassExtraction.test_extract_empty_tree: TestRubyClassExtraction#test_extract_empty_tree().
  TestRubyFunctionExtraction.test_extract_functions_empty_tree: TestRubyFunctionExtraction#test_extract_functions_empty_tree().
  TestRubyVariableExtraction.test_extract_variables_empty_tree: TestRubyVariableExtraction#test_extract_variables_empty_tree().
  TestRubyImportExtraction.test_extract_imports_empty_tree: TestRubyImportExtraction#test_extract_imports_empty_tree().
  TestRubyPluginAnalyzeFile.test_analyze_file_node_count: TestRubyPluginAnalyzeFile#test_analyze_file_node_count().
  TestRubyPluginAnalyzeFile.test_analyze_file_line_count_nonzero: TestRubyPluginAnalyzeFile#test_analyze_file_line_count_nonzero().
  CONSTANTS_CODE: CONSTANTS_CODE.
  REQUIRE_STATEMENTS_CODE: REQUIRE_STATEMENTS_CODE.
  TestRubyPluginInterface.test_plugin_instantiation: TestRubyPluginInterface#test_plugin_instantiation().
  TestRubyExtractorHelpers.test_get_node_text_optimized_caching: TestRubyExtractorHelpers#test_get_node_text_optimized_caching().
  TestRubyPluginAnalyzeFile.test_analyze_file_nonexistent: TestRubyPluginAnalyzeFile#test_analyze_file_nonexistent().
  INHERITANCE_CODE: INHERITANCE_CODE.
  SINGLETON_METHODS_CODE: SINGLETON_METHODS_CODE.
  MODULE_CODE: MODULE_CODE.
  TestRubyPluginInterface.test_get_tree_sitter_language: TestRubyPluginInterface#test_get_tree_sitter_language().
  TestRubyPluginInterface.test_language_caching: TestRubyPluginInterface#test_language_caching().
  TestRubyExtractorHelpers.test_determine_visibility_default: TestRubyExtractorHelpers#test_determine_visibility_default().
  TestRubyIntegration.test_plugin_loads_successfully: TestRubyIntegration#test_plugin_loads_successfully().
  TestRubyIntegration.test_rb_file_extension_recognized: TestRubyIntegration#test_rb_file_extension_recognized().
  _OPTIONAL_PARAM_CODE: _OPTIONAL_PARAM_CODE.
  BLOCK_PARAMS_CODE: BLOCK_PARAMS_CODE.
  TestRubyPluginInterface: TestRubyPluginInterface#
  TestRubyClassExtraction: TestRubyClassExtraction#
  TestRubyFunctionExtraction: TestRubyFunctionExtraction#
  TestRubyVariableExtraction: TestRubyVariableExtraction#
  TestRubyImportExtraction: TestRubyImportExtraction#
  TestRubyExtractorHelpers: TestRubyExtractorHelpers#
  TestRubyPluginAnalyzeFile: TestRubyPluginAnalyzeFile#
  TestRubyIntegration: TestRubyIntegration#
  TestRubyMethodNameClean: TestRubyMethodNameClean#
  TestRubyOptionalParamExtraction: TestRubyOptionalParamExtraction#
---
# Module: [`tests/unit/languages/test_ruby_plugin.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py)

## Classes
### `TestRubyClassExtraction`
- def: [`tests/unit/languages/test_ruby_plugin.py:177`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L177)
- doc: Test Ruby class extraction.
- signature: `class TestRubyClassExtraction:`
- members:
  - `test_class_line_numbers(self)` — [`L227`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L227) — Test that class line numbers are correct.
  - `test_extract_class_with_inheritance(self)` — [`L203`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L203) — Test extraction of class with inheritance.
  - `test_extract_empty_tree(self)` — [`L237`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L237) — Test extraction with empty code.
  - `test_extract_module(self)` — [`L192`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L192) — Test extraction of modules.
  - `test_extract_multiple_classes(self)` — [`L215`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L215) — Test extraction of multiple classes.
  - `test_extract_simple_class(self)` — [`L180`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L180) — Test extraction of a simple class.
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`extract_classes`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor.extract_classes), [`class_type`](../../../tree_sitter_analyzer/models/base.md#Class.class_type), [`RubyPlugin`](../../../tree_sitter_analyzer/languages/ruby_plugin.md#RubyPlugin), [`create_extractor`](../../../tree_sitter_analyzer/languages/ruby_plugin.md#RubyPlugin.create_extractor), [`superclass`](../../../tree_sitter_analyzer/models/base.md#Class.superclass)  (4 test-only)

### `TestRubyExtractorHelpers`
- def: [`tests/unit/languages/test_ruby_plugin.py:478`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L478)
- doc: Test RubyElementExtractor helper methods.
- signature: `class TestRubyExtractorHelpers:`
- members:
  - `test_determine_visibility_default(self)` — [`L494`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L494) — Test default visibility determination.
  - `test_determine_visibility_private(self)` — [`L500`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L500) — Method defined after 'private' keyword should be private.
  - `test_determine_visibility_protected(self)` — [`L513`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L513) — Method defined after 'protected' keyword should be protected.
  - `test_determine_visibility_restores_public(self)` — [`L526`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L526) — Method after explicit 'public' re-declaration should be public.
  - `test_get_node_text_optimized_caching(self)` — [`L548`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L548) — Test that node text extraction uses caching.
  - `test_reset_caches(self)` — [`L481`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L481) — Test cache reset functionality.
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`extract_functions`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor.extract_functions), [`visibility`](../../../tree_sitter_analyzer/models/base.md#Function.visibility), [`RubyPlugin`](../../../tree_sitter_analyzer/languages/ruby_plugin.md#RubyPlugin), [`create_extractor`](../../../tree_sitter_analyzer/languages/ruby_plugin.md#RubyPlugin.create_extractor), [`RubyElementExtractor`](../../../tree_sitter_analyzer/languages/ruby_plugin.md#RubyElementExtractor), [`_reset_caches`](../../../tree_sitter_analyzer/languages/ruby_plugin.md#RubyElementExtractor._reset_caches), [`_node_text_cache`](../../../tree_sitter_analyzer/languages/ruby_plugin.md#RubyElementExtractor._node_text_cache), [`_determine_visibility`](../../../tree_sitter_analyzer/languages/ruby_plugin.md#RubyElementExtractor._determine_visibility), [`_processed_nodes`](../../../tree_sitter_analyzer/languages/ruby_plugin.md#RubyElementExtractor._processed_nodes), [`current_module`](../../../tree_sitter_analyzer/languages/ruby_plugin.md#RubyElementExtractor.current_module)  (1 test-only)

### `TestRubyFunctionExtraction`
- def: [`tests/unit/languages/test_ruby_plugin.py:247`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L247)
- doc: Test Ruby method extraction.
- signature: `class TestRubyFunctionExtraction:`
- members:
  - `test_extract_attr_accessor(self)` — [`L275`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L275) — Test extraction of attr_accessor methods.
  - `test_extract_functions_empty_tree(self)` — [`L320`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L320) — Test function extraction with empty code.
  - `test_extract_instance_methods(self)` — [`L250`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L250) — Test extraction of instance methods.
  - `test_extract_method_parameters(self)` — [`L286`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L286) — Test extraction of method parameters.
  - `test_extract_singleton_methods(self)` — [`L263`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L263) — Test extraction of singleton (class) methods.
  - `test_extract_splat_parameters(self)` — [`L298`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L298) — Test extraction of splat parameters.
  - `test_singleton_method_is_static(self)` — [`L309`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L309) — Test that singleton methods are marked as static.
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`extract_functions`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor.extract_functions), [`parameters`](../../../tree_sitter_analyzer/models/base.md#Function.parameters), [`RubyPlugin`](../../../tree_sitter_analyzer/languages/ruby_plugin.md#RubyPlugin), [`receiver_type`](../../../tree_sitter_analyzer/models/base.md#Function.receiver_type), [`create_extractor`](../../../tree_sitter_analyzer/languages/ruby_plugin.md#RubyPlugin.create_extractor), [`is_static`](../../../tree_sitter_analyzer/models/base.md#Function.is_static)  (4 test-only)

### `TestRubyImportExtraction`
- def: [`tests/unit/languages/test_ruby_plugin.py:413`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L413)
- doc: Test Ruby require statement extraction.
- signature: `class TestRubyImportExtraction:`
- members:
  - `test_extract_imports_empty_tree(self)` — [`L457`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L457) — Test import extraction with empty code.
  - `test_extract_load(self)` — [`L437`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L437) — Test extraction of load statements.
  - `test_extract_require(self)` — [`L416`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L416) — Test extraction of require statements.
  - `test_extract_require_relative(self)` — [`L427`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L427) — Test extraction of require_relative statements.
  - `test_extract_simple_require(self)` — [`L466`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L466) — Test extraction from simple class code.
  - `test_import_line_numbers(self)` — [`L447`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L447) — Test that import line numbers are correct.
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`extract_imports`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor.extract_imports), [`RubyPlugin`](../../../tree_sitter_analyzer/languages/ruby_plugin.md#RubyPlugin), [`create_extractor`](../../../tree_sitter_analyzer/languages/ruby_plugin.md#RubyPlugin.create_extractor)  (3 test-only)

### `TestRubyIntegration`
- def: [`tests/unit/languages/test_ruby_plugin.py:613`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L613)
- doc: Integration tests for Ruby plugin.
- signature: `class TestRubyIntegration:`
- members:
  - `test_full_extraction_workflow(self)` — [`L628`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L628) — Test complete extraction workflow.
  - `test_inheritance_chain(self)` — [`L657`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L657) — Test extraction of inheritance relationships.
  - `test_module_extraction(self)` — [`L643`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L643) — Test extraction from module code.
  - `test_plugin_loads_successfully(self)` — [`L616`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L616) — Test that Ruby plugin loads successfully.
  - `test_rb_file_extension_recognized(self)` — [`L622`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L622) — Test that .rb file extension is recognized.
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`extract_functions`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor.extract_functions), [`extract_classes`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor.extract_classes), [`extract_variables`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor.extract_variables), [`extract_imports`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor.extract_imports), [`class_type`](../../../tree_sitter_analyzer/models/base.md#Class.class_type), [`RubyPlugin`](../../../tree_sitter_analyzer/languages/ruby_plugin.md#RubyPlugin), [`create_extractor`](../../../tree_sitter_analyzer/languages/ruby_plugin.md#RubyPlugin.create_extractor), [`superclass`](../../../tree_sitter_analyzer/models/base.md#Class.superclass), [`get_language_name`](../../../tree_sitter_analyzer/languages/ruby_plugin.md#RubyPlugin.get_language_name), [`get_file_extensions`](../../../tree_sitter_analyzer/languages/ruby_plugin.md#RubyPlugin.get_file_extensions)  (4 test-only)

### `TestRubyMethodNameClean`
- def: [`tests/unit/languages/test_ruby_plugin.py:675`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L675)
- doc: Issue #535 — method name must be bare; owner in receiver_type.
- signature: `class TestRubyMethodNameClean:`
- members:
  - `test_attr_method_name_is_bare(self)` — [`L715`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L715) — Attribute methods must have bare names.
  - `test_instance_method_name_is_bare(self)` — [`L678`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L678) — Method name must NOT contain 'ClassName#' prefix.
  - `test_instance_method_receiver_type_is_owner(self)` — [`L690`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L690) — receiver_type must carry the owner class name for instance methods.
  - `test_singleton_method_name_is_bare(self)` — [`L702`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L702) — Class method name must NOT contain 'ClassName.' prefix.
  - `test_user_contains_initialize(self)` — [`L729`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L729) — Acceptance: User.methods contains initialize (bare name).
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`extract_functions`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor.extract_functions), [`RubyPlugin`](../../../tree_sitter_analyzer/languages/ruby_plugin.md#RubyPlugin), [`receiver_type`](../../../tree_sitter_analyzer/models/base.md#Function.receiver_type), [`create_extractor`](../../../tree_sitter_analyzer/languages/ruby_plugin.md#RubyPlugin.create_extractor), [`is_static`](../../../tree_sitter_analyzer/models/base.md#Function.is_static), [`is_property`](../../../tree_sitter_analyzer/models/base.md#Function.is_property)  (3 test-only)

### `TestRubyOptionalParamExtraction`
- def: [`tests/unit/languages/test_ruby_plugin.py:767`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L767)
- doc: #768: optional/keyword parameters must appear in .parameters (not silently dropped).
- signature: `class TestRubyOptionalParamExtraction:`
- members:
  - `test_keyword_parameter_included_with_default(self)` — [`L780`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L780) — mode: :strict must appear as 'mode: :strict', not be silently dropped.
  - `test_optional_parameter_included_with_default(self)` — [`L770`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L770) — permissions = [] must appear as 'permissions = []', not be silently dropped.
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`extract_functions`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor.extract_functions), [`parameters`](../../../tree_sitter_analyzer/models/base.md#Function.parameters), [`RubyPlugin`](../../../tree_sitter_analyzer/languages/ruby_plugin.md#RubyPlugin), [`create_extractor`](../../../tree_sitter_analyzer/languages/ruby_plugin.md#RubyPlugin.create_extractor)  (2 test-only)

### `TestRubyPluginAnalyzeFile`
- def: [`tests/unit/languages/test_ruby_plugin.py:565`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L565)
- doc: Test analyze_file method.
- signature: `class TestRubyPluginAnalyzeFile:`
- members:
  - `test_analyze_file_line_count_nonzero(self, tmp_path)` — [`L602`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L602) — #769: line_count must reflect actual file line count, not default 0.
  - `test_analyze_file_node_count(self, tmp_path)` — [`L591`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L591) — Test that node count is returned.
  - `test_analyze_file_nonexistent(self)` — [`L569`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L569) — Test analyzing nonexistent file.
  - `test_analyze_file_with_temp_file(self, tmp_path)` — [`L576`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L576) — Test analyzing a temporary Ruby file.
- uses (calls/refs, reference-scoped): [`elements`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.elements), [`language`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.language), [`file_path`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.file_path), [`success`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.success), [`line_count`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.line_count), [`RubyPlugin`](../../../tree_sitter_analyzer/languages/ruby_plugin.md#RubyPlugin), [`node_count`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.node_count), [`analyze_file`](../../../tree_sitter_analyzer/languages/ruby_plugin.md#RubyPlugin.analyze_file)  (1 test-only)

### `TestRubyPluginInterface`
- def: [`tests/unit/languages/test_ruby_plugin.py:154`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L154)
- doc: Test Ruby plugin interface implementation.
- signature: `class TestRubyPluginInterface:`
- members:
  - `test_get_tree_sitter_language(self)` — [`L163`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L163) — Test tree-sitter language retrieval.
  - `test_language_caching(self)` — [`L169`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L169) — Test that language is cached after first load.
  - `test_plugin_instantiation(self)` — [`L157`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L157) — Test that plugin instantiates successfully.
- uses (calls/refs, reference-scoped): [`RubyPlugin`](../../../tree_sitter_analyzer/languages/ruby_plugin.md#RubyPlugin), [`create_extractor`](../../../tree_sitter_analyzer/languages/ruby_plugin.md#RubyPlugin.create_extractor), [`RubyElementExtractor`](../../../tree_sitter_analyzer/languages/ruby_plugin.md#RubyElementExtractor), [`get_tree_sitter_language`](../../../tree_sitter_analyzer/languages/ruby_plugin.md#RubyPlugin.get_tree_sitter_language)

### `TestRubyVariableExtraction`
- def: [`tests/unit/languages/test_ruby_plugin.py:330`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L330)
- doc: Test Ruby variable/constant extraction.
- signature: `class TestRubyVariableExtraction:`
- members:
  - `test_constant_is_marked_constant(self)` — [`L345`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L345) — Test that constants are marked as constant.
  - `test_extract_class_variables(self)` — [`L356`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L356) — Test extraction of class variables.
  - `test_extract_constants(self)` — [`L333`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L333) — Test extraction of constants.
  - `test_extract_variables_empty_tree(self)` — [`L378`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L378) — Test variable extraction with empty code.
  - `test_scoped_constant_assignment_not_dropped(self)` — [`L387`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L387) — #902 Codex P2: Config::TIMEOUT = 30 must not be silently dropped.
  - `test_variable_line_numbers(self)` — [`L368`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L368) — Test that variable line numbers are correct.
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`extract_variables`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor.extract_variables), [`RubyPlugin`](../../../tree_sitter_analyzer/languages/ruby_plugin.md#RubyPlugin), [`create_extractor`](../../../tree_sitter_analyzer/languages/ruby_plugin.md#RubyPlugin.create_extractor), [`is_constant`](../../../tree_sitter_analyzer/models/base.md#Variable.is_constant)  (2 test-only)

## Functions
- `get_tree_for_code(code: str, plugin: RubyPlugin)` — [`L147`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L147) — Helper to parse Ruby code and return tree.

## Module values
- `BLOCK_PARAMS_CODE` — [`L117`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L117)
- `CONSTANTS_CODE` — [`L79`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L79)
- `INHERITANCE_CODE` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L53)
- `MODULE_CODE` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L35)
- `REQUIRE_STATEMENTS_CODE` — [`L133`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L133)
- `SIMPLE_CLASS_CODE` — [`L9`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L9)
- `SINGLETON_METHODS_CODE` — [`L98`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L98)
- `_OPTIONAL_PARAM_CODE` — [`L751`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_plugin.py#L751)

