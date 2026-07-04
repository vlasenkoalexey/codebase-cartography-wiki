---
title: 'Module: tests/unit/test_uml_state.py'
type: catalog
provenance: extracted
module: tests/unit/test_uml_state.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_uml_state`/
symbols:
  _make_ts_node: _make_ts_node().
  test_execute_state_diagram_success.FakeExporter.state_diagram: test_execute_state_diagram_success().FakeExporter#state_diagram().
  test_execute_state_diagram_not_found_missing_file.FakeExporter.state_diagram: test_execute_state_diagram_not_found_missing_file().FakeExporter#state_diagram().
  test_qualified_enum_base_states_and_transitions: test_qualified_enum_base_states_and_transitions().
  test_build_state_result_parse_failed: test_build_state_result_parse_failed().
  test_state_result_dataclass_exists: test_state_result_dataclass_exists().
  test_render_state_mermaid_transition_with_label: test_render_state_mermaid_transition_with_label().
  test_assignment_transitions_detected_door_controller: test_assignment_transitions_detected_door_controller().
  test_execute_state_diagram_success: test_execute_state_diagram_success().
  test_second_enum_transitions_found_when_first_enum_has_none: test_second_enum_transitions_found_when_first_enum_has_none().
  test_find_return_enum_ref_assignment_branch_via_integration: test_find_return_enum_ref_assignment_branch_via_integration().
  test_multi_enum_both_have_transitions_aggregated_and_deduped: test_multi_enum_both_have_transitions_aggregated_and_deduped().
  test_state_transition_dataclass_exists: test_state_transition_dataclass_exists().
  test_state_transition_label_defaults_empty: test_state_transition_label_defaults_empty().
  test_build_state_result_missing_file_returns_not_found: test_build_state_result_missing_file_returns_not_found().
  test_build_state_result_transition_sources_and_targets: test_build_state_result_transition_sources_and_targets().
  test_build_state_result_no_match_zero_transitions: test_build_state_result_no_match_zero_transitions().
  test_render_state_mermaid_transition_edge: test_render_state_mermaid_transition_edge().
  test_execute_state_diagram_not_found_missing_file: test_execute_state_diagram_not_found_missing_file().
  test_info_zero_transition_state_diagram_no_initial_edges: test_info_zero_transition_state_diagram_no_initial_edges().
  test_info_zero_transition_state_diagram_mermaid_starts_with_header: test_info_zero_transition_state_diagram_mermaid_starts_with_header().
  test_multi_enum_no_transitions_falls_back_to_all_members: test_multi_enum_no_transitions_falls_back_to_all_members().
  test_case_pattern_fallback_exercises_node_text_path: test_case_pattern_fallback_exercises_node_text_path().
  test_dotted_name_direct_source_member: test_dotted_name_direct_source_member().
  test_parse_file_for_state_calls_parser_once: test_parse_file_for_state_calls_parser_once().
  test_build_state_result_finds_enum_members: test_build_state_result_finds_enum_members().
  test_build_state_result_class_name_filter: test_build_state_result_class_name_filter().
  test_build_state_result_max_nodes_truncates: test_build_state_result_max_nodes_truncates().
  test_build_state_result_match_transitions_detected: test_build_state_result_match_transitions_detected().
  test_state_diagram_mermaid_type: test_state_diagram_mermaid_type().
  test_state_diagram_diagram_type: test_state_diagram_diagram_type().
  test_state_diagram_analysis_kind_metadata: test_state_diagram_analysis_kind_metadata().
  test_state_diagram_note_in_metadata: test_state_diagram_note_in_metadata().
  test_state_diagram_zero_transitions_info: test_state_diagram_zero_transitions_info().
  test_state_diagram_missing_file_not_found: test_state_diagram_missing_file_not_found().
  test_state_diagram_mermaid_starts_stateDiagram_with_transitions: test_state_diagram_mermaid_starts_stateDiagram_with_transitions().
  test_state_diagram_node_count_exact_no_transitions: test_state_diagram_node_count_exact_no_transitions().
  test_state_diagram_exact_node_count_with_transitions: test_state_diagram_exact_node_count_with_transitions().
  test_assignment_transitions_combined_with_return: test_assignment_transitions_combined_with_return().
  test_uml_max_nodes_cli_mcp_default_parity: test_uml_max_nodes_cli_mcp_default_parity().
  test_state_diagram_true_not_found_zero_states: test_state_diagram_true_not_found_zero_states().
  test_state_diagram_non_python_file_not_found_mentions_language: test_state_diagram_non_python_file_not_found_mentions_language().
  test_extract_enum_members_includes_lowercase: test_extract_enum_members_includes_lowercase().
  test_enum_with_method_body_still_extracts_members: test_enum_with_method_body_still_extracts_members().
  test_enum_with_docstring_skips_non_assignment_expressions: test_enum_with_docstring_skips_non_assignment_expressions().
  test_build_state_result_ignores_underscore_prefixed_members: test_build_state_result_ignores_underscore_prefixed_members().
  test_multi_enum_dedup_members_preserves_unique: test_multi_enum_dedup_members_preserves_unique().
  test_build_state_result_real_file_no_enum: test_build_state_result_real_file_no_enum().
  test_build_state_result_state_names_correct: test_build_state_result_state_names_correct().
  test_build_state_result_class_name_not_found: test_build_state_result_class_name_not_found().
  test_state_in_diagram_enum: test_state_in_diagram_enum().
  test_uml_tool_schema_lists_diagrams_with_state: test_uml_tool_schema_lists_diagrams_with_state().
  test_state_diagram_validate_arguments_accepts_state: test_state_diagram_validate_arguments_accepts_state().
  test_state_diagram_validate_arguments_rejects_unknown: test_state_diagram_validate_arguments_rejects_unknown().
  test_node_text_raw_none_returns_empty: test_node_text_raw_none_returns_empty().
  test_node_text_exception_returns_empty: test_node_text_exception_returns_empty().
  test_node_text_long_string_truncated: test_node_text_long_string_truncated().
  test_iter_case_clauses_direct_child_fallback: test_iter_case_clauses_direct_child_fallback().
  test_extract_enum_members_with_empty_lhs_children_skipped: test_extract_enum_members_with_empty_lhs_children_skipped().
  test_extract_enum_members_with_non_identifier_lhs_skipped: test_extract_enum_members_with_non_identifier_lhs_skipped().
  test_iter_case_clauses_block_with_non_case_clause_child: test_iter_case_clauses_block_with_non_case_clause_child().
  test_parse_enum_ref_no_match_returns_none: test_parse_enum_ref_no_match_returns_none().
  test_dotted_name_non_matching_source_skipped: test_dotted_name_non_matching_source_skipped().
  test_find_return_enum_ref_assignment_with_eq_first_reversed: test_find_return_enum_ref_assignment_with_eq_first_reversed().
  test_find_return_enum_ref_assignment_non_matching_rhs_breaks: test_find_return_enum_ref_assignment_non_matching_rhs_breaks().
  test_find_return_enum_ref_assignment_no_children_no_crash: test_find_return_enum_ref_assignment_no_children_no_crash().
  test_parse_file_for_state_returns_none_for_missing_file: test_parse_file_for_state_returns_none_for_missing_file().
  test_render_state_mermaid_starts_with_stateDiagram: test_render_state_mermaid_starts_with_stateDiagram().
  test_render_state_mermaid_includes_states: test_render_state_mermaid_includes_states().
  test_render_state_mermaid_includes_initial_edges: test_render_state_mermaid_includes_initial_edges().
  test_render_state_mermaid_approximation_note: test_render_state_mermaid_approximation_note().
  test_render_state_mermaid_empty_states: test_render_state_mermaid_empty_states().
  test_state_in_uml_cli_choices: test_state_in_uml_cli_choices().
  test_uml_max_nodes_cli_flag_registered: test_uml_max_nodes_cli_flag_registered().
  test_uml_max_nodes_cli_flag_default_50: test_uml_max_nodes_cli_flag_default_50().
  test_execute_state_diagram_not_found_missing_file.FakeHub.uml_exporter: test_execute_state_diagram_not_found_missing_file().FakeHub#uml_exporter().
  test_execute_state_diagram_success.FakeHub.uml_exporter: test_execute_state_diagram_success().FakeHub#uml_exporter().
  test_execute_state_diagram_not_found_missing_file.FakeExporter: test_execute_state_diagram_not_found_missing_file().FakeExporter#
  test_execute_state_diagram_success.FakeExporter: test_execute_state_diagram_success().FakeExporter#
  test_parse_file_for_state_calls_parser_once.counting_parse: test_parse_file_for_state_calls_parser_once().counting_parse().
  test_execute_state_diagram_not_found_missing_file.FakeHub: test_execute_state_diagram_not_found_missing_file().FakeHub#
  test_execute_state_diagram_success.FakeHub: test_execute_state_diagram_success().FakeHub#
  test_node_text_exception_returns_empty.BadNode: test_node_text_exception_returns_empty().BadNode#
  test_build_state_result_parse_failed.fake_parse: test_build_state_result_parse_failed().fake_parse().
  test_execute_state_diagram_not_found_missing_file.FakeHub.__init__: test_execute_state_diagram_not_found_missing_file().FakeHub#__init__().
  test_execute_state_diagram_success.FakeHub.__init__: test_execute_state_diagram_success().FakeHub#__init__().
  test_node_text_exception_returns_empty.BadNode.text: test_node_text_exception_returns_empty().BadNode#text().
---
# Module: [`tests/unit/test_uml_state.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py)

