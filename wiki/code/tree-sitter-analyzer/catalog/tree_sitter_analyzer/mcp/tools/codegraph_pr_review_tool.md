---
title: 'Module: tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.codegraph_pr_review_tool`/
symbols:
  CodeGraphPRReviewTool.execute: CodeGraphPRReviewTool#execute().
  CodeGraphPRReviewTool: CodeGraphPRReviewTool#
  CodeGraphPRReviewTool._analyze_call_graph_impact: CodeGraphPRReviewTool#_analyze_call_graph_impact().
  PRReviewResult.to_dict: PRReviewResult#to_dict().
  FileReview.to_dict: FileReview#to_dict().
  _filter_affected_by_language: _filter_affected_by_language().
  CodeGraphPRReviewTool._get_call_graph: CodeGraphPRReviewTool#_get_call_graph().
  _build_recommendations: _build_recommendations().
  CodeGraphPRReviewTool._try_get_cache: CodeGraphPRReviewTool#_try_get_cache().
  _get_local_diff: _get_local_diff().
  CodeGraphPRReviewTool._call_graph: CodeGraphPRReviewTool#_call_graph.
  FileReview: FileReview#
  FileReview.file_path: FileReview#file_path.
  _KNOWN_GENERIC_CALLBACK_NAMES._KNOWN_GENERIC_CALLBACK_NAMES: _KNOWN_GENERIC_CALLBACK_NAMES._KNOWN_GENERIC_CALLBACK_NAMES.
  CodeGraphPRReviewTool._format_response: CodeGraphPRReviewTool#_format_response().
  FileReview.dominant_category: FileReview#dominant_category.
  FileReview.risk_level: FileReview#risk_level.
  FileReview.category_counts: FileReview#category_counts.
  _risk_to_score: _risk_to_score().
  _compute_verdict: _compute_verdict().
  _AMBIGUOUS_NAME_FILE_THRESHOLD: _AMBIGUOUS_NAME_FILE_THRESHOLD.
  FileReview.language: FileReview#language.
  FileReview.change_summary: FileReview#change_summary.
  FileReview.hunk_count: FileReview#hunk_count.
  _score_to_risk: _score_to_risk().
  _branch_diff_base: _branch_diff_base().
  CodeGraphPRReviewTool.get_call_graph: CodeGraphPRReviewTool#get_call_graph().
  PRReviewResult.file_reviews: PRReviewResult#file_reviews.
  _get_old_source: _get_old_source().
  CodeGraphPRReviewTool.__init__: CodeGraphPRReviewTool#__init__().
  CodeGraphPRReviewTool.call_graph_initialized: CodeGraphPRReviewTool#call_graph_initialized().
  FileReview.high_risk_hunks: FileReview#high_risk_hunks.
  _parse_diff_files: _parse_diff_files().
  CodeGraphPRReviewTool._on_project_root_changed: CodeGraphPRReviewTool#_on_project_root_changed().
  CodeGraphPRReviewTool.get_tool_definition: CodeGraphPRReviewTool#get_tool_definition().
  PRReviewResult: PRReviewResult#
  PRReviewResult.files_reviewed: PRReviewResult#files_reviewed.
  PRReviewResult.files_skipped: PRReviewResult#files_skipped.
  PRReviewResult.overall_risk: PRReviewResult#overall_risk.
  PRReviewResult.overall_verdict: PRReviewResult#overall_verdict.
  PRReviewResult.api_changes: PRReviewResult#api_changes.
  PRReviewResult.affected_functions: PRReviewResult#affected_functions.
  PRReviewResult.recommendations: PRReviewResult#recommendations.
  _extract_file_diff: _extract_file_diff().
  _extract_old_new_from_diff: _extract_old_new_from_diff().
  _get_new_source: _get_new_source().
  logger: logger.
  PRReviewResult.phantom_edge_stats: PRReviewResult#phantom_edge_stats.
  CodeGraphPRReviewTool.get_tool_schema: CodeGraphPRReviewTool#get_tool_schema().
  CodeGraphPRReviewTool.validate_arguments: CodeGraphPRReviewTool#validate_arguments().
  _MAX_FILES: _MAX_FILES.
  _current_pr_base: _current_pr_base().
  _git_ref_exists: _git_ref_exists().
  _MAX_HUNKS_DISPLAY: _MAX_HUNKS_DISPLAY.
---
# Module: [`tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.py)

