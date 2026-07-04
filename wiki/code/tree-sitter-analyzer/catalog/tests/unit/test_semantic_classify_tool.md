---
title: 'Module: tests/unit/test_semantic_classify_tool.py'
type: catalog
provenance: extracted
module: tests/unit/test_semantic_classify_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_semantic_classify_tool`/
symbols:
  _run: _run().
  TestClassifiedHunkSerializerOptIn._make_classified_hunk: TestClassifiedHunkSerializerOptIn#_make_classified_hunk().
  TestClassifiedHunkSerializerOptIn.test_semantic_classification_to_dict_default_is_lean: TestClassifiedHunkSerializerOptIn#test_semantic_classification_to_dict_default_is_lean().
  TestClassifiedHunkSerializerOptIn.test_semantic_classification_to_dict_opt_in_delivers_children: TestClassifiedHunkSerializerOptIn#test_semantic_classification_to_dict_opt_in_delivers_children().
  TestClassifyByteBudget.test_default_classifications_have_no_ast_children: TestClassifyByteBudget#test_default_classifications_have_no_ast_children().
  TestClassifyByteBudget.test_default_response_exact_bytes_string_mode: TestClassifyByteBudget#test_default_response_exact_bytes_string_mode().
  TestClassifyByteBudget.test_default_response_has_verdict_and_summary_fields: TestClassifyByteBudget#test_default_response_has_verdict_and_summary_fields().
  TestClassifyByteBudget.test_truncation_honesty_fields_when_capped: TestClassifyByteBudget#test_truncation_honesty_fields_when_capped().
  TestClassifyByteBudget.test_include_ast_nodes_opt_in_adds_hunk_detail: TestClassifyByteBudget#test_include_ast_nodes_opt_in_adds_hunk_detail().
  _SRC_V1: _SRC_V1.
  _SRC_V2: _SRC_V2.
  TestSemanticClassifyToolDefinition.test_tool_name: TestSemanticClassifyToolDefinition#test_tool_name().
  TestSemanticClassifyToolDefinition.test_mode_is_optional_in_schema: TestSemanticClassifyToolDefinition#test_mode_is_optional_in_schema().
  TestSemanticClassifyToolDefinition.test_resolve_mode_defaults: TestSemanticClassifyToolDefinition#test_resolve_mode_defaults().
  TestSemanticClassifyToolDefinition.test_file_path_only_does_not_demand_sources: TestSemanticClassifyToolDefinition#test_file_path_only_does_not_demand_sources().
  TestSemanticClassifyValidation.test_classify_file_requires_path: TestSemanticClassifyValidation#test_classify_file_requires_path().
  TestSemanticClassifyValidation.test_classify_string_requires_sources: TestSemanticClassifyValidation#test_classify_string_requires_sources().
  TestSemanticClassifyValidation.test_classify_string_requires_language: TestSemanticClassifyValidation#test_classify_string_requires_language().
  TestSemanticClassifyValidation.test_valid_classify_file: TestSemanticClassifyValidation#test_valid_classify_file().
  TestSemanticClassifyExecution.test_classify_string_function_added: TestSemanticClassifyExecution#test_classify_string_function_added().
  TestSemanticClassifyExecution.test_classify_string_signature_changed: TestSemanticClassifyExecution#test_classify_string_signature_changed().
  TestSemanticClassifyExecution.test_classify_string_no_changes: TestSemanticClassifyExecution#test_classify_string_no_changes().
  TestSemanticClassifyExecution.test_classify_string_function_removed: TestSemanticClassifyExecution#test_classify_string_function_removed().
  TestSemanticClassifyExecution.test_classify_string_import_change: TestSemanticClassifyExecution#test_classify_string_import_change().
  TestSemanticClassifyExecution.test_classify_string_body_change: TestSemanticClassifyExecution#test_classify_string_body_change().
  TestSemanticClassifyExecution.test_toon_format: TestSemanticClassifyExecution#test_toon_format().
  git_repo_with_two_commits: git_repo_with_two_commits().
  TestClassifyByteBudget.test_schema_has_include_ast_nodes_param: TestClassifyByteBudget#test_schema_has_include_ast_nodes_param().
  TestClassifyByteBudget.test_schema_has_hunk_cap_param: TestClassifyByteBudget#test_schema_has_hunk_cap_param().
  TestClassifyByteBudget.test_default_response_leq_raw_diff_bytes_git_mode: TestClassifyByteBudget#test_default_response_leq_raw_diff_bytes_git_mode().
  TestClassifyByteBudget.test_include_ast_nodes_delivers_children_in_hunk_nodes: TestClassifyByteBudget#test_include_ast_nodes_delivers_children_in_hunk_nodes().
  tool: tool().
  TestSemanticClassifyToolRegistry.test_tool_registered: TestSemanticClassifyToolRegistry#test_tool_registered().
  TestSemanticClassifyToolRegistry.test_tool_in_cli_class_names: TestSemanticClassifyToolRegistry#test_tool_in_cli_class_names().
  TestSemanticClassifyChangeImpactIntegration.test_change_impact_includes_semantic_when_changed: TestSemanticClassifyChangeImpactIntegration#test_change_impact_includes_semantic_when_changed().
  TestSemanticClassifyChangeImpactIntegration.test_classify_changed_files_empty: TestSemanticClassifyChangeImpactIntegration#test_classify_changed_files_empty().
  TestCompactHelpers.test_compact_classification_passthrough_when_include_ast_nodes: TestCompactHelpers#test_compact_classification_passthrough_when_include_ast_nodes().
  TestCompactHelpers.test_compact_classification_returns_entry_when_hunk_not_dict: TestCompactHelpers#test_compact_classification_returns_entry_when_hunk_not_dict().
  TestCompactHelpers.test_compact_hunk_strips_children_from_old_and_new: TestCompactHelpers#test_compact_hunk_strips_children_from_old_and_new().
  TestCompactHelpers.test_compact_hunk_passthrough_non_old_new_keys: TestCompactHelpers#test_compact_hunk_passthrough_non_old_new_keys().
  TestCompactHelpers.test_compact_hunk_old_new_non_dict_passthrough: TestCompactHelpers#test_compact_hunk_old_new_non_dict_passthrough().
  TestClassifiedHunkSerializerOptIn.test_classified_hunk_to_dict_default_is_lean: TestClassifiedHunkSerializerOptIn#test_classified_hunk_to_dict_default_is_lean().
  TestClassifiedHunkSerializerOptIn.test_classified_hunk_to_dict_opt_in_delivers_children: TestClassifiedHunkSerializerOptIn#test_classified_hunk_to_dict_opt_in_delivers_children().
  TestSemanticClassifyToolDefinition: TestSemanticClassifyToolDefinition#
  TestSemanticClassifyValidation: TestSemanticClassifyValidation#
  TestSemanticClassifyExecution: TestSemanticClassifyExecution#
  TestSemanticClassifyToolRegistry: TestSemanticClassifyToolRegistry#
  TestSemanticClassifyChangeImpactIntegration: TestSemanticClassifyChangeImpactIntegration#
  TestCompactHelpers: TestCompactHelpers#
  TestClassifyByteBudget: TestClassifyByteBudget#
  TestClassifiedHunkSerializerOptIn: TestClassifiedHunkSerializerOptIn#
---
# Module: [`tests/unit/test_semantic_classify_tool.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_classify_tool.py)

