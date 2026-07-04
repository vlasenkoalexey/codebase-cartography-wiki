---
title: 'Module: tree_sitter_analyzer/mcp/tools/base_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/base_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.base_tool`/
symbols:
  BaseMCPTool: BaseMCPTool#
  BaseMCPTool.project_root: BaseMCPTool#project_root().
  BaseMCPTool.execute: BaseMCPTool#execute().
  BaseMCPTool.get_tool_definition: BaseMCPTool#get_tool_definition().
  BaseMCPTool.get_tool_schema: BaseMCPTool#get_tool_schema().
  BaseMCPTool.validate_arguments: BaseMCPTool#validate_arguments().
  BaseMCPTool._on_project_root_changed: BaseMCPTool#_on_project_root_changed().
  BaseMCPTool.resolve_and_validate_file_path: BaseMCPTool#resolve_and_validate_file_path().
  BaseMCPTool.__init__: BaseMCPTool#__init__().
  BaseMCPTool.path_resolver: BaseMCPTool#path_resolver.
  BaseMCPTool.set_project_path: BaseMCPTool#set_project_path().
  mirror_summary_line: mirror_summary_line().
  BaseMCPTool.security_validator: BaseMCPTool#security_validator.
  _canonicalize_verdict: _canonicalize_verdict().
  BaseMCPTool.resolve_and_validate_directory_path: BaseMCPTool#resolve_and_validate_directory_path().
  detect_language_mismatch: detect_language_mismatch().
  language_mismatch_error_response: language_mismatch_error_response().
  format_summary_line: format_summary_line().
  MCPTool: MCPTool#
  _LEGAL_VERDICTS._LEGAL_VERDICTS: _LEGAL_VERDICTS._LEGAL_VERDICTS.
  logger: logger.
  BaseMCPTool.__init_subclass__: BaseMCPTool#__init_subclass__().
  BaseMCPTool._wrapped: BaseMCPTool#_wrapped().
  BaseMCPTool._guard_strict_parameters: BaseMCPTool#_guard_strict_parameters().
  BaseMCPTool._apply_project_root: BaseMCPTool#_apply_project_root().
  BaseMCPTool.get_output_schema: BaseMCPTool#get_output_schema().
  MCPTool.get_tool_definition: MCPTool#get_tool_definition().
  MCPTool.execute: MCPTool#execute().
  MCPTool.validate_arguments: MCPTool#validate_arguments().
  BaseMCPTool._project_root: BaseMCPTool#_project_root.
  _F5_WRAPPED_ATTR: _F5_WRAPPED_ATTR.
  BaseMCPTool._normalize_file_path: BaseMCPTool#_normalize_file_path().
  _VERDICT_ALIASES._VERDICT_ALIASES: _VERDICT_ALIASES._VERDICT_ALIASES.
  BaseMCPTool._project_root_initialized: BaseMCPTool#_project_root_initialized.
  MCPTool.get_tool_schema: MCPTool#get_tool_schema().
---
# Module: [`tree_sitter_analyzer/mcp/tools/base_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/base_tool.py)

