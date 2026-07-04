---
title: 'Module: tests/unit/cli/test_mcp_commands.py'
type: catalog
provenance: extracted
module: tests/unit/cli/test_mcp_commands.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.cli.test_mcp_commands`/
symbols:
  _args: _args().
  test_mcp_cli_commands_delegate_to_matching_tool: test_mcp_cli_commands_delegate_to_matching_tool().
  test_safe_to_edit_cli_forwards_requested_edit_type: test_safe_to_edit_cli_forwards_requested_edit_type().
  test_project_health_cli_forwards_requested_max_files: test_project_health_cli_forwards_requested_max_files().
  test_parser_readiness_cli_forwards_language_option: test_parser_readiness_cli_forwards_language_option().
  test_safe_to_edit_cli_falls_back_to_schema_default_for_legacy_namespaces: test_safe_to_edit_cli_falls_back_to_schema_default_for_legacy_namespaces().
  test_project_scoped_dependency_modes_do_not_require_file_path: test_project_scoped_dependency_modes_do_not_require_file_path().
  test_mcp_cli_toon_output_prints_tool_toon_content: test_mcp_cli_toon_output_prints_tool_toon_content().
  test_change_impact_cli_forwards_scope_paths: test_change_impact_cli_forwards_scope_paths().
  test_change_impact_cli_forwards_scope_mode_strict: test_change_impact_cli_forwards_scope_mode_strict().
  test_change_impact_cli_forwards_resource_profile: test_change_impact_cli_forwards_resource_profile().
  test_change_impact_cli_forwards_agent_summary_only: test_change_impact_cli_forwards_agent_summary_only().
  test_change_impact_cli_forwards_mode_and_test_discovery_toggle: test_change_impact_cli_forwards_mode_and_test_discovery_toggle().
  test_change_impact_cli_forwards_change_impact_full: test_change_impact_cli_forwards_change_impact_full().
  test_change_impact_fail_on_risk_exits_1_on_caution_verdict: test_change_impact_fail_on_risk_exits_1_on_caution_verdict().
  test_change_impact_fail_on_risk_exits_0_below_threshold: test_change_impact_fail_on_risk_exits_0_below_threshold().
  test_change_impact_fail_on_risk_unsafe_only_exits_1_for_unsafe: test_change_impact_fail_on_risk_unsafe_only_exits_1_for_unsafe().
  test_change_impact_fail_on_risk_unsafe_exits_0_for_caution: test_change_impact_fail_on_risk_unsafe_exits_0_for_caution().
  test_change_impact_no_fail_on_risk_exits_0_on_any_verdict: test_change_impact_no_fail_on_risk_exits_0_on_any_verdict().
  test_change_impact_fail_on_risk_review_exits_1_for_warn: test_change_impact_fail_on_risk_review_exits_1_for_warn().
  test_change_impact_fail_on_risk_review_exits_0_for_caution: test_change_impact_fail_on_risk_review_exits_0_for_caution().
  test_callers_cli_delegates_to_callers_tool: test_callers_cli_delegates_to_callers_tool().
  test_callees_cli_delegates_to_callees_tool: test_callees_cli_delegates_to_callees_tool().
  test_symbol_resolve_cli_delegates_to_resolve_tool: test_symbol_resolve_cli_delegates_to_resolve_tool().
  test_compact_toon_cli_flag_forwards_compact_only: test_compact_toon_cli_flag_forwards_compact_only().
  test_file_scoped_mcp_cli_commands_require_file_path: test_file_scoped_mcp_cli_commands_require_file_path().
  test_change_impact_cli_does_not_require_file_path: test_change_impact_cli_does_not_require_file_path().
  MCP_COMMAND_FLAGS: MCP_COMMAND_FLAGS.
  test_mcp_cli_commands_delegate_to_matching_tool.FakeTool: test_mcp_cli_commands_delegate_to_matching_tool().FakeTool#
  test_safe_to_edit_cli_forwards_requested_edit_type.FakeSafeToEditTool: test_safe_to_edit_cli_forwards_requested_edit_type().FakeSafeToEditTool#
  test_project_health_cli_forwards_requested_max_files.FakeProjectHealthTool: test_project_health_cli_forwards_requested_max_files().FakeProjectHealthTool#
  test_parser_readiness_cli_forwards_language_option.FakeParserReadinessTool: test_parser_readiness_cli_forwards_language_option().FakeParserReadinessTool#
  test_safe_to_edit_cli_falls_back_to_schema_default_for_legacy_namespaces.FakeSafeToEditTool: test_safe_to_edit_cli_falls_back_to_schema_default_for_legacy_namespaces().FakeSafeToEditTool#
  test_project_scoped_dependency_modes_do_not_require_file_path.FakeDependencyAnalysisTool: test_project_scoped_dependency_modes_do_not_require_file_path().FakeDependencyAnalysisTool#
  test_mcp_cli_toon_output_prints_tool_toon_content.FakeProjectOverviewTool: test_mcp_cli_toon_output_prints_tool_toon_content().FakeProjectOverviewTool#
  test_change_impact_cli_does_not_require_file_path.FakeChangeImpactTool: test_change_impact_cli_does_not_require_file_path().FakeChangeImpactTool#
  test_change_impact_cli_forwards_scope_paths.FakeChangeImpactTool: test_change_impact_cli_forwards_scope_paths().FakeChangeImpactTool#
  test_change_impact_cli_forwards_scope_mode_strict.FakeChangeImpactTool: test_change_impact_cli_forwards_scope_mode_strict().FakeChangeImpactTool#
  test_change_impact_cli_forwards_resource_profile.FakeChangeImpactTool: test_change_impact_cli_forwards_resource_profile().FakeChangeImpactTool#
  test_change_impact_cli_forwards_agent_summary_only.FakeChangeImpactTool: test_change_impact_cli_forwards_agent_summary_only().FakeChangeImpactTool#
  test_change_impact_cli_forwards_mode_and_test_discovery_toggle.FakeChangeImpactTool: test_change_impact_cli_forwards_mode_and_test_discovery_toggle().FakeChangeImpactTool#
  test_change_impact_cli_forwards_change_impact_full.FakeChangeImpactTool: test_change_impact_cli_forwards_change_impact_full().FakeChangeImpactTool#
  test_change_impact_fail_on_risk_exits_1_on_caution_verdict.FakeChangeImpactTool: test_change_impact_fail_on_risk_exits_1_on_caution_verdict().FakeChangeImpactTool#
  test_change_impact_fail_on_risk_exits_0_below_threshold.FakeChangeImpactTool: test_change_impact_fail_on_risk_exits_0_below_threshold().FakeChangeImpactTool#
  test_change_impact_fail_on_risk_unsafe_only_exits_1_for_unsafe.FakeChangeImpactTool: test_change_impact_fail_on_risk_unsafe_only_exits_1_for_unsafe().FakeChangeImpactTool#
  test_change_impact_fail_on_risk_unsafe_exits_0_for_caution.FakeChangeImpactTool: test_change_impact_fail_on_risk_unsafe_exits_0_for_caution().FakeChangeImpactTool#
  test_change_impact_no_fail_on_risk_exits_0_on_any_verdict.FakeChangeImpactTool: test_change_impact_no_fail_on_risk_exits_0_on_any_verdict().FakeChangeImpactTool#
  test_change_impact_fail_on_risk_review_exits_1_for_warn.FakeChangeImpactTool: test_change_impact_fail_on_risk_review_exits_1_for_warn().FakeChangeImpactTool#
  test_change_impact_fail_on_risk_review_exits_0_for_caution.FakeChangeImpactTool: test_change_impact_fail_on_risk_review_exits_0_for_caution().FakeChangeImpactTool#
  test_callers_cli_delegates_to_callers_tool.FakeCallersTool: test_callers_cli_delegates_to_callers_tool().FakeCallersTool#
  test_callees_cli_delegates_to_callees_tool.FakeCalleesTool: test_callees_cli_delegates_to_callees_tool().FakeCalleesTool#
  test_symbol_resolve_cli_delegates_to_resolve_tool.FakeResolveTool: test_symbol_resolve_cli_delegates_to_resolve_tool().FakeResolveTool#
  test_compact_toon_cli_flag_forwards_compact_only.FakeFileHealthTool: test_compact_toon_cli_flag_forwards_compact_only().FakeFileHealthTool#
  test_mcp_cli_commands_delegate_to_matching_tool.FakeTool.__init__: test_mcp_cli_commands_delegate_to_matching_tool().FakeTool#__init__().
  test_mcp_cli_commands_delegate_to_matching_tool.FakeTool.execute: test_mcp_cli_commands_delegate_to_matching_tool().FakeTool#execute().
  test_safe_to_edit_cli_forwards_requested_edit_type.FakeSafeToEditTool.__init__: test_safe_to_edit_cli_forwards_requested_edit_type().FakeSafeToEditTool#__init__().
  test_safe_to_edit_cli_forwards_requested_edit_type.FakeSafeToEditTool.execute: test_safe_to_edit_cli_forwards_requested_edit_type().FakeSafeToEditTool#execute().
  test_project_health_cli_forwards_requested_max_files.FakeProjectHealthTool.__init__: test_project_health_cli_forwards_requested_max_files().FakeProjectHealthTool#__init__().
  test_project_health_cli_forwards_requested_max_files.FakeProjectHealthTool.execute: test_project_health_cli_forwards_requested_max_files().FakeProjectHealthTool#execute().
  test_parser_readiness_cli_forwards_language_option.FakeParserReadinessTool.__init__: test_parser_readiness_cli_forwards_language_option().FakeParserReadinessTool#__init__().
  test_parser_readiness_cli_forwards_language_option.FakeParserReadinessTool.execute: test_parser_readiness_cli_forwards_language_option().FakeParserReadinessTool#execute().
  test_safe_to_edit_cli_falls_back_to_schema_default_for_legacy_namespaces.FakeSafeToEditTool.__init__: test_safe_to_edit_cli_falls_back_to_schema_default_for_legacy_namespaces().FakeSafeToEditTool#__init__().
  test_safe_to_edit_cli_falls_back_to_schema_default_for_legacy_namespaces.FakeSafeToEditTool.execute: test_safe_to_edit_cli_falls_back_to_schema_default_for_legacy_namespaces().FakeSafeToEditTool#execute().
  test_project_scoped_dependency_modes_do_not_require_file_path.FakeDependencyAnalysisTool.__init__: test_project_scoped_dependency_modes_do_not_require_file_path().FakeDependencyAnalysisTool#__init__().
  test_project_scoped_dependency_modes_do_not_require_file_path.FakeDependencyAnalysisTool.execute: test_project_scoped_dependency_modes_do_not_require_file_path().FakeDependencyAnalysisTool#execute().
  test_mcp_cli_toon_output_prints_tool_toon_content.FakeProjectOverviewTool.__init__: test_mcp_cli_toon_output_prints_tool_toon_content().FakeProjectOverviewTool#__init__().
  test_mcp_cli_toon_output_prints_tool_toon_content.FakeProjectOverviewTool.execute: test_mcp_cli_toon_output_prints_tool_toon_content().FakeProjectOverviewTool#execute().
  test_change_impact_cli_does_not_require_file_path.FakeChangeImpactTool.__init__: test_change_impact_cli_does_not_require_file_path().FakeChangeImpactTool#__init__().
  test_change_impact_cli_does_not_require_file_path.FakeChangeImpactTool.execute: test_change_impact_cli_does_not_require_file_path().FakeChangeImpactTool#execute().
  test_change_impact_cli_forwards_scope_paths.FakeChangeImpactTool.__init__: test_change_impact_cli_forwards_scope_paths().FakeChangeImpactTool#__init__().
  test_change_impact_cli_forwards_scope_paths.FakeChangeImpactTool.execute: test_change_impact_cli_forwards_scope_paths().FakeChangeImpactTool#execute().
  test_change_impact_cli_forwards_scope_mode_strict.FakeChangeImpactTool.__init__: test_change_impact_cli_forwards_scope_mode_strict().FakeChangeImpactTool#__init__().
  test_change_impact_cli_forwards_scope_mode_strict.FakeChangeImpactTool.execute: test_change_impact_cli_forwards_scope_mode_strict().FakeChangeImpactTool#execute().
  test_change_impact_cli_forwards_resource_profile.FakeChangeImpactTool.__init__: test_change_impact_cli_forwards_resource_profile().FakeChangeImpactTool#__init__().
  test_change_impact_cli_forwards_resource_profile.FakeChangeImpactTool.execute: test_change_impact_cli_forwards_resource_profile().FakeChangeImpactTool#execute().
  test_change_impact_cli_forwards_agent_summary_only.FakeChangeImpactTool.__init__: test_change_impact_cli_forwards_agent_summary_only().FakeChangeImpactTool#__init__().
  test_change_impact_cli_forwards_agent_summary_only.FakeChangeImpactTool.execute: test_change_impact_cli_forwards_agent_summary_only().FakeChangeImpactTool#execute().
  test_change_impact_cli_forwards_mode_and_test_discovery_toggle.FakeChangeImpactTool.__init__: test_change_impact_cli_forwards_mode_and_test_discovery_toggle().FakeChangeImpactTool#__init__().
  test_change_impact_cli_forwards_mode_and_test_discovery_toggle.FakeChangeImpactTool.execute: test_change_impact_cli_forwards_mode_and_test_discovery_toggle().FakeChangeImpactTool#execute().
  test_change_impact_cli_forwards_change_impact_full.FakeChangeImpactTool.__init__: test_change_impact_cli_forwards_change_impact_full().FakeChangeImpactTool#__init__().
  test_change_impact_cli_forwards_change_impact_full.FakeChangeImpactTool.execute: test_change_impact_cli_forwards_change_impact_full().FakeChangeImpactTool#execute().
  test_change_impact_fail_on_risk_exits_1_on_caution_verdict.FakeChangeImpactTool.__init__: test_change_impact_fail_on_risk_exits_1_on_caution_verdict().FakeChangeImpactTool#__init__().
  test_change_impact_fail_on_risk_exits_1_on_caution_verdict.FakeChangeImpactTool.execute: test_change_impact_fail_on_risk_exits_1_on_caution_verdict().FakeChangeImpactTool#execute().
  test_change_impact_fail_on_risk_exits_0_below_threshold.FakeChangeImpactTool.__init__: test_change_impact_fail_on_risk_exits_0_below_threshold().FakeChangeImpactTool#__init__().
  test_change_impact_fail_on_risk_exits_0_below_threshold.FakeChangeImpactTool.execute: test_change_impact_fail_on_risk_exits_0_below_threshold().FakeChangeImpactTool#execute().
  test_change_impact_fail_on_risk_unsafe_only_exits_1_for_unsafe.FakeChangeImpactTool.__init__: test_change_impact_fail_on_risk_unsafe_only_exits_1_for_unsafe().FakeChangeImpactTool#__init__().
  test_change_impact_fail_on_risk_unsafe_only_exits_1_for_unsafe.FakeChangeImpactTool.execute: test_change_impact_fail_on_risk_unsafe_only_exits_1_for_unsafe().FakeChangeImpactTool#execute().
  test_change_impact_fail_on_risk_unsafe_exits_0_for_caution.FakeChangeImpactTool.__init__: test_change_impact_fail_on_risk_unsafe_exits_0_for_caution().FakeChangeImpactTool#__init__().
  test_change_impact_fail_on_risk_unsafe_exits_0_for_caution.FakeChangeImpactTool.execute: test_change_impact_fail_on_risk_unsafe_exits_0_for_caution().FakeChangeImpactTool#execute().
  test_change_impact_no_fail_on_risk_exits_0_on_any_verdict.FakeChangeImpactTool.__init__: test_change_impact_no_fail_on_risk_exits_0_on_any_verdict().FakeChangeImpactTool#__init__().
  test_change_impact_no_fail_on_risk_exits_0_on_any_verdict.FakeChangeImpactTool.execute: test_change_impact_no_fail_on_risk_exits_0_on_any_verdict().FakeChangeImpactTool#execute().
  test_change_impact_fail_on_risk_review_exits_1_for_warn.FakeChangeImpactTool.__init__: test_change_impact_fail_on_risk_review_exits_1_for_warn().FakeChangeImpactTool#__init__().
  test_change_impact_fail_on_risk_review_exits_1_for_warn.FakeChangeImpactTool.execute: test_change_impact_fail_on_risk_review_exits_1_for_warn().FakeChangeImpactTool#execute().
  test_change_impact_fail_on_risk_review_exits_0_for_caution.FakeChangeImpactTool.__init__: test_change_impact_fail_on_risk_review_exits_0_for_caution().FakeChangeImpactTool#__init__().
  test_change_impact_fail_on_risk_review_exits_0_for_caution.FakeChangeImpactTool.execute: test_change_impact_fail_on_risk_review_exits_0_for_caution().FakeChangeImpactTool#execute().
  test_callers_cli_delegates_to_callers_tool.FakeCallersTool.__init__: test_callers_cli_delegates_to_callers_tool().FakeCallersTool#__init__().
  test_callers_cli_delegates_to_callers_tool.FakeCallersTool.execute: test_callers_cli_delegates_to_callers_tool().FakeCallersTool#execute().
  test_callees_cli_delegates_to_callees_tool.FakeCalleesTool.__init__: test_callees_cli_delegates_to_callees_tool().FakeCalleesTool#__init__().
  test_callees_cli_delegates_to_callees_tool.FakeCalleesTool.execute: test_callees_cli_delegates_to_callees_tool().FakeCalleesTool#execute().
  test_symbol_resolve_cli_delegates_to_resolve_tool.FakeResolveTool.__init__: test_symbol_resolve_cli_delegates_to_resolve_tool().FakeResolveTool#__init__().
  test_symbol_resolve_cli_delegates_to_resolve_tool.FakeResolveTool.execute: test_symbol_resolve_cli_delegates_to_resolve_tool().FakeResolveTool#execute().
  test_compact_toon_cli_flag_forwards_compact_only.FakeFileHealthTool.__init__: test_compact_toon_cli_flag_forwards_compact_only().FakeFileHealthTool#__init__().
  test_compact_toon_cli_flag_forwards_compact_only.FakeFileHealthTool.execute: test_compact_toon_cli_flag_forwards_compact_only().FakeFileHealthTool#execute().
---
# Module: [`tests/unit/cli/test_mcp_commands.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py)

