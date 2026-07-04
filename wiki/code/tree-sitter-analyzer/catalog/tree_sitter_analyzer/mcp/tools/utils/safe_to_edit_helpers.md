---
title: 'Module: tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.utils.safe_to_edit_helpers`/
symbols:
  _format_safe_to_edit_result: _format_safe_to_edit_result().
  _collect_safe_to_edit_facts: _collect_safe_to_edit_facts().
  build_agent_workflow: build_agent_workflow().
  build_agent_summary: build_agent_summary().
  build_file_dependency_view: build_file_dependency_view().
  _relative_for_constraints: _relative_for_constraints().
  _target_dependents: _target_dependents().
  build_safe_to_edit_result: build_safe_to_edit_result().
  SafeToEditContext.project_root: SafeToEditContext#project_root.
  _format_recommendation: _format_recommendation().
  _agent_next_step: _agent_next_step().
  safe_dependencies: safe_dependencies().
  SafeToEditContext.resolved_path: SafeToEditContext#resolved_path.
  AgentWorkflowContext.risk: AgentWorkflowContext#risk.
  _target_dependencies: _target_dependencies().
  _iter_dependency_source_files: _iter_dependency_source_files().
  SafeToEditContext.file_path: SafeToEditContext#file_path.
  SafeToEditContext: SafeToEditContext#
  SafeToEditFacts.health: SafeToEditFacts#health.
  _agent_stop_condition: _agent_stop_condition().
  FileDependencyView.dependencies_of: FileDependencyView#dependencies_of().
  _max_verdict: _max_verdict().
  safe_dependents: safe_dependents().
  FileDependencyView: FileDependencyView#
  AgentWorkflowContext: AgentWorkflowContext#
  AgentWorkflowContext.has_tests: AgentWorkflowContext#has_tests.
  SafeToEditContext.scorer: SafeToEditContext#scorer.
  FileDependencyView.dependents_of: FileDependencyView#dependents_of().
  _safe_graph_lookup: _safe_graph_lookup().
  SafeToEditContext.edit_type: SafeToEditContext#edit_type.
  SafeToEditFacts: SafeToEditFacts#
  SafeToEditFacts.dependents: SafeToEditFacts#dependents.
  to_relative: to_relative().
  _resolve_import_spec: _resolve_import_spec().
  SafeToEditContext.graph: SafeToEditContext#graph.
  FileDependencyView._nodes: FileDependencyView#_nodes.
  AgentWorkflowContext.file_path: AgentWorkflowContext#file_path.
  AgentWorkflowContext.edit_type: AgentWorkflowContext#edit_type.
  AgentWorkflowContext.health_grade: AgentWorkflowContext#health_grade.
  SafeToEditFacts.dependencies: SafeToEditFacts#dependencies.
  SafeToEditFacts.test_files: SafeToEditFacts#test_files.
  SafeToEditFacts.risk: SafeToEditFacts#risk.
  _extract_import_specs: _extract_import_specs().
  is_init_file: is_init_file().
  FileDependencyView.has_node: FileDependencyView#has_node().
  FileDependencyView.node_count: FileDependencyView#node_count().
  FileDependencyView.nodes: FileDependencyView#nodes().
  AgentWorkflowContext.test_files: AgentWorkflowContext#test_files.
  AgentWorkflowContext.project_root: AgentWorkflowContext#project_root.
  SafeToEditFacts.has_tests: SafeToEditFacts#has_tests.
  SafeToEditFacts.risk_factors: SafeToEditFacts#risk_factors.
  SafeToEditFacts.pre_edit_checklist: SafeToEditFacts#pre_edit_checklist.
  _risk_to_verdict: _risk_to_verdict().
  _VERDICT_SEVERITY._VERDICT_SEVERITY: _VERDICT_SEVERITY._VERDICT_SEVERITY.
  FileDependencyView._deps: FileDependencyView#_deps.
  FileDependencyView._dependents: FileDependencyView#_dependents.
  _fixture_risk_factor: _fixture_risk_factor().
  _edit_strategy: _edit_strategy().
  _agent_guardrails: _agent_guardrails().
  _DEPENDENCY_SKIP_DIRS: _DEPENDENCY_SKIP_DIRS.
  _DEPENDENCY_SOURCE_EXTS: _DEPENDENCY_SOURCE_EXTS.
  _import_needles_for_target: _import_needles_for_target().
  _matching_node: _matching_node().
  FileDependencyView.__init__: FileDependencyView#__init__().
