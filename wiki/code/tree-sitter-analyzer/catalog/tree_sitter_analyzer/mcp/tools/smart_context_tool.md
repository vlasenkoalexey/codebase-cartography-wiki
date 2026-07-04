---
title: 'Module: tree_sitter_analyzer/mcp/tools/smart_context_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/smart_context_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.smart_context_tool`/
symbols:
  SmartContextTool._build_profile: SmartContextTool#_build_profile().
  _build_smart_context_result: _build_smart_context_result().
  _build_agent_summary: _build_agent_summary().
  SmartContextTool.execute: SmartContextTool#execute().
  _safe_query: _safe_query().
  SmartContextTool: SmartContextTool#
  SmartContextTool._scorer: SmartContextTool#_scorer.
  SmartContextTool._get_graph: SmartContextTool#_get_graph().
  _resolve_graph_node: _resolve_graph_node().
  AgentSummaryInput.risk: AgentSummaryInput#risk.
  SmartContextTool._graph: SmartContextTool#_graph.
  AgentSummaryInput.file_path: AgentSummaryInput#file_path.
  AgentSummaryInput.grade: AgentSummaryInput#grade.
  AgentSummaryInput.test_files: AgentSummaryInput#test_files.
  SmartContextTool._get_scorer: SmartContextTool#_get_scorer().
  _build_syntax_error_result: _build_syntax_error_result().
  SmartContextProfile.health: SmartContextProfile#health.
  SmartContextProfile.dependents: SmartContextProfile#dependents.
  AgentSummaryInput: AgentSummaryInput#
  AgentSummaryInput.score: AgentSummaryInput#score.
  AgentSummaryInput.export_count: AgentSummaryInput#export_count.
  AgentSummaryInput.downstream_count: AgentSummaryInput#downstream_count.
  SmartContextTool._on_project_root_changed: SmartContextTool#_on_project_root_changed().
  _quick_risk: _quick_risk().
  SmartContextProfile.exports: SmartContextProfile#exports.
  SmartContextProfile.risk: SmartContextProfile#risk.
  AgentSummaryInput.weakest: AgentSummaryInput#weakest.
  SmartContextProfile: SmartContextProfile#
  SmartContextProfile.file_path: SmartContextProfile#file_path.
  SmartContextProfile.dependencies: SmartContextProfile#dependencies.
  SmartContextProfile.test_files: SmartContextProfile#test_files.
  logger: logger.
  SmartContextTool.get_tool_definition: SmartContextTool#get_tool_definition().
  SmartContextProfile.line_count: SmartContextProfile#line_count.
  SmartContextProfile.language: SmartContextProfile#language.
  SmartContextProfile.structure: SmartContextProfile#structure.
  _to_relative: _to_relative().
  SmartContextTool.get_tool_schema: SmartContextTool#get_tool_schema().
  SmartContextTool.validate_arguments: SmartContextTool#validate_arguments().
  _risk_to_verdict: _risk_to_verdict().
  _focused_test_command: _focused_test_command().
  _agent_next_step: _agent_next_step().
  _agent_stop_condition: _agent_stop_condition().
  _weakest_dimension: _weakest_dimension().
  _build_summary: _build_summary().
  SmartContextTool.__init__: SmartContextTool#__init__().
---
# Module: [`tree_sitter_analyzer/mcp/tools/smart_context_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/smart_context_tool.py)

