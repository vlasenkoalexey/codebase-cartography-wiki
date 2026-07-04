---
title: 'Module: tree_sitter_analyzer/models/result.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/models/result.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.models.result`/
symbols:
  AnalysisResult: AnalysisResult#
  AnalysisResult.elements: AnalysisResult#elements.
  AnalysisResult.language: AnalysisResult#language.
  AnalysisResult.file_path: AnalysisResult#file_path.
  AnalysisResult.success: AnalysisResult#success.
  AnalysisResult.line_count: AnalysisResult#line_count.
  AnalysisResult.error_message: AnalysisResult#error_message.
  AnalysisResult.source_code: AnalysisResult#source_code.
  AnalysisResult.node_count: AnalysisResult#node_count.
  AnalysisResult.to_dict: AnalysisResult#to_dict().
  AnalysisResult.to_mcp_format: AnalysisResult#to_mcp_format().
  AnalysisResult.query_results: AnalysisResult#query_results.
  AnalysisResult.get_summary: AnalysisResult#get_summary().
  AnalysisResult.to_summary_dict: AnalysisResult#to_summary_dict().
  AnalysisResult.package: AnalysisResult#package.
  AnalysisResult.analysis_time: AnalysisResult#analysis_time.
  AnalysisResult.to_json: AnalysisResult#to_json().
  AnalysisResult.modules: AnalysisResult#modules.
  AnalysisResult.get_statistics: AnalysisResult#get_statistics().
  AnalysisResult.goroutines: AnalysisResult#goroutines.
  AnalysisResult.impls: AnalysisResult#impls.
  AnalysisResult.channels: AnalysisResult#channels.
  AnalysisResult.defers: AnalysisResult#defers.
  AnalysisResult.throws: AnalysisResult#throws.
  AnalysisResult.complexity_score: AnalysisResult#complexity_score.
  AnalysisResult.is_suspend: AnalysisResult#is_suspend.
  AnalysisResult.receiver: AnalysisResult#receiver.
  AnalysisResult.receiver_type: AnalysisResult#receiver_type.
  AnalysisResult.is_constructor: AnalysisResult#is_constructor.
  AnalysisResult.__post_init__: AnalysisResult#__post_init__().
  __all__: __all__.
---
# Module: [`tree_sitter_analyzer/models/result.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/result.py)

