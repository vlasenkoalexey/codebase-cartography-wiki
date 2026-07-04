---
title: 'Module: tests/unit/mcp/test_runtime_guidance_facade_names.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_runtime_guidance_facade_names.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_runtime_guidance_facade_names`/
symbols:
  test_tool_routing_entry_is_callable: test_tool_routing_entry_is_callable().
  _Score.dimensions: _Score#dimensions.
  _forbidden_calls_in: _forbidden_calls_in().
  _FORBIDDEN._FORBIDDEN: _FORBIDDEN._FORBIDDEN.
  _forbidden_words_in: _forbidden_words_in().
  TestSmartWorkflowHint.test_smart_prompts_no_legacy_names: TestSmartWorkflowHint#test_smart_prompts_no_legacy_names().
  TestSmartWorkflowHint.test_smart_prompts_response_builders_produce_clean_text: TestSmartWorkflowHint#test_smart_prompts_response_builders_produce_clean_text().
  TestErrorRecoverySuggestedTool.test_error_recovery_hint_texts_no_legacy_names: TestErrorRecoverySuggestedTool#test_error_recovery_hint_texts_no_legacy_names().
  TestSearchSymbolNextStep.test_symbol_search_next_step_no_legacy: TestSearchSymbolNextStep#test_symbol_search_next_step_no_legacy().
  TestBuildSmartHintFacadeNames.test_overview_include_health_smart_hint_no_legacy: TestBuildSmartHintFacadeNames#test_overview_include_health_smart_hint_no_legacy().
  TestBuildSmartHintFacadeNames._assert_clean: TestBuildSmartHintFacadeNames#_assert_clean().
  _parse_routing_snippet: _parse_routing_snippet().
  TestToolRoutingFacadeNames.test_tool_routing_no_legacy_names: TestToolRoutingFacadeNames#test_tool_routing_no_legacy_names().
  TestSmartWorkflowHint.test_health_opt_in_hint_no_legacy_names: TestSmartWorkflowHint#test_health_opt_in_hint_no_legacy_names().
  TestErrorRecoverySuggestedTool.test_file_not_found_suggested_tool_is_facade: TestErrorRecoverySuggestedTool#test_file_not_found_suggested_tool_is_facade().
  TestErrorRecoverySuggestedTool.test_no_such_file_suggested_tool_is_facade: TestErrorRecoverySuggestedTool#test_no_such_file_suggested_tool_is_facade().
  TestSearchSymbolNextStep.test_symbol_search_next_step_exact_facade_form: TestSearchSymbolNextStep#test_symbol_search_next_step_exact_facade_form().
  TestBuildSmartHintFacadeNames.test_healthy_project_no_legacy: TestBuildSmartHintFacadeNames#test_healthy_project_no_legacy().
  TestBuildSmartHintFacadeNames.test_unhealthy_project_no_legacy: TestBuildSmartHintFacadeNames#test_unhealthy_project_no_legacy().
  TestBuildSmartHintFacadeNames.test_analyze_part_uses_facade_form: TestBuildSmartHintFacadeNames#test_analyze_part_uses_facade_form().
  TestBuildSmartHintFacadeNames.test_retrieve_part_uses_facade_form: TestBuildSmartHintFacadeNames#test_retrieve_part_uses_facade_form().
  TestBuildSmartHintFacadeNames.test_suggest_refactor_action_no_legacy: TestBuildSmartHintFacadeNames#test_suggest_refactor_action_no_legacy().
  _get_facade: _get_facade().
  _routing_cases: _routing_cases().
  _LEGACY_NAMES_SET._LEGACY_NAMES_SET: _LEGACY_NAMES_SET._LEGACY_NAMES_SET.
  _SMART_HINT_LEGACY: _SMART_HINT_LEGACY.
  TestToolRoutingFacadeNames.test_tool_routing_values_use_facade_action_form: TestToolRoutingFacadeNames#test_tool_routing_values_use_facade_action_form().
  TestSmartWorkflowHint.test_health_opt_in_hint_uses_facade_form: TestSmartWorkflowHint#test_health_opt_in_hint_uses_facade_form().
  TestProjectHealthToolGuidance.test_recommended_mcp_command_facade_form: TestProjectHealthToolGuidance#test_recommended_mcp_command_facade_form().
  TestProjectHealthToolGuidance.test_safety_mcp_command_facade_form: TestProjectHealthToolGuidance#test_safety_mcp_command_facade_form().
  test_file_action_c_grade_without_weakest_dimension: test_file_action_c_grade_without_weakest_dimension().
  TestProjectHealthToolGuidance.test_recommended_mcp_command_facade_form._Score: TestProjectHealthToolGuidance#test_recommended_mcp_command_facade_form()._Score#
  _FACADE_BUILDERS._FACADE_BUILDERS: _FACADE_BUILDERS._FACADE_BUILDERS.
  _CALL_RE: _CALL_RE.
  TestProjectHealthToolGuidance.test_safety_mcp_command_facade_form._Score: TestProjectHealthToolGuidance#test_safety_mcp_command_facade_form()._Score#
  _ACTION_FORM_RE: _ACTION_FORM_RE.
  _NAMED_PARAM_RE: _NAMED_PARAM_RE.
  _get_inner_schema: _get_inner_schema().
  _EXTRA_FORBIDDEN._EXTRA_FORBIDDEN: _EXTRA_FORBIDDEN._EXTRA_FORBIDDEN.
  _OUTPUT_CONTROL_PARAMS._OUTPUT_CONTROL_PARAMS: _OUTPUT_CONTROL_PARAMS._OUTPUT_CONTROL_PARAMS.
  TestToolRoutingFacadeNames: TestToolRoutingFacadeNames#
  TestSmartWorkflowHint: TestSmartWorkflowHint#
  TestErrorRecoverySuggestedTool: TestErrorRecoverySuggestedTool#
  TestSearchSymbolNextStep: TestSearchSymbolNextStep#
  TestProjectHealthToolGuidance: TestProjectHealthToolGuidance#
  TestProjectHealthToolGuidance.test_recommended_mcp_command_facade_form._Score.__init__: TestProjectHealthToolGuidance#test_recommended_mcp_command_facade_form()._Score#__init__().
  _Score.grade: _Score#grade.
  _Score.file_path: _Score#file_path.
  TestProjectHealthToolGuidance.test_safety_mcp_command_facade_form._Score.__init__: TestProjectHealthToolGuidance#test_safety_mcp_command_facade_form()._Score#__init__().
  _Score.total: _Score#total.
  TestBuildSmartHintFacadeNames: TestBuildSmartHintFacadeNames#