## Classes
### `FakeCalleesTool`
- def: [`tests/unit/cli/test_mcp_commands.py:905`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L905)
- signature: `class FakeCalleesTool:`
- members:
  - `execute(self, arguments: dict[str, Any])` — [`L909`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L909)
- protocol/private: `__init__`[`L906`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L906)
- used by: (1 test-only callers)

### `FakeCallersTool`
- def: [`tests/unit/cli/test_mcp_commands.py:873`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L873)
- signature: `class FakeCallersTool:`
- members:
  - `execute(self, arguments: dict[str, Any])` — [`L877`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L877)
- protocol/private: `__init__`[`L874`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L874)
- used by: (1 test-only callers)

### `FakeChangeImpactTool`
- def: [`tests/unit/cli/test_mcp_commands.py:851`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L851)
- signature: `class FakeChangeImpactTool:`
- members:
  - `execute(self, arguments: dict[str, Any])` — [`L447`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L447)
  - `execute(self, arguments: dict[str, Any])` — [`L496`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L496)
  - `execute(self, arguments: dict[str, Any])` — [`L544`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L544)
  - `execute(self, arguments: dict[str, Any])` — [`L574`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L574)
  - `execute(self, arguments: dict[str, Any])` — [`L601`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L601)
  - `execute(self, arguments: dict[str, Any])` — [`L638`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L638)
  - `execute(self, arguments: dict[str, Any])` — [`L686`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L686)
  - `execute(self, arguments: dict[str, Any])` — [`L723`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L723)
  - `execute(self, arguments: dict[str, Any])` — [`L745`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L745)
  - `execute(self, arguments: dict[str, Any])` — [`L767`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L767)
  - `execute(self, arguments: dict[str, Any])` — [`L789`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L789)
  - `execute(self, arguments: dict[str, Any])` — [`L811`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L811)
  - `execute(self, arguments: dict[str, Any])` — [`L833`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L833)
  - `execute(self, arguments: dict[str, Any])` — [`L855`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L855)