## Classes
### `CodeGraphPRReviewTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.py:365`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.py#L365)
- doc: MCP Tool for AI-powered PR review via AST diff + semantic classify + call graph.
- signature: `class CodeGraphPRReviewTool(BaseMCPTool):`
- members:
  - `_analyze_call_graph_impact(self, changed_files: list[str])` — [`L638`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.py#L638) — Analyze call-graph impact for changed files. — documented in [tree_sitter_analyzer-call_graph](../../../../concepts/tree_sitter_analyzer-call_graph.md)
  - `call_graph_initialized(self)` — [`L406`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.py#L406) — True if the call graph has been lazily initialized (i.e. cached).
  - `execute(self, arguments: dict[str, Any])` — [`L466`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.py#L466) — documented in [tree_sitter_analyzer-ast_diff](../../../../concepts/tree_sitter_analyzer-ast_diff.md)
  - `get_call_graph(self)` — [`L401`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.py#L401) — Public alias for _get_call_graph() — use this instead of accessing _call_graph.
  - `get_tool_definition(self)` — [`L410`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.py#L410)
  - `get_tool_schema(self)` — [`L431`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.py#L431)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L460`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.py#L460)
- protocol/private: `__init__`[`L368`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.py#L368), `_call_graph`[`L369`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.py#L369), `_format_response`[`L750`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.py#L750), `_get_call_graph`[`L390`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.py#L390), `_on_project_root_changed`[`L372`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.py#L372), `_try_get_cache`[`L375`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.py#L375)
- uses (calls/refs, reference-scoped): [`ASTCache`](../../ast_cache.md#ASTCache), [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`FunctionRef`](../../call_graph.md#FunctionRef), [`project_root`](base_tool.md#BaseMCPTool.project_root), [`apply_toon_format_to_response`](../utils/format_helper.md#apply_toon_format_to_response), [`close`](../../ast_cache.md#ASTCache.close), [`CallGraph`](../../call_graph.md#CallGraph), [`build`](../../call_graph.md#CallGraph.build), [`diff_strings`](../../ast_diff.md#ASTDiffer.diff_strings), [`_language_from_ext`](../../project_graph.md#_language_from_ext), [`CachedCallGraph`](../../call_graph.md#CachedCallGraph), [`__init__`](base_tool.md#BaseMCPTool.__init__), [`classify`](../../semantic_change_classifier.md#SemanticChangeClassifier.classify), [`category`](../../semantic_change_classifier.md#ClassifiedHunk.category), [`get_stats`](../../ast_cache.md#ASTCache.get_stats), [`parse_pr_url`](../../pr_url.md#parse_pr_url), [`to_dict`](codegraph_pr_review_tool.md#PRReviewResult.to_dict), [`caller_refs_of`](../../call_graph.md#CallGraph.caller_refs_of), [`qualified_name`](../../call_graph.md#FunctionRef.qualified_name), [`reason`](../../semantic_change_classifier.md#ClassifiedHunk.reason), [`callee_refs_of`](../../call_graph.md#CallGraph.callee_refs_of), [`ASTDiffer`](../../ast_diff.md#ASTDiffer), [`_filter_affected_by_language`](codegraph_pr_review_tool.md#_filter_affected_by_language), [`to_dict`](../../semantic_change_classifier.md#ClassifiedHunk.to_dict), [`function_refs`](../../call_graph.md#CallGraph.function_refs), [`SemanticChangeClassifier`](../../semantic_change_classifier.md#SemanticChangeClassifier), [`language_from_path`](../../_language_family.md#language_from_path), [`_build_recommendations`](codegraph_pr_review_tool.md#_build_recommendations), [`hunks`](../../ast_diff.md#ASTDiffResult.hunks), [`fetch_pr_diff`](../../pr_url.md#fetch_pr_diff), [`dominant_category`](../../semantic_change_classifier.md#SemanticClassification.dominant_category), [`_func_by_file`](../../call_graph.md#CallGraph._func_by_file), [`classifications`](../../semantic_change_classifier.md#SemanticClassification.classifications), [`_get_local_diff`](codegraph_pr_review_tool.md#_get_local_diff), [`check_gh_available`](../../pr_url.md#check_gh_available), [`FileReview`](codegraph_pr_review_tool.md#FileReview), [`_KNOWN_GENERIC_CALLBACK_NAMES`](codegraph_pr_review_tool.md#_KNOWN_GENERIC_CALLBACK_NAMES._KNOWN_GENERIC_CALLBACK_NAMES), [`file_path`](codegraph_pr_review_tool.md#FileReview.file_path), [`risk_level`](../../semantic_change_classifier.md#SemanticClassification.risk_level), [`_compute_verdict`](codegraph_pr_review_tool.md#_compute_verdict)  (+28 more)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`_on_project_root_changed`](base_tool.md#BaseMCPTool._on_project_root_changed), [`build_edit_facade`](edit_facade.md#build_edit_facade), [`_PRReviewViaFacade`](edit_facade.md#build_edit_facade._PRReviewViaFacade), [`execute`](edit_facade.md#build_edit_facade._PRReviewViaFacade.execute)  (35 test-only)

### `FileReview`
- def: [`tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.py:158`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.py#L158)
- signature: `class FileReview:`
- members:
  - `to_dict(self)` — [`L168`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.py#L168)
  - `category_counts` — [`L164`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.py#L164)
  - `change_summary` — [`L163`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.py#L163)
  - `dominant_category` — [`L161`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.py#L161)
  - `file_path` — [`L159`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.py#L159)
  - `high_risk_hunks` — [`L166`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.py#L166)
  - `hunk_count` — [`L165`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.py#L165)
  - `language` — [`L160`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.py#L160)
  - `risk_level` — [`L162`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.py#L162)
- used by: [`execute`](codegraph_pr_review_tool.md#CodeGraphPRReviewTool.execute), [`to_dict`](codegraph_pr_review_tool.md#PRReviewResult.to_dict), [`_build_recommendations`](codegraph_pr_review_tool.md#_build_recommendations), [`file_reviews`](codegraph_pr_review_tool.md#PRReviewResult.file_reviews)  (4 test-only)

### `PRReviewResult`
- def: [`tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.py:185`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.py#L185)
- signature: `class PRReviewResult:`
- members:
  - `to_dict(self)` — [`L201`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.py#L201)
  - `affected_functions` — [`L192`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.py#L192)
  - `api_changes` — [`L191`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.py#L191)
  - `file_reviews` — [`L190`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.py#L190)
  - `files_reviewed` — [`L186`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.py#L186)
  - `files_skipped` — [`L187`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.py#L187)
  - `overall_risk` — [`L188`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.py#L188)
  - `overall_verdict` — [`L189`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.py#L189)
  - `phantom_edge_stats` — [`L194`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.py#L194)
  - `recommendations` — [`L193`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.py#L193)
- uses (calls/refs, reference-scoped): [`to_dict`](codegraph_pr_review_tool.md#FileReview.to_dict), [`FileReview`](codegraph_pr_review_tool.md#FileReview)
- used by: [`execute`](codegraph_pr_review_tool.md#CodeGraphPRReviewTool.execute)  (1 test-only)

## Functions
- `_branch_diff_base(project_root: str)` — [`L252`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.py#L252)
- `_build_recommendations(file_reviews: list[FileReview], api_changes: list[str], affected_functions: list[dict[str, Any]])` — [`L784`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.py#L784)
- `_compute_verdict(overall_risk: str, api_changes: int, affected_funcs: int)` — [`L758`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.py#L758) — Map PR risk to the project's canonical verdict vocabulary.
- `_current_pr_base(project_root: str)` — [`L263`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.py#L263)
- `_extract_file_diff(diff_text: str, file_path: str)` — [`L308`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.py#L308)
- `_extract_old_new_from_diff(file_diff: str)` — [`L323`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.py#L323)
- `_filter_affected_by_language(candidates: list[dict], changed_languages: set[str], name_file_count: dict[str, int])` — [`L70`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.py#L70) — Filter call-graph edges to remove cross-language phantoms and ambiguous bare names.
- `_get_local_diff(mode: str, project_root: str | None)` — [`L229`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.py#L229)
- `_get_new_source(project_root: str, file_path: str)` — [`L357`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.py#L357)
- `_get_old_source(project_root: str, file_path: str)` — [`L339`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.py#L339)
- `_git_ref_exists(project_root: str, ref: str)` — [`L279`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.py#L279)
- `_parse_diff_files(diff_text: str)` — [`L298`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.py#L298)
- `_risk_to_score(risk: str)` — [`L215`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.py#L215)
- `_score_to_risk(score: float)` — [`L219`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.py#L219)

## Module values
- `_AMBIGUOUS_NAME_FILE_THRESHOLD` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.py#L48)
- `_KNOWN_GENERIC_CALLBACK_NAMES` — [`L54`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.py#L54)
- `_MAX_FILES` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.py#L36)
- `_MAX_HUNKS_DISPLAY` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.py#L37)
- `logger` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_pr_review_tool.py#L34)