---
# Module: [`tests/unit/mcp/test_runtime_guidance_facade_names.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_runtime_guidance_facade_names.py)

## Classes
### `TestBuildSmartHintFacadeNames`
- def: [`tests/unit/mcp/test_runtime_guidance_facade_names.py:369`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_runtime_guidance_facade_names.py#L369)
- doc: P2-3 ratchet: _build_smart_hint output must not contain legacy tool names.
- signature: `class TestBuildSmartHintFacadeNames:`
- members:
  - `test_analyze_part_uses_facade_form(self)` — [`L401`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_runtime_guidance_facade_names.py#L401) — The SMART Analyze part must teach structure action=analyze.
  - `test_healthy_project_no_legacy(self)` — [`L378`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_runtime_guidance_facade_names.py#L378)
  - `test_overview_include_health_smart_hint_no_legacy(self, tmp_path)` — [`L437`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_runtime_guidance_facade_names.py#L437) — End-to-end: overview include_health=true smart_workflow_hint must be clean.
  - `test_retrieve_part_uses_facade_form(self)` — [`L412`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_runtime_guidance_facade_names.py#L412) — The SMART Retrieve part must teach structure action=read.
  - `test_suggest_refactor_action_no_legacy(self)` — [`L423`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_runtime_guidance_facade_names.py#L423) — _suggest_refactor_action for a large prod file must use facade form.
  - `test_unhealthy_project_no_legacy(self)` — [`L386`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_runtime_guidance_facade_names.py#L386) — The REFACTOR branch must not produce check_file_health or analyze_code_structure.
- protocol/private: `_assert_clean`[`L372`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_runtime_guidance_facade_names.py#L372)
- uses (calls/refs, reference-scoped): [`ProjectOverviewTool`](../../../tree_sitter_analyzer/mcp/tools/project_overview_tool.md#ProjectOverviewTool), [`execute`](../../../tree_sitter_analyzer/mcp/tools/project_overview_tool.md#ProjectOverviewTool.execute), [`_build_smart_hint`](../../../tree_sitter_analyzer/mcp/tools/project_overview_tool.md#_build_smart_hint), [`_suggest_refactor_action`](../../../tree_sitter_analyzer/mcp/tools/project_overview_tool.md#_suggest_refactor_action)  (1 test-only)

### `TestErrorRecoverySuggestedTool`
- def: [`tests/unit/mcp/test_runtime_guidance_facade_names.py:209`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_runtime_guidance_facade_names.py#L209)
- signature: `class TestErrorRecoverySuggestedTool:`
- members:
  - `test_error_recovery_hint_texts_no_legacy_names(self)` — [`L240`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_runtime_guidance_facade_names.py#L240) — All recovery hint text strings in _ERROR_RECOVERY_HINTS must be clean.
  - `test_file_not_found_suggested_tool_is_facade(self)` — [`L210`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_runtime_guidance_facade_names.py#L210) — file_not_found recovery hint must suggest a facade name, not list_files.
  - `test_no_such_file_suggested_tool_is_facade(self)` — [`L226`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_runtime_guidance_facade_names.py#L226) — 'no such file' recovery hint must suggest a facade name.
- uses (calls/refs, reference-scoped): [`build_agent_friendly_error`](../../../tree_sitter_analyzer/mcp/server_utils/error_recovery.md#build_agent_friendly_error), [`_ERROR_RECOVERY_HINTS`](../../../tree_sitter_analyzer/mcp/server_utils/error_recovery.md#_ERROR_RECOVERY_HINTS._ERROR_RECOVERY_HINTS)  (2 test-only)

### `TestProjectHealthToolGuidance`
- def: [`tests/unit/mcp/test_runtime_guidance_facade_names.py:308`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_runtime_guidance_facade_names.py#L308)
- signature: `class TestProjectHealthToolGuidance:`
- members:
  - `test_recommended_mcp_command_facade_form(self)` — [`L309`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_runtime_guidance_facade_names.py#L309) — _file_action() must return facade form commands.
  - `test_safety_mcp_command_facade_form(self)` — [`L334`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_runtime_guidance_facade_names.py#L334) — _build_agent_backlog_item() safety_mcp_command must use facade form.
- uses (calls/refs, reference-scoped): [`_build_agent_backlog`](../../../tree_sitter_analyzer/mcp/tools/project_health_tool.md#_build_agent_backlog), [`_file_action`](../../../tree_sitter_analyzer/mcp/tools/project_health_tool.md#_file_action)

### `TestSearchSymbolNextStep`
- def: [`tests/unit/mcp/test_runtime_guidance_facade_names.py:261`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_runtime_guidance_facade_names.py#L261)
- signature: `class TestSearchSymbolNextStep:`
- members:
  - `test_symbol_search_next_step_exact_facade_form(self)` — [`L287`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_runtime_guidance_facade_names.py#L287) — The next_step builder must produce the facade call form string.
  - `test_symbol_search_next_step_no_legacy(self, tmp_path)` — [`L262`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_runtime_guidance_facade_names.py#L262) — search action=symbol next_step must not say 'codegraph_explore'.
- uses (calls/refs, reference-scoped): [`CodeGraphSymbolSearchTool`](../../../tree_sitter_analyzer/mcp/tools/symbol_search_tool.md#CodeGraphSymbolSearchTool), [`execute`](../../../tree_sitter_analyzer/mcp/tools/symbol_search_tool.md#CodeGraphSymbolSearchTool.execute)  (1 test-only)

### `TestSmartWorkflowHint`
- def: [`tests/unit/mcp/test_runtime_guidance_facade_names.py:155`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_runtime_guidance_facade_names.py#L155)
- signature: `class TestSmartWorkflowHint:`
- members:
  - `test_health_opt_in_hint_no_legacy_names(self)` — [`L156`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_runtime_guidance_facade_names.py#L156) — _health_opt_in_hint() must not teach get_project_overview.
  - `test_health_opt_in_hint_uses_facade_form(self)` — [`L164`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_runtime_guidance_facade_names.py#L164) — _health_opt_in_hint() must reference the facade call form.
  - `test_smart_prompts_no_legacy_names(self)` — [`L170`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_runtime_guidance_facade_names.py#L170) — smart_prompts.py instruction templates must not teach legacy names.
  - `test_smart_prompts_response_builders_produce_clean_text(self)` — [`L182`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_runtime_guidance_facade_names.py#L182) — build_smart_analyze_response / build_smart_explore_response facade names.
- uses (calls/refs, reference-scoped): [`build_smart_analyze_response`](../../../tree_sitter_analyzer/mcp/server_utils/smart_prompts.md#build_smart_analyze_response), [`build_smart_explore_response`](../../../tree_sitter_analyzer/mcp/server_utils/smart_prompts.md#build_smart_explore_response), [`_health_opt_in_hint`](../../../tree_sitter_analyzer/mcp/tools/project_overview_tool.md#_health_opt_in_hint), [`_ANALYZE_INSTRUCTIONS_TEMPLATE`](../../../tree_sitter_analyzer/mcp/server_utils/smart_prompts.md#_ANALYZE_INSTRUCTIONS_TEMPLATE), [`_EXPLORE_INSTRUCTIONS_TEMPLATE`](../../../tree_sitter_analyzer/mcp/server_utils/smart_prompts.md#_EXPLORE_INSTRUCTIONS_TEMPLATE)  (1 test-only)

### `TestToolRoutingFacadeNames`
- def: [`tests/unit/mcp/test_runtime_guidance_facade_names.py:101`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_runtime_guidance_facade_names.py#L101)
- signature: `class TestToolRoutingFacadeNames:`
- members:
  - `test_tool_routing_no_legacy_names(self)` — [`L102`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_runtime_guidance_facade_names.py#L102) — Every value in _build_tool_routing() must use facade form only.
  - `test_tool_routing_values_use_facade_action_form(self)` — [`L115`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_runtime_guidance_facade_names.py#L115) — At least the high-traffic routing keys must use facade action= form.
- uses (calls/refs, reference-scoped): [`_build_tool_routing`](../../../tree_sitter_analyzer/mcp/tools/project_overview_tool.md#_build_tool_routing)  (1 test-only)

### `_Score`
- def: [`tests/unit/mcp/test_runtime_guidance_facade_names.py:340`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_runtime_guidance_facade_names.py#L340)
- signature: `class _Score:`
- members:
  - `dimensions` — [`L317`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_runtime_guidance_facade_names.py#L317)
  - `file_path` — [`L316`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_runtime_guidance_facade_names.py#L316)
  - `grade` — [`L315`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_runtime_guidance_facade_names.py#L315)
  - `total` — [`L344`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_runtime_guidance_facade_names.py#L344)
- protocol/private: `__init__`[`L314`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_runtime_guidance_facade_names.py#L314), `__init__`[`L341`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_runtime_guidance_facade_names.py#L341)
- uses (calls/refs, reference-scoped): [`_build_agent_backlog`](../../../tree_sitter_analyzer/mcp/tools/project_health_tool.md#_build_agent_backlog), [`_file_action`](../../../tree_sitter_analyzer/mcp/tools/project_health_tool.md#_file_action)  (2 test-only)

## Functions
- `_forbidden_calls_in(text: str)` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_runtime_guidance_facade_names.py#L73) — Return list of forbidden legacy tool names found as call sites in text.
- `_forbidden_words_in(text: str, *, extras: frozenset[str] = frozenset())` — [`L83`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_runtime_guidance_facade_names.py#L83) — Return list of forbidden legacy tool names found as bare words in text.
- `_get_facade(facade_name: str)` — [`L528`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_runtime_guidance_facade_names.py#L528) — Lazily build a facade (with project_root=None) for schema inspection.
- `_get_inner_schema(facade: object, action: str)` — [`L539`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_runtime_guidance_facade_names.py#L539) — Return the inner tool's schema for a given action, or None.
- `_parse_routing_snippet(snippet: str)` — [`L515`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_runtime_guidance_facade_names.py#L515) — Parse 'facade action=X param=... param2=...' → (facade, action, [param,...]).
- `_routing_cases()` — [`L556`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_runtime_guidance_facade_names.py#L556)
- `test_file_action_c_grade_without_weakest_dimension()` — [`L604`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_runtime_guidance_facade_names.py#L604) — C grade with no weakest dimension → bare health action=file form.
- `test_tool_routing_entry_is_callable(routing_key: str, snippet: str)` — [`L561`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_runtime_guidance_facade_names.py#L561) — Callability ratchet: every tool_routing entry must be a valid facade call.

## Module values
- `_ACTION_FORM_RE` — [`L506`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_runtime_guidance_facade_names.py#L506)
- `_CALL_RE` — [`L70`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_runtime_guidance_facade_names.py#L70)
- `_EXTRA_FORBIDDEN` — [`L57`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_runtime_guidance_facade_names.py#L57)
- `_FACADE_BUILDERS` — [`L495`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_runtime_guidance_facade_names.py#L495)
- `_FORBIDDEN` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_runtime_guidance_facade_names.py#L65)
- `_LEGACY_NAMES_SET` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_runtime_guidance_facade_names.py#L53)
- `_NAMED_PARAM_RE` — [`L512`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_runtime_guidance_facade_names.py#L512)
- `_OUTPUT_CONTROL_PARAMS` — [`L481`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_runtime_guidance_facade_names.py#L481)
- `_SMART_HINT_LEGACY` — [`L364`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_runtime_guidance_facade_names.py#L364)