- protocol/private: `__init__`[`L444`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L444), `__init__`[`L493`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L493), `__init__`[`L541`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L541), `__init__`[`L571`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L571), `__init__`[`L598`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L598), `__init__`[`L635`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L635), `__init__`[`L683`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L683), `__init__`[`L720`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L720), `__init__`[`L742`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L742), `__init__`[`L764`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L764), `__init__`[`L786`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L786), `__init__`[`L808`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L808), `__init__`[`L830`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L830), `__init__`[`L852`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L852)
- used by: (1 test-only callers)

### `FakeDependencyAnalysisTool`
- def: [`tests/unit/cli/test_mcp_commands.py:388`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L388)
- signature: `class FakeDependencyAnalysisTool:`
- members:
  - `execute(self, arguments: dict[str, Any])` — [`L392`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L392)
- protocol/private: `__init__`[`L389`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L389)
- used by: (1 test-only callers)

### `FakeFileHealthTool`
- def: [`tests/unit/cli/test_mcp_commands.py:969`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L969)
- signature: `class FakeFileHealthTool:`
- members:
  - `execute(self, arguments: dict[str, Any])` — [`L973`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L973)
- protocol/private: `__init__`[`L970`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L970)
- used by: (1 test-only callers)

### `FakeParserReadinessTool`
- def: [`tests/unit/cli/test_mcp_commands.py:275`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L275)
- signature: `class FakeParserReadinessTool:`
- members:
  - `execute(self, arguments: dict[str, Any])` — [`L279`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L279)
