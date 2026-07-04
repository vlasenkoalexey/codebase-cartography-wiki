---
title: 'Module: tests/unit/languages/test_typescript_plugin_edge_cases.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_typescript_plugin_edge_cases.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_typescript_plugin_edge_cases`/TestTypeScript
symbols:
  TestTypeScriptPluginEdgeCases.test_analyze_file_encoding_error: PluginEdgeCases#test_analyze_file_encoding_error().
  TestTypeScriptPluginEdgeCases.test_analyze_file_permission_error: PluginEdgeCases#test_analyze_file_permission_error().
  TestTypeScriptPluginEdgeCases.test_analyze_file_parser_creation_error: PluginEdgeCases#test_analyze_file_parser_creation_error().
  TestTypeScriptElementExtractorEdgeCases.extractor: ElementExtractorEdgeCases#extractor().
  TestTypeScriptPluginEdgeCases.plugin: PluginEdgeCases#plugin().
  TestTypeScriptElementExtractorEdgeCases: ElementExtractorEdgeCases#
  TestTypeScriptElementExtractorEdgeCases.test_extract_function_optimized_error_handling: ElementExtractorEdgeCases#test_extract_function_optimized_error_handling().
  TestTypeScriptElementExtractorEdgeCases.test_extract_function_optimized_exception: ElementExtractorEdgeCases#test_extract_function_optimized_exception().
  TestTypeScriptElementExtractorEdgeCases.test_extract_arrow_function_optimized_with_parent: ElementExtractorEdgeCases#test_extract_arrow_function_optimized_with_parent().
  TestTypeScriptElementExtractorEdgeCases.test_extract_arrow_function_optimized_single_param: ElementExtractorEdgeCases#test_extract_arrow_function_optimized_single_param().
  TestTypeScriptElementExtractorEdgeCases.test_extract_arrow_function_optimized_with_type_annotation: ElementExtractorEdgeCases#test_extract_arrow_function_optimized_with_type_annotation().
  TestTypeScriptElementExtractorEdgeCases.test_extract_method_optimized_error_handling: ElementExtractorEdgeCases#test_extract_method_optimized_error_handling().
  TestTypeScriptElementExtractorEdgeCases.test_extract_class_optimized_no_name: ElementExtractorEdgeCases#test_extract_class_optimized_no_name().
  TestTypeScriptElementExtractorEdgeCases.test_extract_class_optimized_with_heritage: ElementExtractorEdgeCases#test_extract_class_optimized_with_heritage().
  TestTypeScriptElementExtractorEdgeCases.test_extract_interface_optimized_with_extends: ElementExtractorEdgeCases#test_extract_interface_optimized_with_extends().
  TestTypeScriptElementExtractorEdgeCases.test_extract_enum_optimized_no_name: ElementExtractorEdgeCases#test_extract_enum_optimized_no_name().
  TestTypeScriptElementExtractorEdgeCases.test_extract_property_optimized_with_modifiers: ElementExtractorEdgeCases#test_extract_property_optimized_with_modifiers().
  TestTypeScriptElementExtractorEdgeCases.test_extract_property_signature_optimized_optional: ElementExtractorEdgeCases#test_extract_property_signature_optimized_optional().
  TestTypeScriptElementExtractorEdgeCases.test_parse_variable_declarator_with_arrow_function: ElementExtractorEdgeCases#test_parse_variable_declarator_with_arrow_function().
  TestTypeScriptElementExtractorEdgeCases.test_parse_variable_declarator_with_assignment: ElementExtractorEdgeCases#test_parse_variable_declarator_with_assignment().
  TestTypeScriptElementExtractorEdgeCases.test_parse_function_signature_optimized_no_name: ElementExtractorEdgeCases#test_parse_function_signature_optimized_no_name().
  TestTypeScriptElementExtractorEdgeCases.test_parse_method_signature_optimized_no_name: ElementExtractorEdgeCases#test_parse_method_signature_optimized_no_name().
  TestTypeScriptElementExtractorEdgeCases.test_extract_import_info_simple_no_source: ElementExtractorEdgeCases#test_extract_import_info_simple_no_source().
  TestTypeScriptElementExtractorEdgeCases.test_extract_import_info_simple_error_handling: ElementExtractorEdgeCases#test_extract_import_info_simple_error_handling().
  TestTypeScriptElementExtractorEdgeCases.test_extract_dynamic_import_no_call_expression: ElementExtractorEdgeCases#test_extract_dynamic_import_no_call_expression().
  TestTypeScriptElementExtractorEdgeCases.test_extract_dynamic_import_no_import_identifier: ElementExtractorEdgeCases#test_extract_dynamic_import_no_import_identifier().
  TestTypeScriptElementExtractorEdgeCases.test_extract_dynamic_import_error_handling: ElementExtractorEdgeCases#test_extract_dynamic_import_error_handling().
  TestTypeScriptElementExtractorEdgeCases.test_extract_commonjs_requires_error_handling: ElementExtractorEdgeCases#test_extract_commonjs_requires_error_handling().
  TestTypeScriptElementExtractorEdgeCases.test_extract_tsdoc_for_line_error_handling: ElementExtractorEdgeCases#test_extract_tsdoc_for_line_error_handling().
  TestTypeScriptElementExtractorEdgeCases.test_calculate_complexity_optimized_error_handling: ElementExtractorEdgeCases#test_calculate_complexity_optimized_error_handling().
  TestTypeScriptElementExtractorEdgeCases.test_extract_variables_from_declaration_error_handling: ElementExtractorEdgeCases#test_extract_variables_from_declaration_error_handling().
  TestTypeScriptElementExtractorEdgeCases.test_extract_variable_optimized_delegation: ElementExtractorEdgeCases#test_extract_variable_optimized_delegation().
  TestTypeScriptElementExtractorEdgeCases.test_extract_lexical_variable_optimized_let: ElementExtractorEdgeCases#test_extract_lexical_variable_optimized_let().
  TestTypeScriptElementExtractorEdgeCases.test_extract_lexical_variable_optimized_const: ElementExtractorEdgeCases#test_extract_lexical_variable_optimized_const().
  TestTypeScriptPluginEdgeCases: PluginEdgeCases#
  TestTypeScriptPluginEdgeCases.test_get_tree_sitter_language_exception: PluginEdgeCases#test_get_tree_sitter_language_exception().
