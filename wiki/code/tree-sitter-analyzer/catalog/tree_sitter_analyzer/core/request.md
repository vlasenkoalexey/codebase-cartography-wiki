---
title: 'Module: tree_sitter_analyzer/core/request.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/core/request.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.core.request`/AnalysisRequest#
symbols:
  AnalysisRequest: ''
  AnalysisRequest.file_path: file_path.
  AnalysisRequest.language: language.
  AnalysisRequest.include_complexity: include_complexity.
  AnalysisRequest.include_details: include_details.
  AnalysisRequest.format_type: format_type.
  AnalysisRequest.queries: queries.
  AnalysisRequest.include_queries: include_queries.
  AnalysisRequest.include_elements: include_elements.
  AnalysisRequest.from_mcp_arguments: from_mcp_arguments().
---
# Module: [`tree_sitter_analyzer/core/request.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/request.py)

## Classes
### `AnalysisRequest`
- def: [`tree_sitter_analyzer/core/request.py:11`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/request.py#L11) — documented in [tree_sitter_analyzer-core-request](../../../concepts/tree_sitter_analyzer-core-request.md)
- doc: Analysis request
- signature: `class AnalysisRequest:`
- members:
  - `from_mcp_arguments(cls, arguments: dict[str, Any])` — [`L36`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/request.py#L36) — Create analysis request from MCP tool arguments
  - `file_path` — [`L26`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/request.py#L26) — documented in [tree_sitter_analyzer-core-request](../../../concepts/tree_sitter_analyzer-core-request.md)
  - `format_type` — [`L33`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/request.py#L33)
  - `include_complexity` — [`L31`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/request.py#L31) — documented in [tree_sitter_analyzer-core-request](../../../concepts/tree_sitter_analyzer-core-request.md)
  - `include_details` — [`L32`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/request.py#L32)
  - `include_elements` — [`L29`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/request.py#L29)
  - `include_queries` — [`L30`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/request.py#L30)
  - `language` — [`L27`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/request.py#L27) — documented in [tree_sitter_analyzer-core-request](../../../concepts/tree_sitter_analyzer-core-request.md)
  - `queries` — [`L28`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/request.py#L28)
- used by: [`_get_covered_node_types_from_plugin`](../grammar_coverage/validator.md#_get_covered_node_types_from_plugin), [`analyze_file`](../languages/rust_plugin.md#RustPlugin.analyze_file), [`analyze_file`](../plugins/base.md#LanguagePlugin.analyze_file), [`analyze_file`](../languages/go_plugin.md#GoPlugin.analyze_file), [`analyze_file`](../languages/c_plugin.md#CPlugin.analyze_file), [`analyze_file`](../languages/swift_plugin.md#SwiftPlugin.analyze_file), [`analyze`](_analysis_engine_analysis_mixin.md#UnifiedAnalysisEngineAnalysisMixin.analyze), [`analyze_file`](../languages/cpp_plugin.md#CppPlugin.analyze_file), [`analyze_file`](../languages/typescript_plugin/plugin.md#TypeScriptPlugin.analyze_file), [`analyze_file`](../languages/markdown_plugin/plugin.md#MarkdownPlugin.analyze_file), [`analyze_file`](../languages/kotlin_plugin.md#KotlinPlugin.analyze_file), [`analyze_file`](../languages/csharp_plugin.md#CSharpPlugin.analyze_file), [`analyze_file`](../languages/ruby_plugin.md#RubyPlugin.analyze_file), [`analyze_file`](_analysis_engine_file_mixin.md#UnifiedAnalysisEngineFileMixin.analyze_file), [`analyze_file`](../languages/php_plugin.md#PHPPlugin.analyze_file), [`analyze_file`](../languages/sql_plugin/plugin.md#SQLPlugin.analyze_file), [`analyze_file`](../languages/json_plugin.md#JSONPlugin.analyze_file), [`analyze_file`](../languages/yaml_plugin.md#YAMLPlugin.analyze_file), [`analyze_file`](../languages/java_plugin.md#JavaPlugin.analyze_file), [`analyze_file`](../languages/python_plugin/plugin.md#PythonPlugin.analyze_file), [`extract_elements`](../mcp/tools/utils/element_extractor.md#extract_elements), [`analyze_file`](../languages/bash_plugin.md#BashPlugin.analyze_file), [`analyze_file`](../languages/javascript_plugin/plugin.md#JavaScriptPlugin.analyze_file), [`build_request_from_params`](request_builder.md#build_request_from_params), [`_analyze_universal`](../mcp/tools/universal_analyze_tool.md#UniversalAnalyzeTool._analyze_universal), [`analyze_file`](analysis_engine.md#MockLanguagePlugin.analyze_file), [`analyze_file`](../cli/commands/base_command.md#BaseCommand.analyze_file), [`TREE_SITTER_AVAILABLE`](../languages/bash_plugin.md#TREE_SITTER_AVAILABLE), [`TREE_SITTER_AVAILABLE`](../languages/python_plugin/plugin.md#TREE_SITTER_AVAILABLE), [`_analyze_advanced`](../mcp/tools/universal_analyze_tool.md#UniversalAnalyzeTool._analyze_advanced), [`analyze_file`](../plugins/base.md#DefaultLanguagePlugin.analyze_file), [`update_request_from_params`](request_builder.md#update_request_from_params), [`_analyze_structure`](../mcp/tools/analyze_code_structure_tool.md#AnalyzeCodeStructureTool._analyze_structure), [`analyze_file`](../languages/scala_plugin.md#ScalaPlugin.analyze_file), [`analyze_code`](_analysis_engine_code_mixin.md#UnifiedAnalysisEngineCodeMixin.analyze_code), [`analyze_file`](../languages/css_plugin.md#CssPlugin.analyze_file), [`_analyze_file_sync`](../api.md#_analyze_file_sync), [`_clone_request_for_temp_path`](_analysis_engine_code_mixin.md#_clone_request_for_temp_path), [`_run_analysis_and_build_result`](../mcp/tools/analyze_scale_tool_cli_compatible.md#AnalyzeScaleToolCLICompatible._run_analysis_and_build_result), [`_run_structural_analysis`](../mcp/tools/analyze_scale_tool.md#AnalyzeScaleTool._run_structural_analysis)  (+19 more; 124 test-only)