## Classes
### `BaseMCPTool`  ·  implements/extends ABC
- def: [`tree_sitter_analyzer/mcp/tools/base_tool.py:282`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/base_tool.py#L282) — documented in [tree_sitter_analyzer-mcp-server](../../../../concepts/tree_sitter_analyzer-mcp-server.md)
- doc: Base class for all MCP tools.
- signature: `class BaseMCPTool(ABC):`
- members:
  - `__init__(self, project_root: str | None = None)` — [`L343`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/base_tool.py#L343) — Initialize the base MCP tool.
  - `__init_subclass__(cls, **kwargs: Any)` — [`L290`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/base_tool.py#L290) — F5: wrap every subclass's ``execute`` with strict-parameter check.
  - `_apply_project_root(self, project_root: str | None, *, _is_init: bool)` — [`L408`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/base_tool.py#L408) — Single internal entry point for both constructor and rebind paths.
  - `_guard_strict_parameters(self, arguments: dict[str, Any])` — [`L325`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/base_tool.py#L325) — Refuse unknown top-level parameters using the tool's own schema.
  - `_normalize_file_path(raw: str)` — [`L454`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/base_tool.py#L454) — Strip leading ``./`` and normalize separators for consistent echo.
  - `_on_project_root_changed(self, project_root: str | None)` — [`L440`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/base_tool.py#L440) — Hook for subclasses to reset lazy caches when project_root rebinds.
  - `execute(self, arguments: dict[str, Any])` — [`L658`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/base_tool.py#L658) — Execute the tool with the given arguments. — documented in [tree_sitter_analyzer-mcp-tools-base_tool](../../../../concepts/tree_sitter_analyzer-mcp-tools-base_tool.md)
  - `get_output_schema(self)` — [`L566`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/base_tool.py#L566) — Return the canonical ``outputSchema`` for the ToolResponse envelope.
  - `get_tool_definition(self)` — [`L648`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/base_tool.py#L648) — Get the MCP tool definition. — documented in [tree_sitter_analyzer-mcp-tools-base_tool](../../../../concepts/tree_sitter_analyzer-mcp-tools-base_tool.md)
  - `get_tool_schema(self)` — [`L636`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/base_tool.py#L636) — Return the JSON Schema for the tool's input parameters.
  - `project_root(self)` — [`L362`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/base_tool.py#L362) — The current project root for this tool. — documented in [tree_sitter_analyzer-mcp-server](../../../../concepts/tree_sitter_analyzer-mcp-server.md)
  - `resolve_and_validate_directory_path(self, dir_path: str)` — [`L541`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/base_tool.py#L541) — Resolve a directory path and validate it.
  - `resolve_and_validate_file_path(self, file_path: str)` — [`L489`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/base_tool.py#L489) — Resolve a file path and validate it with caching to avoid redundant checks. — documented in [tree_sitter_analyzer-mcp-tools-read_partial_tool](../../../../concepts/tree_sitter_analyzer-mcp-tools-read_partial_tool.md)
  - `set_project_path(self, project_path: str)` — [`L394`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/base_tool.py#L394) — Update the project path for all components.
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L671`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/base_tool.py#L671) — Validate tool arguments.
  - `path_resolver` — [`L418`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/base_tool.py#L418) — documented in [tree_sitter_analyzer-mcp-tools-read_partial_tool](../../../../concepts/tree_sitter_analyzer-mcp-tools-read_partial_tool.md)
  - `security_validator` — [`L417`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/base_tool.py#L417) — documented in [tree_sitter_analyzer-security-validator](../../../../concepts/tree_sitter_analyzer-security-validator.md)
- protocol/private: `_project_root`[`L392`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/base_tool.py#L392), `_project_root_initialized`[`L416`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/base_tool.py#L416), `_wrapped`[`L316`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/base_tool.py#L316)
- uses (calls/refs, reference-scoped): [`SearchContentTool`](search_content_tool.md#SearchContentTool), [`ReadPartialTool`](read_partial_tool.md#ReadPartialTool), [`execute`](list_files_tool.md#ListFilesTool.execute), [`ListFilesTool`](list_files_tool.md#ListFilesTool), [`execute`](facade_tool.md#FacadeTool.execute), [`execute`](search_content_tool.md#SearchContentTool.execute), [`SecurityValidator`](../../security/validator.md#SecurityValidator), [`AnalyzeCodeStructureTool`](analyze_code_structure_tool.md#AnalyzeCodeStructureTool), [`execute`](codegraph_pr_review_tool.md#CodeGraphPRReviewTool.execute), [`FindAndGrepTool`](find_and_grep_tool.md#FindAndGrepTool), [`QueryTool`](query_tool.md#QueryTool), [`AnalyzeScaleTool`](analyze_scale_tool.md#AnalyzeScaleTool), [`UniversalAnalyzeTool`](universal_analyze_tool.md#UniversalAnalyzeTool), [`GetCodeOutlineTool`](get_code_outline_tool.md#GetCodeOutlineTool), [`validate_file_path`](../../security/validator.md#SecurityValidator.validate_file_path), [`execute`](find_and_grep_tool.md#FindAndGrepTool.execute), [`execute`](change_impact_tool.md#ChangeImpactTool.execute), [`execute`](analyze_code_structure_tool.md#AnalyzeCodeStructureTool.execute), [`execute`](callers_tool.md#CodeGraphCallersTool.execute), [`execute`](get_code_outline_tool.md#GetCodeOutlineTool.execute), [`execute`](codegraph_query_tool.md#CodeGraphQueryTool.execute), [`FacadeTool`](facade_tool.md#FacadeTool), [`CodeGraphContextTool`](codegraph_context_tool.md#CodeGraphContextTool), [`execute`](dead_code_tool.md#CodeGraphDeadCodeTool.execute), [`execute`](read_partial_tool.md#ReadPartialTool.execute), [`execute`](analyze_scale_tool.md#AnalyzeScaleTool.execute), [`execute`](symbol_lineage_tool.md#SymbolLineageTool.execute), [`PathResolver`](../utils/path_resolver.md#PathResolver), [`execute`](codegraph_explore_tool.md#CodeGraphExploreTool.execute), [`execute`](callees_tool.md#CodeGraphCalleesTool.execute), [`execute`](code_patterns_tool.md#CodePatternsTool.execute), [`resolve`](../utils/path_resolver.md#PathResolver.resolve), [`execute`](class_inspect_tool.md#ClassInspectTool.execute), [`execute`](codegraph_context_tool.md#CodeGraphContextTool.execute), [`execute`](query_tool.md#QueryTool.execute), [`CodeGraphCallersTool`](callers_tool.md#CodeGraphCallersTool), [`execute`](class_hierarchy_tool.md#ClassHierarchyTool.execute), [`execute`](uml_tool.md#CodeGraphUMLTool.execute), [`CodeGraphSymbolSearchTool`](symbol_search_tool.md#CodeGraphSymbolSearchTool), [`execute`](trace_impact_tool.md#TraceImpactTool.execute)  (+400 more; 69 test-only)
- used by: [`SearchContentTool`](search_content_tool.md#SearchContentTool), [`ReadPartialTool`](read_partial_tool.md#ReadPartialTool), [`execute`](list_files_tool.md#ListFilesTool.execute), [`ListFilesTool`](list_files_tool.md#ListFilesTool), [`execute`](facade_tool.md#FacadeTool.execute), [`execute`](search_content_tool.md#SearchContentTool.execute), [`AnalyzeCodeStructureTool`](analyze_code_structure_tool.md#AnalyzeCodeStructureTool), [`execute`](codegraph_pr_review_tool.md#CodeGraphPRReviewTool.execute), [`FindAndGrepTool`](find_and_grep_tool.md#FindAndGrepTool), [`QueryTool`](query_tool.md#QueryTool), [`AnalyzeScaleTool`](analyze_scale_tool.md#AnalyzeScaleTool), [`action_map`](facade_tool.md#FacadeTool.action_map), [`UniversalAnalyzeTool`](universal_analyze_tool.md#UniversalAnalyzeTool), [`GetCodeOutlineTool`](get_code_outline_tool.md#GetCodeOutlineTool), [`_apply_step`](codegraph_query_tool.md#CodeGraphQueryTool._apply_step), [`execute`](change_impact_tool.md#ChangeImpactTool.execute), [`FacadeTool`](facade_tool.md#FacadeTool), [`CodeGraphContextTool`](codegraph_context_tool.md#CodeGraphContextTool), [`execute`](dead_code_tool.md#CodeGraphDeadCodeTool.execute), [`execute`](read_partial_tool.md#ReadPartialTool.execute), [`execute`](symbol_lineage_tool.md#SymbolLineageTool.execute), [`execute`](codegraph_explore_tool.md#CodeGraphExploreTool.execute), [`execute`](code_patterns_tool.md#CodePatternsTool.execute), [`_build_profile`](smart_context_tool.md#SmartContextTool._build_profile), [`execute`](class_inspect_tool.md#ClassInspectTool.execute), [`execute`](codegraph_context_tool.md#CodeGraphContextTool.execute), [`execute`](query_tool.md#QueryTool.execute), [`CodeGraphCallersTool`](callers_tool.md#CodeGraphCallersTool), [`execute`](class_hierarchy_tool.md#ClassHierarchyTool.execute), [`execute`](uml_tool.md#CodeGraphUMLTool.execute), [`CodeGraphSymbolSearchTool`](symbol_search_tool.md#CodeGraphSymbolSearchTool), [`CodePatternsTool`](code_patterns_tool.md#CodePatternsTool), [`execute`](universal_analyze_tool.md#UniversalAnalyzeTool.execute), [`CodeGraphCalleesTool`](callees_tool.md#CodeGraphCalleesTool), [`CodeGraphUMLTool`](uml_tool.md#CodeGraphUMLTool), [`_execute_pr_analysis`](change_impact_tool.md#ChangeImpactTool._execute_pr_analysis), [`ASTCacheTool`](ast_cache_tool.md#ASTCacheTool), [`execute_batch`](batch_executor.md#execute_batch), [`execute`](safe_to_edit_tool.md#SafeToEditTool.execute), [`execute`](knowledge_graph_tool.md#CodeGraphKnowledgeIndexTool.execute)  (+264 more; 138 test-only)

### `MCPTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/base_tool.py:688`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/base_tool.py#L688)
- doc: Protocol for MCP tools (deprecated, use BaseMCPTool instead).
- signature: `class MCPTool(BaseMCPTool):`
- members:
  - `execute(self, arguments: dict[str, Any])` — [`L712`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/base_tool.py#L712) — Execute the tool with the given arguments.
  - `get_tool_definition(self)` — [`L703`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/base_tool.py#L703) — Get the MCP tool definition.
  - `get_tool_schema(self)` — [`L696`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/base_tool.py#L696) — Return the JSON Schema for the tool's input parameters.
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L724`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/base_tool.py#L724) — Validate tool arguments.
- uses (calls/refs, reference-scoped): [`BaseMCPTool`](base_tool.md#BaseMCPTool)  (6 test-only)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments)  (4 test-only)

## Functions
- `_canonicalize_verdict(value: str | None)` — [`L64`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/base_tool.py#L64) — Return a verdict guaranteed to belong to ``_LEGAL_VERDICTS``.
- `detect_language_mismatch(file_path: str, explicit_language: str | None, *, project_root: str | None = None)` — [`L192`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/base_tool.py#L192) — Return a warning message if explicit ``language`` disagrees with the file extension.
- `format_summary_line(*parts: Any)` — [`L169`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/base_tool.py#L169) — Join non-empty segments with single spaces into a clean summary line.
- `language_mismatch_error_response(*, tool_name: str, file_path: str, warning: str)` — [`L245`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/base_tool.py#L245) — Canonical strict error envelope for the language-mismatch gate.
- `mirror_summary_line(result: dict[str, Any])` — [`L125`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/base_tool.py#L125) — Mirror ``agent_summary.summary_line`` to the top-level envelope.

## Module values
- `_F5_WRAPPED_ATTR` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/base_tool.py#L25)
- `_LEGAL_VERDICTS` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/base_tool.py#L38)
- `_VERDICT_ALIASES` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/base_tool.py#L53)
- `logger` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/base_tool.py#L21)