---
# Module: [`tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py)

## Classes
### `AgentWorkflowContext`
- def: [`tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py:71`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py#L71)
- doc: Inputs needed to build the structured agent edit workflow.
- signature: `class AgentWorkflowContext:`
- members:
  - `edit_type` — [`L76`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py#L76)
  - `file_path` — [`L74`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py#L74)
  - `has_tests` — [`L77`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py#L77)
  - `health_grade` — [`L79`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py#L79)
  - `project_root` — [`L80`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py#L80)
  - `risk` — [`L75`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py#L75)
  - `test_files` — [`L78`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py#L78)
- used by: [`_format_safe_to_edit_result`](safe_to_edit_helpers.md#_format_safe_to_edit_result), [`build_agent_workflow`](safe_to_edit_helpers.md#build_agent_workflow), [`build_agent_summary`](safe_to_edit_helpers.md#build_agent_summary), [`_agent_next_step`](safe_to_edit_helpers.md#_agent_next_step), [`_agent_stop_condition`](safe_to_edit_helpers.md#_agent_stop_condition)

### `FileDependencyView`
- def: [`tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py:37`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py#L37)
- doc: Small graph-like view for one file's immediate import surface.
- signature: `class FileDependencyView:`
- members:
  - `dependencies_of(self, file_rel: str)` — [`L63`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py#L63)
  - `dependents_of(self, file_rel: str)` — [`L66`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py#L66)
  - `has_node(self, file_rel: str)` — [`L51`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py#L51) — Return True if *file_rel* is a node in this view (O(1) set lookup).
  - `node_count(self)` — [`L55`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py#L55) — Return the number of nodes in this view.
  - `nodes(self)` — [`L59`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py#L59) — Return all nodes as a sorted list.
- protocol/private: `__init__`[`L40`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py#L40), `_dependents`[`L49`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py#L49), `_deps`[`L48`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py#L48), `_nodes`[`L47`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py#L47)
- used by: [`build_file_dependency_view`](safe_to_edit_helpers.md#build_file_dependency_view)  (6 test-only)

### `SafeToEditContext`
- def: [`tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py:26`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py#L26)
- doc: Inputs needed to build a safe-to-edit response.
- signature: `class SafeToEditContext:`
- members:
  - `edit_type` — [`L30`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py#L30)
  - `file_path` — [`L29`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py#L29)
  - `graph` — [`L33`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py#L33)
  - `project_root` — [`L32`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py#L32)
  - `resolved_path` — [`L31`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py#L31)
  - `scorer` — [`L34`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py#L34)
- uses (calls/refs, reference-scoped): [`HealthScorer`](../../../health_scorer.md#HealthScorer)
- used by: [`_format_safe_to_edit_result`](safe_to_edit_helpers.md#_format_safe_to_edit_result), [`_collect_safe_to_edit_facts`](safe_to_edit_helpers.md#_collect_safe_to_edit_facts), [`execute`](../safe_to_edit_tool.md#SafeToEditTool.execute), [`_relative_for_constraints`](safe_to_edit_helpers.md#_relative_for_constraints), [`build_safe_to_edit_result`](safe_to_edit_helpers.md#build_safe_to_edit_result)

### `SafeToEditFacts`
- def: [`tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py:84`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py#L84)
- doc: Derived data for a safe-to-edit response.
- signature: `class SafeToEditFacts:`
- members:
  - `dependencies` — [`L88`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py#L88)
  - `dependents` — [`L87`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py#L87)
  - `has_tests` — [`L91`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py#L91)
  - `health` — [`L89`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py#L89)
  - `pre_edit_checklist` — [`L94`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py#L94)
  - `risk` — [`L92`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py#L92)
  - `risk_factors` — [`L93`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py#L93)
  - `test_files` — [`L90`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py#L90)
- used by: [`_format_safe_to_edit_result`](safe_to_edit_helpers.md#_format_safe_to_edit_result), [`_collect_safe_to_edit_facts`](safe_to_edit_helpers.md#_collect_safe_to_edit_facts), [`_format_recommendation`](safe_to_edit_helpers.md#_format_recommendation)

## Functions
- `_agent_guardrails(risk: str, edit_type: str, health_grade: str, has_tests: bool)` — [`L425`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py#L425) — Return concise guardrails for an autonomous edit.
- `_agent_next_step(context: AgentWorkflowContext, workflow: dict[str, Any])` — [`L446`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py#L446) — Return one immediate action for the safe-to-edit decision.
- `_agent_stop_condition(context: AgentWorkflowContext, workflow: dict[str, Any])` — [`L461`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py#L461) — Describe when this edit queue can be considered safe to close.
- `_collect_safe_to_edit_facts(context: SafeToEditContext)` — [`L103`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py#L103) — Collect graph, health, test, and risk facts for a file.
- `_edit_strategy(risk: str, edit_type: str)` — [`L414`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py#L414) — Return a compact edit strategy label for agents.
- `_extract_import_specs(source: str, suffix: str)` — [`L585`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py#L585)
- `_fixture_risk_factor(fact: Any, file_path: str)` — [`L269`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py#L269) — Build a ``risk_factors`` entry for a detected test-fixture file.
- `_format_recommendation(verdict: str, facts: SafeToEditFacts, workflow: dict[str, Any])` — [`L295`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py#L295) — One-line agent-readable summary of what to do next.
- `_format_safe_to_edit_result(context: SafeToEditContext, facts: SafeToEditFacts)` — [`L141`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py#L141) — Format the public safe-to-edit response.
- `_import_needles_for_target(rel_path: str)` — [`L624`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py#L624)
- `_iter_dependency_source_files(root: Path)` — [`L569`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py#L569)
- `_matching_node(graph: Any, rel_path: str)` — [`L668`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py#L668) — Find the graph node matching a relative path.
- `_max_verdict(base: str, override: str | None)` — [`L247`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py#L247) — Return whichever verdict is more severe, preferring the override on ties.
- `_relative_for_constraints(context: SafeToEditContext)` — [`L214`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py#L214) — Return the project-relative path that constraint rows are keyed on.
- `_resolve_import_spec(spec: str, rel_path: str, root: Path)` — [`L598`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py#L598)
- `_risk_to_verdict(risk: str)` — [`L256`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py#L256) — Map ``risk_level`` to the modification_guard verdict vocabulary.
- `_safe_graph_lookup(graph: Any, rel_path: str, lookup: Any)` — [`L655`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py#L655) — Look up graph edges directly or via suffix match.
- `_target_dependencies(target: Path, rel_path: str, root: Path)` — [`L537`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py#L537)
- `_target_dependents(target: Path, rel_path: str, root: Path)` — [`L551`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py#L551)
- `build_agent_summary(context: AgentWorkflowContext, workflow: dict[str, Any], verdict_override: str | None = None)` — [`L326`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py#L326) — Build the compact first-read decision summary for agents.
- `build_agent_workflow(context: AgentWorkflowContext)` — [`L376`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py#L376) — Build a machine-friendly edit workflow for autonomous agents.
- `build_file_dependency_view(resolved_path: str, project_root: str)` — [`L514`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py#L514) — Build a fast graph-like dependency view for one file.
- `build_safe_to_edit_result(context: SafeToEditContext)` — [`L97`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py#L97) — Build the MCP response payload for a safe-to-edit request.
- `is_init_file(file_path: str)` — [`L650`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py#L650) — Return whether a path points at a package __init__.py file.
- `safe_dependencies(graph: Any, rel_path: str)` — [`L645`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py#L645) — Return files rel_path depends on, tolerating stale graph data.
- `safe_dependents(graph: Any, rel_path: str)` — [`L640`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py#L640) — Return files that depend on rel_path, tolerating stale graph data.
- `to_relative(abs_path: str, project_root: str)` — [`L478`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py#L478) — Return a path relative to the project root when possible.

## Module values
- `_DEPENDENCY_SKIP_DIRS` — [`L486`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py#L486)
- `_DEPENDENCY_SOURCE_EXTS` — [`L509`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py#L509)
- `_VERDICT_SEVERITY` — [`L237`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_helpers.py#L237)