## Classes
### `AnalysisResult`
- def: [`tree_sitter_analyzer/models/result.py:44`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/result.py#L44) — documented in [tree_sitter_analyzer-mcp-tools-base_tool](../../../concepts/tree_sitter_analyzer-mcp-tools-base_tool.md)
- doc: Comprehensive analysis result container
- signature: `class AnalysisResult:`
- members:
  - `get_statistics(self)` — [`L201`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/result.py#L201) — Get detailed statistics (alias for get_summary)
  - `get_summary(self)` — [`L148`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/result.py#L148) — Get analysis summary statistics using unified elements
  - `to_dict(self)` — [`L87`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/result.py#L87) — Convert analysis result to dictionary for serialization. — documented in [tree_sitter_analyzer-models-result](../../../concepts/tree_sitter_analyzer-models-result.md)
  - `to_json(self)` — [`L205`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/result.py#L205) — Convert to JSON-serializable format (alias for to_dict)
  - `to_mcp_format(self)` — [`L173`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/result.py#L173) — Produce output in MCP-compatible format. — documented in [tree_sitter_analyzer-models-result](../../../concepts/tree_sitter_analyzer-models-result.md)
  - `to_summary_dict(self, types: list[str] | None = None)` — [`L110`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/result.py#L110) — Return analysis summary as a dictionary using unified elements.
  - `analysis_time` — [`L65`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/result.py#L65)
  - `channels` — [`L81`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/result.py#L81)
  - `complexity_score` — [`L71`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/result.py#L71)
  - `defers` — [`L82`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/result.py#L82)
  - `elements` — [`L50`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/result.py#L50) — documented in [tree_sitter_analyzer-mcp-tools-base_tool](../../../concepts/tree_sitter_analyzer-mcp-tools-base_tool.md)
  - `error_message` — [`L67`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/result.py#L67)
  - `file_path` — [`L47`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/result.py#L47) — documented in [tree_sitter_analyzer-models-result](../../../concepts/tree_sitter_analyzer-models-result.md)
  - `goroutines` — [`L80`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/result.py#L80)
  - `impls` — [`L79`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/result.py#L79)
  - `is_constructor` — [`L77`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/result.py#L77)
  - `is_suspend` — [`L74`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/result.py#L74)
  - `language` — [`L48`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/result.py#L48) — documented in [tree_sitter_analyzer-models-result](../../../concepts/tree_sitter_analyzer-models-result.md)
  - `line_count` — [`L49`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/result.py#L49)
  - `modules` — [`L78`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/result.py#L78)
  - `node_count` — [`L53`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/result.py#L53)
  - `package` — [`L58`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/result.py#L58)
  - `query_results` — [`L54`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/result.py#L54)
  - `receiver` — [`L75`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/result.py#L75)
  - `receiver_type` — [`L76`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/result.py#L76)
  - `source_code` — [`L57`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/result.py#L57)
  - `success` — [`L66`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/result.py#L66)
  - `throws` — [`L70`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/result.py#L70)
- protocol/private: `__post_init__`[`L84`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/result.py#L84)
- uses (calls/refs, reference-scoped): [`CodeElement`](base.md#CodeElement), [`ELEMENT_TYPE_CLASS`](../constants.md#ELEMENT_TYPE_CLASS), [`ELEMENT_TYPE_FUNCTION`](../constants.md#ELEMENT_TYPE_FUNCTION), [`is_element_of_type`](../constants.md#is_element_of_type), [`ELEMENT_TYPE_VARIABLE`](../constants.md#ELEMENT_TYPE_VARIABLE), [`ELEMENT_TYPE_IMPORT`](../constants.md#ELEMENT_TYPE_IMPORT), [`get_element_type`](../constants.md#get_element_type), [`to_summary_item`](base.md#CodeElement.to_summary_item), [`_group_elements_by_type`](_result_helpers.md#_group_elements_by_type), [`_mcp_metadata_block`](_result_helpers.md#_mcp_metadata_block), [`_mcp_annotation_entries`](_result_helpers.md#_mcp_annotation_entries), [`_mcp_class_entries`](_result_helpers.md#_mcp_class_entries), [`_mcp_field_entries`](_result_helpers.md#_mcp_field_entries), [`_mcp_import_entries`](_result_helpers.md#_mcp_import_entries), [`_mcp_method_entries`](_result_helpers.md#_mcp_method_entries), [`ELEMENT_TYPE_ANNOTATION`](../constants.md#ELEMENT_TYPE_ANNOTATION), [`JavaPackage`](java_models.md#JavaPackage), [`_mcp_package_info`](_result_helpers.md#_mcp_package_info), [`_to_dict_annotation_row`](_result_helpers.md#_to_dict_annotation_row), [`_to_dict_class_row`](_result_helpers.md#_to_dict_class_row), [`_to_dict_field_row`](_result_helpers.md#_to_dict_field_row), [`_to_dict_import_row`](_result_helpers.md#_to_dict_import_row), [`_to_dict_method_row`](_result_helpers.md#_to_dict_method_row)
- used by: [`_get_covered_node_types_from_plugin`](../grammar_coverage/validator.md#_get_covered_node_types_from_plugin), [`analyze_file`](../languages/rust_plugin.md#RustPlugin.analyze_file), [`analyze_file`](../plugins/base.md#LanguagePlugin.analyze_file), [`analyze_file`](../languages/go_plugin.md#GoPlugin.analyze_file), [`analyze_file`](../languages/c_plugin.md#CPlugin.analyze_file), [`analyze_file`](../languages/swift_plugin.md#SwiftPlugin.analyze_file), [`analyze_file`](../languages/cpp_plugin.md#CppPlugin.analyze_file), [`analyze_file`](../languages/typescript_plugin/plugin.md#TypeScriptPlugin.analyze_file), [`analyze_file`](../languages/markdown_plugin/plugin.md#MarkdownPlugin.analyze_file), [`_analyze_html_fallback`](../languages/html_plugin.md#_analyze_html_fallback), [`analyze_file`](../languages/kotlin_plugin.md#KotlinPlugin.analyze_file), [`analyze_file`](../languages/csharp_plugin.md#CSharpPlugin.analyze_file), [`analyze_file`](../languages/ruby_plugin.md#RubyPlugin.analyze_file), [`format_analysis_result`](../formatters/toon_formatter.md#ToonFormatter.format_analysis_result), [`analyze_file`](../languages/php_plugin.md#PHPPlugin.analyze_file), [`analyze_file`](../languages/sql_plugin/plugin.md#SQLPlugin.analyze_file), [`_analyze_css_fallback`](../languages/css_plugin.md#_analyze_css_fallback), [`analyze_file`](../languages/json_plugin.md#JSONPlugin.analyze_file), [`analyze_file`](../languages/yaml_plugin.md#YAMLPlugin.analyze_file), [`analyze_file`](../languages/java_plugin.md#JavaPlugin.analyze_file), [`analyze_file`](../languages/python_plugin/plugin.md#PythonPlugin.analyze_file), [`_output_statistics`](../cli/commands/advanced_command.md#AdvancedCommand._output_statistics), [`extract_elements`](../mcp/tools/utils/element_extractor.md#extract_elements), [`get_all_exports`](../mcp/tools/utils/element_extractor.md#get_all_exports), [`analyze_file`](../languages/bash_plugin.md#BashPlugin.analyze_file), [`analyze_file`](../languages/javascript_plugin/plugin.md#JavaScriptPlugin.analyze_file), [`_output_full_analysis`](../cli/commands/advanced_command.md#AdvancedCommand._output_full_analysis), [`_analyze_with_tree_sitter`](../languages/css_plugin.md#CssPlugin._analyze_with_tree_sitter), [`analyze_file`](../core/analysis_engine.md#MockLanguagePlugin.analyze_file), [`analyze_file`](../cli/commands/base_command.md#BaseCommand.analyze_file), [`TREE_SITTER_AVAILABLE`](../languages/bash_plugin.md#TREE_SITTER_AVAILABLE), [`_analyze_with_tree_sitter`](../languages/html_plugin.md#HtmlPlugin._analyze_with_tree_sitter), [`get_functions`](../mcp/tools/utils/element_extractor.md#get_functions), [`TREE_SITTER_AVAILABLE`](../languages/python_plugin/plugin.md#TREE_SITTER_AVAILABLE), [`_convert_to_legacy_format`](../cli/commands/structure_command.md#StructureCommand._convert_to_legacy_format), [`analyze_file`](../plugins/base.md#DefaultLanguagePlugin.analyze_file), [`_format_internal`](../formatters/toon_formatter.md#ToonFormatter._format_internal), [`_output_text_analysis`](../cli/commands/advanced_command.md#AdvancedCommand._output_text_analysis), [`_output_summary_analysis`](../cli/commands/summary_command.md#SummaryCommand._output_summary_analysis), [`_scala_analysis_result`](../languages/scala_plugin.md#ScalaPlugin._scala_analysis_result)  (+41 more; 238 test-only)

## Module values
- `__all__` — [`L210`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/result.py#L210)