## Classes
### `BadNode`
- def: [`tests/unit/test_uml_state.py:1307`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L1307)
- signature: `class BadNode:`
- members:
  - `text(self)` — [`L1309`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L1309)
- used by: (1 test-only callers)

### `FakeExporter`
- def: [`tests/unit/test_uml_state.py:887`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L887)
- signature: `class FakeExporter:`
- members:
  - `state_diagram(self, *, class_name: str | None = None, file_path: str | None = None, max_nodes: int = 30)` — [`L835`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L835)
  - `state_diagram(self, *, class_name: str | None = None, file_path: str | None = None, max_nodes: int = 30)` — [`L888`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L888)
- uses (calls/refs, reference-scoped): [`metadata`](../../tree_sitter_analyzer/uml_export.md#UMLDiagram.metadata), [`UMLEdge`](../../tree_sitter_analyzer/uml_export.md#UMLEdge), [`mermaid`](../../tree_sitter_analyzer/uml_export.md#UMLDiagram.mermaid), [`nodes`](../../tree_sitter_analyzer/uml_export.md#UMLDiagram.nodes), [`UMLDiagram`](../../tree_sitter_analyzer/uml_export.md#UMLDiagram), [`edges`](../../tree_sitter_analyzer/uml_export.md#UMLDiagram.edges), [`diagram_type`](../../tree_sitter_analyzer/uml_export.md#UMLDiagram.diagram_type), [`mermaid_type`](../../tree_sitter_analyzer/uml_export.md#UMLDiagram.mermaid_type)
- used by: (1 test-only callers)

### `FakeHub`
- def: [`tests/unit/test_uml_state.py:909`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L909)
- signature: `class FakeHub:`
- members:
  - `uml_exporter(self)` — [`L859`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L859)
  - `uml_exporter(self)` — [`L913`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L913)
- protocol/private: `__init__`[`L856`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L856), `__init__`[`L910`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L910)
- uses (calls/refs, reference-scoped): (2 test-only callers)
- used by: (1 test-only callers)

## Functions
- `_make_ts_node(type_: str, text: str = "", children: list | None = None)` — [`L21`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L21) — Build a minimal tree-sitter node mock that won't OOM.
- `counting_parse(file_path: str, language: str = "python")` — [`L99`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L99)
- `fake_parse(file_path: str, language: str = "python")` — [`L1338`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L1338)
- `test_assignment_transitions_combined_with_return(tmp_path: Path)` — [`L701`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L701) — A mix of return-based and assignment-based transitions are all captured.
- `test_assignment_transitions_detected_door_controller(tmp_path: Path)` — [`L654`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L654) — OOP FSM with self.state = Door.LOCKED produces transitions (P2a fix).
- `test_build_state_result_class_name_filter(tmp_path: Path)` — [`L197`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L197) — class_name filter selects only the named Enum class.
- `test_build_state_result_class_name_not_found(tmp_path: Path)` — [`L225`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L225) — class_name that does not exist → error='NOT_FOUND:class_missing'.
- `test_build_state_result_finds_enum_members(tmp_path: Path)` — [`L148`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L148) — Enum subclass members become states; exact count pinned.
- `test_build_state_result_ignores_underscore_prefixed_members(tmp_path: Path)` — [`L1728`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L1728) — _extract_enum_members skips names starting with '_' (line 157 branch).
- `test_build_state_result_match_transitions_detected(tmp_path: Path)` — [`L273`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L273) — match/case blocks targeting enum members produce transitions.
- `test_build_state_result_max_nodes_truncates(tmp_path: Path)` — [`L247`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L247) — max_nodes=2 truncates a 4-member enum to 2 states, truncated=True.
- `test_build_state_result_missing_file_returns_not_found(tmp_path: Path)` — [`L119`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L119) — build_state_result returns error='NOT_FOUND:file_missing' for absent file.
- `test_build_state_result_no_match_zero_transitions(tmp_path: Path)` — [`L340`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L340) — Enum with no match/case block has zero transitions.
- `test_build_state_result_parse_failed(tmp_path: Path)` — [`L1331`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L1331) — build_state_result returns error='PARSE_FAILED' when parser returns None (line 332).
- `test_build_state_result_real_file_no_enum(tmp_path: Path)` — [`L133`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L133) — File with no Enum subclass → error='NOT_FOUND:no_enum_class'.
- `test_build_state_result_state_names_correct(tmp_path: Path)` — [`L173`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L173) — State names match the enum member names exactly.
- `test_build_state_result_transition_sources_and_targets(tmp_path: Path)` — [`L308`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L308) — Transition source/target names match the case/return pattern.
- `test_case_pattern_fallback_exercises_node_text_path()` — [`L1510`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L1510) — _extract_transitions uses case_pattern text fallback when children don't yield ref (line 283).
- `test_dotted_name_direct_source_member()` — [`L1544`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L1544) — Lines 284-287: dotted_name/attribute directly in case_clause as source member.
- `test_dotted_name_non_matching_source_skipped()` — [`L1573`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L1573) — Line 286->271: dotted_name in case_clause doesn't match enum prefix → skipped.
- `test_enum_with_docstring_skips_non_assignment_expressions(tmp_path: Path)` — [`L1256`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L1256) — Enum class with a docstring: expression_statement wrapping a string
- `test_enum_with_method_body_still_extracts_members(tmp_path: Path)` — [`L1224`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L1224) — Enum class with a method definition: non-expression_statement block children
- `test_execute_state_diagram_not_found_missing_file(tmp_path: Path)` — [`L829`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L829) — execute with diagram='state' and missing file returns verdict NOT_FOUND.
- `test_execute_state_diagram_success(tmp_path: Path)` — [`L882`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L882) — execute with diagram='state' and a valid FakeExporter returns INFO verdict.
- `test_extract_enum_members_includes_lowercase(tmp_path: Path)` — [`L1075`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L1075) — _extract_enum_members includes lowercase names as enum members.
- `test_extract_enum_members_with_empty_lhs_children_skipped()` — [`L1421`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L1421) — _extract_enum_members skips an assignment with empty children (line 153->150).
- `test_extract_enum_members_with_non_identifier_lhs_skipped()` — [`L1441`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L1441) — _extract_enum_members skips an assignment whose LHS is not an identifier (line 155->150).
- `test_find_return_enum_ref_assignment_branch_via_integration(tmp_path: Path)` — [`L1684`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L1684) — Assignment-style transitions exercise the reversed-children scan (lines 211-220).
- `test_find_return_enum_ref_assignment_no_children_no_crash()` — [`L1662`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L1662) — _find_return_enum_ref handles assignment with no children gracefully (line 215->221).
- `test_find_return_enum_ref_assignment_non_matching_rhs_breaks()` — [`L1632`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L1632) — _find_return_enum_ref hits break (line 220) when RHS of assignment doesn't match enum.
- `test_find_return_enum_ref_assignment_with_eq_first_reversed()` — [`L1603`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L1603) — _find_return_enum_ref skips reversed children where type == '=' (line 216->215).
- `test_info_zero_transition_state_diagram_mermaid_starts_with_header(tmp_path: Path)` — [`L1005`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L1005) — INFO (zero-transition) mermaid output starts with 'stateDiagram-v2' header.
- `test_info_zero_transition_state_diagram_no_initial_edges(tmp_path: Path)` — [`L973`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L973) — INFO (zero-transition) state diagram mermaid must NOT contain '[*] -->' lines.
- `test_iter_case_clauses_block_with_non_case_clause_child()` — [`L1460`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L1460) — _iter_case_clauses skips non-case_clause children in block (line 258->257).
- `test_iter_case_clauses_direct_child_fallback()` — [`L1403`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L1403) — _iter_case_clauses handles direct case_clause children (grammar fallback, line 262).
- `test_multi_enum_both_have_transitions_aggregated_and_deduped(tmp_path: Path)` — [`L1799`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L1799) — Both enums have transitions; cross-enum duplicate transitions are deduped.
- `test_multi_enum_dedup_members_preserves_unique(tmp_path: Path)` — [`L1759`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L1759) — When multiple enums have overlapping member names, dedup preserves uniqueness.
- `test_multi_enum_no_transitions_falls_back_to_all_members(tmp_path: Path)` — [`L1362`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L1362) — When class_name is None and NO enum has transitions, fall back to all members.
- `test_node_text_exception_returns_empty()` — [`L1303`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L1303) — _node_text returns '' when node.text raises AttributeError (lines 95-96).
- `test_node_text_long_string_truncated()` — [`L1316`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L1316) — _node_text truncates at max_len (line 94 short-path covered).
- `test_node_text_raw_none_returns_empty()` — [`L1293`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L1293) — _node_text returns '' when node.text is None (line 92 branch).
- `test_parse_enum_ref_no_match_returns_none()` — [`L1479`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L1479) — _parse_enum_ref returns None when text doesn't start with class_name prefix (194->196).
- `test_parse_file_for_state_calls_parser_once(tmp_path: Path)` — [`L83`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L83) — Rule-11 invariant: exactly one tree-sitter parse per build_state_result call.
- `test_parse_file_for_state_returns_none_for_missing_file(tmp_path: Path)` — [`L75`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L75) — Returns None when the file does not exist.
- `test_qualified_enum_base_states_and_transitions(tmp_path: Path)` — [`L1172`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L1172) — enum.Enum-based FSM is recognised (qualified base name fix).
- `test_render_state_mermaid_approximation_note()` — [`L419`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L419) — Mermaid output includes the RFC-mandated %% NOTE: state diagram comment.
- `test_render_state_mermaid_empty_states()` — [`L427`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L427) — Empty state list renders a sentinel node, not a crash.
- `test_render_state_mermaid_includes_initial_edges()` — [`L390`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L390) — Each state gets a [*] --> StateName initial-state edge.
- `test_render_state_mermaid_includes_states()` — [`L380`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L380) — State names appear in the rendered Mermaid.
- `test_render_state_mermaid_starts_with_stateDiagram()` — [`L372`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L372) — render_state_mermaid output starts with 'stateDiagram-v2'.
- `test_render_state_mermaid_transition_edge()` — [`L398`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L398) — Transitions appear as StateA --> StateB.
- `test_render_state_mermaid_transition_with_label()` — [`L408`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L408) — Transition with label appears as StateA --> StateB : label.
- `test_second_enum_transitions_found_when_first_enum_has_none(tmp_path: Path)` — [`L1110`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L1110) — With class_name omitted, transitions from a second Enum are found.
- `test_state_diagram_analysis_kind_metadata(tmp_path: Path)` — [`L486`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L486) — metadata['analysis_kind'] == 'static_approximation' (RFC-0015 §P2-B).
- `test_state_diagram_diagram_type(tmp_path: Path)` — [`L467`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L467) — UMLDiagram.diagram_type == 'state'.
- `test_state_diagram_exact_node_count_with_transitions(tmp_path: Path)` — [`L619`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L619) — node count == 3 for a 3-member Enum FSM with transitions.
- `test_state_diagram_mermaid_starts_stateDiagram_with_transitions(tmp_path: Path)` — [`L568`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L568) — mermaid output starts with 'stateDiagram-v2' for a real FSM.
- `test_state_diagram_mermaid_type(tmp_path: Path)` — [`L447`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L447) — UMLDiagram.mermaid_type == 'stateDiagram-v2'.
- `test_state_diagram_missing_file_not_found(tmp_path: Path)` — [`L557`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L557) — Missing file → verdict='NOT_FOUND' in metadata.
- `test_state_diagram_node_count_exact_no_transitions(tmp_path: Path)` — [`L598`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L598) — node count == 2 for a 2-member Enum with no transitions (NOT_FOUND path).
- `test_state_diagram_non_python_file_not_found_mentions_language(tmp_path: Path)` — [`L1048`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L1048) — Non-Python file (TypeScript) → NOT_FOUND with language coverage note (#480).
- `test_state_diagram_note_in_metadata(tmp_path: Path)` — [`L506`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L506) — metadata['note'] indicates parsed from current file content.
- `test_state_diagram_true_not_found_zero_states(tmp_path: Path)` — [`L1032`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L1032) — TRUE NOT_FOUND = zero states: class not found in file at all.
- `test_state_diagram_validate_arguments_accepts_state()` — [`L771`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L771) — validate_arguments accepts diagram='state' without error.
- `test_state_diagram_validate_arguments_rejects_unknown()` — [`L780`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L780) — validate_arguments still rejects unknown diagram types.
- `test_state_diagram_zero_transitions_info(tmp_path: Path)` — [`L526`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L526) — Zero transitions but states found → verdict='INFO' in metadata (#480 fix).
- `test_state_in_diagram_enum()` — [`L745`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L745) — 'state' appears in CodeGraphUMLTool schema diagram enum.
- `test_state_in_uml_cli_choices()` — [`L794`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L794) — 'state' is a valid choice for the --uml CLI flag.
- `test_state_result_dataclass_exists()` — [`L41`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L41) — StateResult dataclass is importable and has expected fields.
- `test_state_transition_dataclass_exists()` — [`L52`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L52) — StateTransition dataclass has source/target/label fields.
- `test_state_transition_label_defaults_empty()` — [`L62`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L62) — StateTransition label defaults to empty string.
- `test_uml_max_nodes_cli_flag_default_50()` — [`L812`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L812) — --uml-max-nodes default is 50 (matches RFC-0015 table).
- `test_uml_max_nodes_cli_flag_registered()` — [`L803`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L803) — --uml-max-nodes is registered in the CLI parser.
- `test_uml_max_nodes_cli_mcp_default_parity()` — [`L944`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L944) — CLI argparse default for --uml-max-nodes == MCP schema default for max_nodes.
- `test_uml_tool_schema_lists_diagrams_with_state()` — [`L754`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_state.py#L754) — Enum after P2-A + P2-B integration — exactly 6 members.