- protocol/private: `__init__`[`L276`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L276)
- used by: (1 test-only callers)

### `FakeProjectHealthTool`
- def: [`tests/unit/cli/test_mcp_commands.py:243`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L243)
- signature: `class FakeProjectHealthTool:`
- members:
  - `execute(self, arguments: dict[str, Any])` — [`L247`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L247)
- protocol/private: `__init__`[`L244`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L244)
- used by: (1 test-only callers)

### `FakeProjectOverviewTool`
- def: [`tests/unit/cli/test_mcp_commands.py:415`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L415)
- signature: `class FakeProjectOverviewTool:`
- members:
  - `execute(self, arguments: dict[str, Any])` — [`L419`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L419)
- protocol/private: `__init__`[`L416`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L416)
- used by: (1 test-only callers)

### `FakeResolveTool`
- def: [`tests/unit/cli/test_mcp_commands.py:937`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L937)
- signature: `class FakeResolveTool:`
- members:
  - `execute(self, arguments: dict[str, Any])` — [`L941`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L941)
- protocol/private: `__init__`[`L938`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L938)
- used by: (1 test-only callers)

### `FakeSafeToEditTool`
- def: [`tests/unit/cli/test_mcp_commands.py:313`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L313)
- signature: `class FakeSafeToEditTool:`
- members:
  - `execute(self, arguments: dict[str, Any])` — [`L215`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L215)
  - `execute(self, arguments: dict[str, Any])` — [`L317`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L317)