## Classes
### `AgentSummaryInput`
- def: [`tree_sitter_analyzer/mcp/tools/smart_context_tool.py:49`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/smart_context_tool.py#L49)
- signature: `class AgentSummaryInput:`
- members:
  - `downstream_count` — [`L56`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/smart_context_tool.py#L56)
  - `export_count` — [`L55`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/smart_context_tool.py#L55)
  - `file_path` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/smart_context_tool.py#L50)
  - `grade` — [`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/smart_context_tool.py#L51)
  - `risk` — [`L54`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/smart_context_tool.py#L54)
  - `score` — [`L52`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/smart_context_tool.py#L52)
  - `test_files` — [`L57`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/smart_context_tool.py#L57)
  - `weakest` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/smart_context_tool.py#L53)
- used by: [`_build_smart_context_result`](smart_context_tool.md#_build_smart_context_result), [`_build_agent_summary`](smart_context_tool.md#_build_agent_summary)  (2 test-only)

### `SmartContextProfile`
- def: [`tree_sitter_analyzer/mcp/tools/smart_context_tool.py:35`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/smart_context_tool.py#L35)
- signature: `class SmartContextProfile:`
- members:
  - `dependencies` — [`L42`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/smart_context_tool.py#L42)
  - `dependents` — [`L43`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/smart_context_tool.py#L43)
  - `exports` — [`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/smart_context_tool.py#L40)
  - `file_path` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/smart_context_tool.py#L36)
  - `health` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/smart_context_tool.py#L39)
  - `language` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/smart_context_tool.py#L38)
  - `line_count` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/smart_context_tool.py#L37)
  - `risk` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/smart_context_tool.py#L45)
  - `structure` — [`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/smart_context_tool.py#L41)
  - `test_files` — [`L44`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/smart_context_tool.py#L44)
- used by: [`_build_profile`](smart_context_tool.md#SmartContextTool._build_profile), [`_build_smart_context_result`](smart_context_tool.md#_build_smart_context_result)

### `SmartContextTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/smart_context_tool.py:60`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/smart_context_tool.py#L60)
- doc: MCP Tool that provides a compact file profile combining multiple analyses.
- signature: `class SmartContextTool(BaseMCPTool):`
- members:
  - `execute(self, arguments: dict[str, Any])` — [`L149`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/smart_context_tool.py#L149)
  - `get_tool_definition(self)` — [`L87`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/smart_context_tool.py#L87)
  - `get_tool_schema(self)` — [`L120`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/smart_context_tool.py#L120)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L140`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/smart_context_tool.py#L140)
- protocol/private: `__init__`[`L63`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/smart_context_tool.py#L63), `_build_profile`[`L178`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/smart_context_tool.py#L178), `_get_graph`[`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/smart_context_tool.py#L73), `_get_scorer`[`L81`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/smart_context_tool.py#L81), `_graph`[`L64`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/smart_context_tool.py#L64), `_on_project_root_changed`[`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/smart_context_tool.py#L68), `_scorer`[`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/smart_context_tool.py#L65)
- uses (calls/refs, reference-scoped): [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`project_root`](base_tool.md#BaseMCPTool.project_root), [`apply_toon_format_to_response`](../utils/format_helper.md#apply_toon_format_to_response), [`detect_language_from_file`](../../language_detector.md#detect_language_from_file), [`DependencyGraph`](../../project_graph.md#DependencyGraph), [`resolve_and_validate_file_path`](base_tool.md#BaseMCPTool.resolve_and_validate_file_path), [`_build_smart_context_result`](smart_context_tool.md#_build_smart_context_result), [`__init__`](base_tool.md#BaseMCPTool.__init__), [`HealthScorer`](../../health_scorer.md#HealthScorer), [`extract_elements`](utils/element_extractor.md#extract_elements), [`get_all_exports`](utils/element_extractor.md#get_all_exports), [`score_file`](../../health_scorer.md#HealthScorer.score_file), [`get_structure`](utils/element_extractor.md#get_structure), [`is_file_parse_broken`](utils/parse_validity.md#is_file_parse_broken), [`grade`](../../health_scorer.md#HealthScore.grade), [`_safe_query`](smart_context_tool.md#_safe_query), [`_build_syntax_error_result`](smart_context_tool.md#_build_syntax_error_result), [`_quick_risk`](smart_context_tool.md#_quick_risk), [`dependents`](smart_context_tool.md#SmartContextProfile.dependents), [`health`](smart_context_tool.md#SmartContextProfile.health), [`exports`](smart_context_tool.md#SmartContextProfile.exports), [`risk`](smart_context_tool.md#SmartContextProfile.risk), [`SmartContextProfile`](smart_context_tool.md#SmartContextProfile), [`dependencies`](smart_context_tool.md#SmartContextProfile.dependencies), [`file_path`](smart_context_tool.md#SmartContextProfile.file_path), [`test_files`](smart_context_tool.md#SmartContextProfile.test_files), [`_to_relative`](smart_context_tool.md#_to_relative), [`language`](smart_context_tool.md#SmartContextProfile.language), [`line_count`](smart_context_tool.md#SmartContextProfile.line_count), [`structure`](smart_context_tool.md#SmartContextProfile.structure)  (1 test-only)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`_on_project_root_changed`](base_tool.md#BaseMCPTool._on_project_root_changed), [`build_project_facade`](project_facade.md#build_project_facade)  (2 test-only)

## Functions
- `_agent_next_step(*, file_path: str, grade: str, risk: str, has_tests: bool)` — [`L418`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/smart_context_tool.py#L418)
- `_agent_stop_condition(verification_command: str, test_files: list[str])` — [`L444`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/smart_context_tool.py#L444)
- `_build_agent_summary(context: AgentSummaryInput)` — [`L342`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/smart_context_tool.py#L342)
- `_build_smart_context_result(profile: SmartContextProfile)` — [`L242`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/smart_context_tool.py#L242)
- `_build_summary(grade: str, risk: str, export_count: int, downstream_count: int)` — [`L487`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/smart_context_tool.py#L487)
- `_build_syntax_error_result(resolved: str, language: str | None, project_root: str | None, output_format: str)` — [`L288`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/smart_context_tool.py#L288) — #754: syntax-error short-circuit that preserves the happy-path key shape.
- `_focused_test_command(test_files: list[str])` — [`L410`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/smart_context_tool.py#L410)
- `_quick_risk(downstream: int, grade: str, has_tests: bool)` — [`L453`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/smart_context_tool.py#L453)
- `_resolve_graph_node(graph: DependencyGraph, rel_path: str)` — [`L235`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/smart_context_tool.py#L235)
- `_risk_to_verdict(risk: str)` — [`L392`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/smart_context_tool.py#L392) — Map smart_context's ``risk`` label to the safe_to_edit verdict vocab.
- `_safe_query(graph: DependencyGraph, rel_path: str, method: str)` — [`L224`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/smart_context_tool.py#L224)
- `_to_relative(abs_path: str, project_root: str)` — [`L216`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/smart_context_tool.py#L216)
- `_weakest_dimension(dimensions: dict[str, float])` — [`L479`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/smart_context_tool.py#L479)

## Module values
- `logger` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/smart_context_tool.py#L31)