---
# Module: [`tests/unit/languages/test_typescript_plugin_edge_cases.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin_edge_cases.py)

## Classes
### `TestTypeScriptElementExtractorEdgeCases`
- def: [`tests/unit/languages/test_typescript_plugin_edge_cases.py:22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin_edge_cases.py#L22)
- doc: Edge case tests for TypeScriptElementExtractor
- signature: `class TestTypeScriptElementExtractorEdgeCases:`
- members:
  - `extractor(self)` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin_edge_cases.py#L26) — Create a TypeScriptElementExtractor instance for testing
  - `test_calculate_complexity_optimized_error_handling(self, extractor)` — [`L488`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin_edge_cases.py#L488) — Test complexity calculation with error handling
  - `test_extract_arrow_function_optimized_single_param(self, extractor)` — [`L92`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin_edge_cases.py#L92) — Test arrow function extraction with single parameter
  - `test_extract_arrow_function_optimized_with_parent(self, extractor)` — [`L56`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin_edge_cases.py#L56) — Test arrow function extraction with variable declarator parent
  - `test_extract_arrow_function_optimized_with_type_annotation(self, extractor)` — [`L117`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin_edge_cases.py#L117) — Test arrow function extraction with return type annotation
  - `test_extract_class_optimized_no_name(self, extractor)` — [`L158`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin_edge_cases.py#L158) — Test class extraction with no name
  - `test_extract_class_optimized_with_heritage(self, extractor)` — [`L169`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin_edge_cases.py#L169) — Test class extraction with inheritance and interfaces
  - `test_extract_commonjs_requires_error_handling(self, extractor)` — [`L465`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin_edge_cases.py#L465) — Test CommonJS require extraction with error handling
  - `test_extract_dynamic_import_error_handling(self, extractor)` — [`L455`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin_edge_cases.py#L455) — Test dynamic import extraction with error handling
  - `test_extract_dynamic_import_no_call_expression(self, extractor)` — [`L431`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin_edge_cases.py#L431) — Test dynamic import extraction with no call expression
  - `test_extract_dynamic_import_no_import_identifier(self, extractor)` — [`L440`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin_edge_cases.py#L440) — Test dynamic import extraction with no import identifier
  - `test_extract_enum_optimized_no_name(self, extractor)` — [`L246`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin_edge_cases.py#L246) — Test enum extraction with no name
  - `test_extract_function_optimized_error_handling(self, extractor)` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin_edge_cases.py#L30) — Test function extraction with error handling
  - `test_extract_function_optimized_exception(self, extractor)` — [`L42`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin_edge_cases.py#L42) — Test function extraction with exception
  - `test_extract_import_info_simple_error_handling(self, extractor)` — [`L419`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin_edge_cases.py#L419) — Test import extraction with error handling
  - `test_extract_import_info_simple_no_source(self, extractor)` — [`L406`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin_edge_cases.py#L406) — Test import extraction with no source string
  - `test_extract_interface_optimized_with_extends(self, extractor)` — [`L211`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin_edge_cases.py#L211) — Test interface extraction with extends clause
  - `test_extract_lexical_variable_optimized_const(self, extractor)` — [`L541`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin_edge_cases.py#L541) — Test lexical variable extraction for const
  - `test_extract_lexical_variable_optimized_let(self, extractor)` — [`L526`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin_edge_cases.py#L526) — Test lexical variable extraction for let
  - `test_extract_method_optimized_error_handling(self, extractor)` — [`L146`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin_edge_cases.py#L146) — Test method extraction with error handling
  - `test_extract_property_optimized_with_modifiers(self, extractor)` — [`L256`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin_edge_cases.py#L256) — Test property extraction with visibility modifiers
  - `test_extract_property_signature_optimized_optional(self, extractor)` — [`L294`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin_edge_cases.py#L294) — Test property signature extraction with optional property
  - `test_extract_tsdoc_for_line_error_handling(self, extractor)` — [`L477`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin_edge_cases.py#L477) — Test TSDoc extraction with error handling
  - `test_extract_variable_optimized_delegation(self, extractor)` — [`L512`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin_edge_cases.py#L512) — Test variable extraction delegation to _extract_variables_from_declaration
  - `test_extract_variables_from_declaration_error_handling(self, extractor)` — [`L498`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin_edge_cases.py#L498) — Test variable extraction from declaration with error handling
  - `test_parse_function_signature_optimized_no_name(self, extractor)` — [`L377`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin_edge_cases.py#L377) — Test function signature parsing with no name
  - `test_parse_method_signature_optimized_no_name(self, extractor)` — [`L391`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin_edge_cases.py#L391) — Test method signature parsing with no name
  - `test_parse_variable_declarator_with_arrow_function(self, extractor)` — [`L318`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin_edge_cases.py#L318) — Test variable declarator parsing that contains arrow function
  - `test_parse_variable_declarator_with_assignment(self, extractor)` — [`L341`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin_edge_cases.py#L341) — Test variable declarator parsing with assignment operator
- uses (calls/refs, reference-scoped): [`TypeScriptElementExtractor`](../../../tree_sitter_analyzer/languages/typescript_plugin/extractor.md#TypeScriptElementExtractor)

### `TestTypeScriptPluginEdgeCases`
- def: [`tests/unit/languages/test_typescript_plugin_edge_cases.py:557`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin_edge_cases.py#L557)
- doc: Edge case tests for TypeScriptPlugin
- signature: `class TestTypeScriptPluginEdgeCases:`
- members:
  - `plugin(self)` — [`L561`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin_edge_cases.py#L561) — Create a TypeScriptPlugin instance for testing
  - `test_analyze_file_encoding_error(self, plugin)` — [`L565`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin_edge_cases.py#L565) — Test file analysis with encoding error
  - `test_analyze_file_parser_creation_error(self, mock_load_language, plugin)` — [`L623`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin_edge_cases.py#L623) — Test file analysis with parser creation error
  - `test_analyze_file_permission_error(self, plugin)` — [`L594`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin_edge_cases.py#L594) — Test file analysis with permission error
  - `test_get_tree_sitter_language_exception(self, plugin)` — [`L650`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_plugin_edge_cases.py#L650) — Test tree-sitter language getter with exception
- uses (calls/refs, reference-scoped): [`AnalysisRequest`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest), [`file_path`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest.file_path), [`TypeScriptPlugin`](../../../tree_sitter_analyzer/languages/typescript_plugin/plugin.md#TypeScriptPlugin)