- protocol/private: `__init__`[`L212`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L212), `__init__`[`L314`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L314)
- used by: (1 test-only callers)

### `FakeTool`
- def: [`tests/unit/cli/test_mcp_commands.py:179`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L179)
- signature: `class FakeTool:`
- members:
  - `execute(self, arguments: dict[str, Any])` — [`L183`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L183)
- protocol/private: `__init__`[`L180`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L180)
- used by: (1 test-only callers)

## Functions
- `_args(**overrides: Any)` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L30)
- `test_callees_cli_delegates_to_callees_tool(monkeypatch)` — [`L902`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L902)
- `test_callers_cli_delegates_to_callers_tool(monkeypatch)` — [`L870`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L870)
- `test_change_impact_cli_does_not_require_file_path(monkeypatch)` — [`L440`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L440)
- `test_change_impact_cli_forwards_agent_summary_only(monkeypatch)` — [`L594`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L594)
- `test_change_impact_cli_forwards_change_impact_full(monkeypatch)` — [`L673`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L673) — ``--change-impact-full`` flips agent_summary_only back to False.
- `test_change_impact_cli_forwards_mode_and_test_discovery_toggle(monkeypatch)` — [`L631`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L631)
- `test_change_impact_cli_forwards_resource_profile(monkeypatch)` — [`L566`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L566) — Local resource profile must reach the MCP change-impact tool.
- `test_change_impact_cli_forwards_scope_mode_strict(monkeypatch)` — [`L536`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L536) — #8 CLI parity: --change-impact-scope-mode strict reaches the MCP tool.
- `test_change_impact_cli_forwards_scope_paths(monkeypatch)` — [`L489`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L489)
- `test_change_impact_fail_on_risk_exits_0_below_threshold(monkeypatch)` — [`L738`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L738) — --change-impact-fail-on-risk caution: exit 0 when verdict is INFO (below threshold).
- `test_change_impact_fail_on_risk_exits_1_on_caution_verdict(monkeypatch)` — [`L716`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L716) — --change-impact-fail-on-risk caution: exit 1 when verdict is CAUTION.
- `test_change_impact_fail_on_risk_review_exits_0_for_caution(monkeypatch)` — [`L848`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L848) — --change-impact-fail-on-risk review: CAUTION (below REVIEW) must exit 0.
- `test_change_impact_fail_on_risk_review_exits_1_for_warn(monkeypatch)` — [`L826`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L826) — --change-impact-fail-on-risk review: WARN (above REVIEW) must exit 1.
- `test_change_impact_fail_on_risk_unsafe_exits_0_for_caution(monkeypatch)` — [`L782`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L782) — --change-impact-fail-on-risk unsafe: exit 0 for CAUTION (below UNSAFE threshold).
- `test_change_impact_fail_on_risk_unsafe_only_exits_1_for_unsafe(monkeypatch)` — [`L760`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L760) — --change-impact-fail-on-risk unsafe: exit 1 only when verdict is UNSAFE.
- `test_change_impact_no_fail_on_risk_exits_0_on_any_verdict(monkeypatch)` — [`L804`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L804) — Without --change-impact-fail-on-risk, any verdict exits 0 on success.
- `test_compact_toon_cli_flag_forwards_compact_only(monkeypatch)` — [`L965`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L965) — RFC-0012 CLI parity: --compact-toon reaches the MCP compact_only arg.
- `test_file_scoped_mcp_cli_commands_require_file_path(flag_overrides: dict[str, Any], expected_error: str)` — [`L354`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L354)
- `test_mcp_cli_commands_delegate_to_matching_tool(monkeypatch, flag_overrides: dict[str, Any], tool_attr: str, expected_tool_args: dict[str, Any])` — [`L171`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L171)
- `test_mcp_cli_toon_output_prints_tool_toon_content(monkeypatch, capsys)` — [`L414`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L414)
- `test_parser_readiness_cli_forwards_language_option(monkeypatch)` — [`L272`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L272)
- `test_project_health_cli_forwards_requested_max_files(monkeypatch)` — [`L240`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L240)
- `test_project_scoped_dependency_modes_do_not_require_file_path(monkeypatch, mode: str, expected_mode: str)` — [`L381`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L381)
- `test_safe_to_edit_cli_falls_back_to_schema_default_for_legacy_namespaces(monkeypatch)` — [`L308`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L308)
- `test_safe_to_edit_cli_forwards_requested_edit_type(monkeypatch)` — [`L208`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L208)
- `test_symbol_resolve_cli_delegates_to_resolve_tool(monkeypatch)` — [`L934`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L934)

## Module values
- `MCP_COMMAND_FLAGS` — [`L12`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_mcp_commands.py#L12)