## Classes
### `TestClassifiedHunkSerializerOptIn`
- def: [`tests/unit/test_semantic_classify_tool.py:669`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_classify_tool.py#L669)
- doc: BUG A (Codex P2 #696 follow-up): ClassifiedHunk.to_dict() must accept
- signature: `class TestClassifiedHunkSerializerOptIn:`
- members:
  - `_make_classified_hunk(self)` — [`L675`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_classify_tool.py#L675) — Return a real ClassifiedHunk with a hunk whose old/new nodes have children.
  - `test_classified_hunk_to_dict_default_is_lean(self)` — [`L693`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_classify_tool.py#L693) — ClassifiedHunk.to_dict() with no args must NOT include children keys.
  - `test_classified_hunk_to_dict_opt_in_delivers_children(self)` — [`L714`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_classify_tool.py#L714) — ClassifiedHunk.to_dict(include_children=True) must still deliver children.
  - `test_semantic_classification_to_dict_default_is_lean(self)` — [`L732`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_classify_tool.py#L732) — SemanticClassification.to_dict() must thread include_children=False to each ClassifiedHunk.
  - `test_semantic_classification_to_dict_opt_in_delivers_children(self)` — [`L755`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_classify_tool.py#L755) — SemanticClassification.to_dict(include_children=True) must deliver children.
- uses (calls/refs, reference-scoped): [`diff_strings`](../../tree_sitter_analyzer/ast_diff.md#ASTDiffer.diff_strings), [`classify`](../../tree_sitter_analyzer/semantic_change_classifier.md#SemanticChangeClassifier.classify), [`to_dict`](../../tree_sitter_analyzer/semantic_change_classifier.md#SemanticClassification.to_dict), [`ASTDiffer`](../../tree_sitter_analyzer/ast_diff.md#ASTDiffer), [`SemanticChangeClassifier`](../../tree_sitter_analyzer/semantic_change_classifier.md#SemanticChangeClassifier), [`classifications`](../../tree_sitter_analyzer/semantic_change_classifier.md#SemanticClassification.classifications)

### `TestClassifyByteBudget`
- def: [`tests/unit/test_semantic_classify_tool.py:409`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_classify_tool.py#L409)
- doc: #528 — default response must not inline full AST subtrees.
- signature: `class TestClassifyByteBudget:`
- members:
  - `test_default_classifications_have_no_ast_children(self, tool: SemanticClassifyTool)` — [`L430`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_classify_tool.py#L430) — By default, each entry in classifications must not contain hunk.old/new children.
  - `test_default_response_exact_bytes_string_mode(self, tool: SemanticClassifyTool)` — [`L460`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_classify_tool.py#L460) — Exact byte pin (string mode, deterministic fixture).
  - `test_default_response_has_verdict_and_summary_fields(self, tool: SemanticClassifyTool)` — [`L531`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_classify_tool.py#L531) — Default response must carry verdict, dominant_category, risk_level, change_summary,
  - `test_default_response_leq_raw_diff_bytes_git_mode(self, tool: SemanticClassifyTool, git_repo_with_two_commits)` — [`L494`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_classify_tool.py#L494) — Differential invariant (git mode): default classify_file response ≤ raw git diff bytes.
  - `test_include_ast_nodes_delivers_children_in_hunk_nodes(self, tool: SemanticClassifyTool)` — [`L609`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_classify_tool.py#L609) — Regression for #694 follow-up: include_ast_nodes=True must deliver
  - `test_include_ast_nodes_opt_in_adds_hunk_detail(self, tool: SemanticClassifyTool)` — [`L583`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_classify_tool.py#L583) — With include_ast_nodes=True, hunk.old/new details appear in classifications.
  - `test_schema_has_hunk_cap_param(self, tool: SemanticClassifyTool)` — [`L422`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_classify_tool.py#L422) — hunk_cap opt-in must be declared in schema, not required.
  - `test_schema_has_include_ast_nodes_param(self, tool: SemanticClassifyTool)` — [`L412`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_classify_tool.py#L412) — include_ast_nodes opt-in must be declared in schema, not required.
  - `test_truncation_honesty_fields_when_capped(self, tool: SemanticClassifyTool)` — [`L561`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_classify_tool.py#L561) — When hunk_cap limits the output, truncated/listed_cap/next_step must appear.
- uses (calls/refs, reference-scoped): [`SemanticClassifyTool`](../../tree_sitter_analyzer/mcp/tools/semantic_classify_tool.md#SemanticClassifyTool), [`get_tool_schema`](../../tree_sitter_analyzer/mcp/tools/semantic_classify_tool.md#SemanticClassifyTool.get_tool_schema)  (3 test-only)

### `TestCompactHelpers`
- def: [`tests/unit/test_semantic_classify_tool.py:345`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_classify_tool.py#L345)
- doc: Unit tests for _compact_classification / _compact_hunk helpers (#528).
- signature: `class TestCompactHelpers:`
- members:
  - `test_compact_classification_passthrough_when_include_ast_nodes(self)` — [`L348`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_classify_tool.py#L348)
  - `test_compact_classification_returns_entry_when_hunk_not_dict(self)` — [`L360`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_classify_tool.py#L360) — Covers the defensive branch when hunk is None or missing.
  - `test_compact_hunk_old_new_non_dict_passthrough(self)` — [`L398`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_classify_tool.py#L398) — When old/new value is not a dict, pass it through unchanged.
  - `test_compact_hunk_passthrough_non_old_new_keys(self)` — [`L389`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_classify_tool.py#L389)
  - `test_compact_hunk_strips_children_from_old_and_new(self)` — [`L374`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_classify_tool.py#L374)
- uses (calls/refs, reference-scoped): [`_compact_hunk`](../../tree_sitter_analyzer/mcp/tools/semantic_classify_tool.md#_compact_hunk), [`_compact_classification`](../../tree_sitter_analyzer/mcp/tools/semantic_classify_tool.md#_compact_classification)

### `TestSemanticClassifyChangeImpactIntegration`
- def: [`tests/unit/test_semantic_classify_tool.py:195`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_classify_tool.py#L195)
- signature: `class TestSemanticClassifyChangeImpactIntegration:`
- members:
  - `test_change_impact_includes_semantic_when_changed(self, tmp_path)` — [`L196`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_classify_tool.py#L196)
  - `test_classify_changed_files_empty(self)` — [`L210`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_classify_tool.py#L210)
- uses (calls/refs, reference-scoped): [`_classify_changed_files`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.md#_classify_changed_files)

### `TestSemanticClassifyExecution`
- def: [`tests/unit/test_semantic_classify_tool.py:77`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_classify_tool.py#L77)
- signature: `class TestSemanticClassifyExecution:`
- members:
  - `test_classify_string_body_change(self, tool: SemanticClassifyTool)` — [`L149`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_classify_tool.py#L149)
  - `test_classify_string_function_added(self, tool: SemanticClassifyTool)` — [`L78`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_classify_tool.py#L78)
  - `test_classify_string_function_removed(self, tool: SemanticClassifyTool)` — [`L123`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_classify_tool.py#L123)
  - `test_classify_string_import_change(self, tool: SemanticClassifyTool)` — [`L136`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_classify_tool.py#L136)
  - `test_classify_string_no_changes(self, tool: SemanticClassifyTool)` — [`L110`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_classify_tool.py#L110)
  - `test_classify_string_signature_changed(self, tool: SemanticClassifyTool)` — [`L93`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_classify_tool.py#L93)
  - `test_toon_format(self, tool: SemanticClassifyTool)` — [`L162`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_classify_tool.py#L162)
- uses (calls/refs, reference-scoped): [`SemanticClassifyTool`](../../tree_sitter_analyzer/mcp/tools/semantic_classify_tool.md#SemanticClassifyTool)  (1 test-only)

### `TestSemanticClassifyToolDefinition`
- def: [`tests/unit/test_semantic_classify_tool.py:22`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_classify_tool.py#L22)
- signature: `class TestSemanticClassifyToolDefinition:`
- members:
  - `test_file_path_only_does_not_demand_sources(self, tool: SemanticClassifyTool)` — [`L48`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_classify_tool.py#L48)
  - `test_mode_is_optional_in_schema(self, tool: SemanticClassifyTool)` — [`L27`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_classify_tool.py#L27)
  - `test_resolve_mode_defaults(self, tool: SemanticClassifyTool)` — [`L35`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_classify_tool.py#L35)
  - `test_tool_name(self, tool: SemanticClassifyTool)` — [`L23`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_classify_tool.py#L23)
- uses (calls/refs, reference-scoped): [`SemanticClassifyTool`](../../tree_sitter_analyzer/mcp/tools/semantic_classify_tool.md#SemanticClassifyTool), [`validate_arguments`](../../tree_sitter_analyzer/mcp/tools/semantic_classify_tool.md#SemanticClassifyTool.validate_arguments), [`_resolve_mode`](../../tree_sitter_analyzer/mcp/tools/semantic_classify_tool.md#SemanticClassifyTool._resolve_mode), [`get_tool_schema`](../../tree_sitter_analyzer/mcp/tools/semantic_classify_tool.md#SemanticClassifyTool.get_tool_schema), [`get_tool_definition`](../../tree_sitter_analyzer/mcp/tools/semantic_classify_tool.md#SemanticClassifyTool.get_tool_definition)

### `TestSemanticClassifyToolRegistry`
- def: [`tests/unit/test_semantic_classify_tool.py:176`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_classify_tool.py#L176)
- signature: `class TestSemanticClassifyToolRegistry:`
- members:
  - `test_tool_in_cli_class_names(self)` — [`L189`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_classify_tool.py#L189)
  - `test_tool_registered(self)` — [`L177`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_classify_tool.py#L177)
- uses (calls/refs, reference-scoped): [`create_tool_registry`](../../tree_sitter_analyzer/mcp/_tool_registry.md#create_tool_registry), [`_TOOL_CLASS_NAMES`](../../tree_sitter_analyzer/cli/commands/mcp_commands/__init__.md#_TOOL_CLASS_NAMES._TOOL_CLASS_NAMES)

### `TestSemanticClassifyValidation`
- def: [`tests/unit/test_semantic_classify_tool.py:54`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_classify_tool.py#L54)
- signature: `class TestSemanticClassifyValidation:`
- members:
  - `test_classify_file_requires_path(self, tool: SemanticClassifyTool)` — [`L55`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_classify_tool.py#L55)
  - `test_classify_string_requires_language(self, tool: SemanticClassifyTool)` — [`L63`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_classify_tool.py#L63)
  - `test_classify_string_requires_sources(self, tool: SemanticClassifyTool)` — [`L59`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_classify_tool.py#L59)
  - `test_valid_classify_file(self, tool: SemanticClassifyTool)` — [`L73`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_classify_tool.py#L73)
- uses (calls/refs, reference-scoped): [`SemanticClassifyTool`](../../tree_sitter_analyzer/mcp/tools/semantic_classify_tool.md#SemanticClassifyTool), [`validate_arguments`](../../tree_sitter_analyzer/mcp/tools/semantic_classify_tool.md#SemanticClassifyTool.validate_arguments)

## Functions
- `_run(tool_instance: SemanticClassifyTool, args: dict[str, Any])` — [`L18`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_classify_tool.py#L18)
- `git_repo_with_two_commits(tmp_path)` — [`L290`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_classify_tool.py#L290) — Minimal git repo with a before/after commit so classify_file can run.
- `tool()` — [`L14`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_classify_tool.py#L14)

## Module values
- `_SRC_V1` — [`L223`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_classify_tool.py#L223)
- `_SRC_V2` — [`L252`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_classify_tool.py#L252)

