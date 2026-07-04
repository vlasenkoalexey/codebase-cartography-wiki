---
title: 'Module: tests/unit/test_uml_activity.py'
type: catalog
provenance: extracted
module: tests/unit/test_uml_activity.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_uml_activity`/test_
symbols:
  test_handle_try_exc_node_path: handle_try_exc_node_path().
  test_try_except_both_return_no_exit_edge: try_except_both_return_no_exit_edge().
  test_if_true_false_edge_labels_with_else: if_true_false_edge_labels_with_else().
  test_if_true_false_edge_labels_no_else: if_true_false_edge_labels_no_else().
  test_handle_if_no_else_false_live_has_non_condition: handle_if_no_else_false_live_has_non_condition().
  test_activity_diagram_no_file_path_index_unique_resolves: activity_diagram_no_file_path_index_unique_resolves().
  test_activity_index_lookup_ignores_non_python_same_name: activity_index_lookup_ignores_non_python_same_name().
  test_activity_diagram_max_nodes_cap: activity_diagram_max_nodes_cap().
  test_activity_diagram_mermaid_type_and_comment: activity_diagram_mermaid_type_and_comment().
  test_activity_diagram_parse_count_exactly_one: activity_diagram_parse_count_exactly_one().
  test_activity_diagram_large_function_parse_count: activity_diagram_large_function_parse_count().
  test_return_label_exact_text: return_label_exact_text().
  test_raise_label_exact_text: raise_label_exact_text().
  test_find_function_bare_name_picks_outermost: find_function_bare_name_picks_outermost().
  test_find_function_qualified_name_picks_inner: find_function_qualified_name_picks_inner().
  test_for_loop_label_includes_both_sides: for_loop_label_includes_both_sides().
  test_condition_text_for_statement_skips_empty_text_children: condition_text_for_statement_skips_empty_text_children().
  test_build_activity_cfg_max_nodes_zero_returns_truncated: build_activity_cfg_max_nodes_zero_returns_truncated().
  test_build_activity_cfg_no_block_child_uses_func_node: build_activity_cfg_no_block_child_uses_func_node().
  test_build_activity_cfg_exit_node_truncated_no_extra_edge: build_activity_cfg_exit_node_truncated_no_extra_edge().
  test_return_node_not_added_when_truncated: return_node_not_added_when_truncated().
  test_handle_if_cond_none_when_max_nodes_reached: handle_if_cond_none_when_max_nodes_reached().
  test_handle_loop_node_none_when_truncated: handle_loop_node_none_when_truncated().
  test_handle_try_node_none_when_truncated: handle_try_node_none_when_truncated().
  test_handle_try_bare_except: handle_try_bare_except().
  test_handle_try_only_no_except_uses_try_node: handle_try_only_no_except_uses_try_node().
  test_activity_diagram_no_file_path_returns_not_found: activity_diagram_no_file_path_returns_not_found().
  test_activity_diagram_relative_file_path: activity_diagram_relative_file_path().
  test_raise_node_not_added_when_truncated: raise_node_not_added_when_truncated().
  test_activity_diagram_no_file_path_index_not_found_message: activity_diagram_no_file_path_index_not_found_message().
  test_activity_diagram_no_file_path_index_ambiguous_lists_files: activity_diagram_no_file_path_index_ambiguous_lists_files().
  test_activity_diagram_metadata_analysis_kind: activity_diagram_metadata_analysis_kind().
  test_activity_diagram_node_count_simple_if: activity_diagram_node_count_simple_if().
  test_activity_diagram_for_loop: activity_diagram_for_loop().
  test_activity_diagram_while_loop: activity_diagram_while_loop().
  test_activity_diagram_try_except: activity_diagram_try_except().
  test_activity_diagram_raise_statement: activity_diagram_raise_statement().
  test_activity_diagram_empty_function_returns_not_found: activity_diagram_empty_function_returns_not_found().
  test_activity_diagram_missing_file_returns_not_found: activity_diagram_missing_file_returns_not_found().
  test_activity_diagram_function_not_found_in_file_returns_not_found: activity_diagram_function_not_found_in_file_returns_not_found().
  test_activity_diagram_metadata_note_always_set: activity_diagram_metadata_note_always_set().
  test_build_activity_cfg_parse_failed: build_activity_cfg_parse_failed().
  test_handle_if_elif_else_full: handle_if_elif_else_full().
  test_handle_if_elif_no_else: handle_if_elif_no_else().
  test_handle_if_with_else_false_live_non_condition: handle_if_with_else_false_live_non_condition().
  test_handle_loop_body_with_return_inside: handle_loop_body_with_return_inside().
  test_activity_diagram_parse_failed_via_exporter: activity_diagram_parse_failed_via_exporter().
  test_parse_file_for_activity_returns_none_on_parse_failure: parse_file_for_activity_returns_none_on_parse_failure().
  test_build_all_terminal_paths_no_exit: build_all_terminal_paths_no_exit().
  test_handle_if_elif_node_none_skip: handle_if_elif_node_none_skip().
  test_uml_tool_schema_lists_diagrams_with_activity: uml_tool_schema_lists_diagrams_with_activity().
  test_activity_in_diagram_enum: activity_in_diagram_enum().
  test_function_name_declared_in_schema: function_name_declared_in_schema().
  test_max_nodes_declared_in_schema: max_nodes_declared_in_schema().
  test_activity_diagram_requires_function_name: activity_diagram_requires_function_name().
  test_activity_diagram_with_function_name_passes_validation: activity_diagram_with_function_name_passes_validation().
  test_activity_diagram_unknown_value_still_rejected: activity_diagram_unknown_value_still_rejected().
  test_build_uml_tool_args_passes_function_name.FakeArgs.uml_max_nodes: build_uml_tool_args_passes_function_name().FakeArgs#uml_max_nodes.
  test_build_uml_tool_args_omits_function_name_when_none.FakeArgs.uml_max_nodes: build_uml_tool_args_omits_function_name_when_none().FakeArgs#uml_max_nodes.
  test_activity_diagram_via_execute: activity_diagram_via_execute().
  test_activity_diagram_missing_function_name_error: activity_diagram_missing_function_name_error().
  test_node_text_returns_empty_on_decode_exception: node_text_returns_empty_on_decode_exception().
  test_condition_text_for_only_right_side: condition_text_for_only_right_side().
  test_condition_text_for_only_right_side.make_child: condition_text_for_only_right_side().make_child().
  test_find_function_node_qualified_outer_missing: find_function_node_qualified_outer_missing().
  test_find_function_node_identifier_decode_error: find_function_node_identifier_decode_error().
  test_handle_try_no_except_returns_try_node: handle_try_no_except_returns_try_node().
  test_uml_tool_meta_verdict_from_not_found_function: uml_tool_meta_verdict_from_not_found_function().
  test_parse_file_for_activity_direct_parse_failure: parse_file_for_activity_direct_parse_failure().
  test_escape_label_strips_newlines: escape_label_strips_newlines().
  test_multiline_condition_no_newline_in_mermaid: multiline_condition_no_newline_in_mermaid().
  test_phase2_cli_flags_registered: phase2_cli_flags_registered().
  test_uml_enum_includes_activity_in_cli: uml_enum_includes_activity_in_cli().
  test_build_uml_tool_args_passes_function_name: build_uml_tool_args_passes_function_name().
  test_build_uml_tool_args_omits_function_name_when_none: build_uml_tool_args_omits_function_name_when_none().
  test_node_text_returns_empty_when_text_is_none: node_text_returns_empty_when_text_is_none().
  test_node_text_truncates_long_text: node_text_truncates_long_text().
  test_condition_text_non_for_all_keywords_fallback: condition_text_non_for_all_keywords_fallback().
  test_find_function_node_root_none: find_function_node_root_none().
  test_safe_id_prepends_N_for_digit_start: safe_id_prepends_N_for_digit_start().
  test_safe_id_empty_string_prepends_N: safe_id_empty_string_prepends_N().
  test_render_flowchart_mermaid_empty_nodes_and_edges: render_flowchart_mermaid_empty_nodes_and_edges().
  test_file_matches_returns_false_for_empty_inputs: file_matches_returns_false_for_empty_inputs().
  test_is_neighbourhood_center_none_returns_false: is_neighbourhood_center_none_returns_false().
  test_find_function_node_function_without_identifier_child: find_function_node_function_without_identifier_child().
  test_activity_diagram_parse_count_exactly_one.counting_parse: activity_diagram_parse_count_exactly_one().counting_parse().
  test_activity_diagram_large_function_parse_count.counting_parse: activity_diagram_large_function_parse_count().counting_parse().
  test_build_uml_tool_args_passes_function_name.FakeArgs: build_uml_tool_args_passes_function_name().FakeArgs#
  test_build_uml_tool_args_omits_function_name_when_none.FakeArgs: build_uml_tool_args_omits_function_name_when_none().FakeArgs#
  test_node_text_returns_empty_on_decode_exception.BadText: node_text_returns_empty_on_decode_exception().BadText#
  test_find_function_node_identifier_decode_error.BadBytes: find_function_node_identifier_decode_error().BadBytes#
  test_activity_diagram_no_file_path_returns_not_found.FakeCache: activity_diagram_no_file_path_returns_not_found().FakeCache#
  test_parse_file_for_activity_direct_parse_failure.FakeParser: parse_file_for_activity_direct_parse_failure().FakeParser#
  test_activity_diagram_no_file_path_index_unique_resolves.FakeCache: activity_diagram_no_file_path_index_unique_resolves().FakeCache#
  test_activity_diagram_no_file_path_index_not_found_message.FakeCache: activity_diagram_no_file_path_index_not_found_message().FakeCache#
  test_activity_diagram_no_file_path_index_ambiguous_lists_files.FakeCache: activity_diagram_no_file_path_index_ambiguous_lists_files().FakeCache#
  test_activity_index_lookup_ignores_non_python_same_name.PolyglotCache: activity_index_lookup_ignores_non_python_same_name().PolyglotCache#
  test_build_uml_tool_args_passes_function_name.FakeArgs.uml: build_uml_tool_args_passes_function_name().FakeArgs#uml.
  test_build_uml_tool_args_passes_function_name.FakeArgs.uml_source: build_uml_tool_args_passes_function_name().FakeArgs#uml_source.
  test_build_uml_tool_args_passes_function_name.FakeArgs.uml_target: build_uml_tool_args_passes_function_name().FakeArgs#uml_target.
  test_build_uml_tool_args_passes_function_name.FakeArgs.uml_max_edges: build_uml_tool_args_passes_function_name().FakeArgs#uml_max_edges.
  test_build_uml_tool_args_passes_function_name.FakeArgs.uml_max_depth: build_uml_tool_args_passes_function_name().FakeArgs#uml_max_depth.
  test_build_uml_tool_args_passes_function_name.FakeArgs.uml_max_paths: build_uml_tool_args_passes_function_name().FakeArgs#uml_max_paths.
  test_build_uml_tool_args_passes_function_name.FakeArgs.uml_package_depth: build_uml_tool_args_passes_function_name().FakeArgs#uml_package_depth.
  test_build_uml_tool_args_passes_function_name.FakeArgs.uml_no_external_bases: build_uml_tool_args_passes_function_name().FakeArgs#uml_no_external_bases.
  test_build_uml_tool_args_passes_function_name.FakeArgs.uml_file_path: build_uml_tool_args_passes_function_name().FakeArgs#uml_file_path.
  test_build_uml_tool_args_passes_function_name.FakeArgs.uml_class_name: build_uml_tool_args_passes_function_name().FakeArgs#uml_class_name.
  test_build_uml_tool_args_passes_function_name.FakeArgs.uml_include_tests: build_uml_tool_args_passes_function_name().FakeArgs#uml_include_tests.
  test_build_uml_tool_args_passes_function_name.FakeArgs.uml_function: build_uml_tool_args_passes_function_name().FakeArgs#uml_function.
  test_build_uml_tool_args_omits_function_name_when_none.FakeArgs.uml: build_uml_tool_args_omits_function_name_when_none().FakeArgs#uml.
  test_build_uml_tool_args_omits_function_name_when_none.FakeArgs.uml_source: build_uml_tool_args_omits_function_name_when_none().FakeArgs#uml_source.
  test_build_uml_tool_args_omits_function_name_when_none.FakeArgs.uml_target: build_uml_tool_args_omits_function_name_when_none().FakeArgs#uml_target.
  test_build_uml_tool_args_omits_function_name_when_none.FakeArgs.uml_max_edges: build_uml_tool_args_omits_function_name_when_none().FakeArgs#uml_max_edges.
  test_build_uml_tool_args_omits_function_name_when_none.FakeArgs.uml_max_depth: build_uml_tool_args_omits_function_name_when_none().FakeArgs#uml_max_depth.
  test_build_uml_tool_args_omits_function_name_when_none.FakeArgs.uml_max_paths: build_uml_tool_args_omits_function_name_when_none().FakeArgs#uml_max_paths.
  test_build_uml_tool_args_omits_function_name_when_none.FakeArgs.uml_package_depth: build_uml_tool_args_omits_function_name_when_none().FakeArgs#uml_package_depth.
  test_build_uml_tool_args_omits_function_name_when_none.FakeArgs.uml_no_external_bases: build_uml_tool_args_omits_function_name_when_none().FakeArgs#uml_no_external_bases.
  test_build_uml_tool_args_omits_function_name_when_none.FakeArgs.uml_file_path: build_uml_tool_args_omits_function_name_when_none().FakeArgs#uml_file_path.
  test_build_uml_tool_args_omits_function_name_when_none.FakeArgs.uml_class_name: build_uml_tool_args_omits_function_name_when_none().FakeArgs#uml_class_name.
  test_build_uml_tool_args_omits_function_name_when_none.FakeArgs.uml_include_tests: build_uml_tool_args_omits_function_name_when_none().FakeArgs#uml_include_tests.
  test_build_uml_tool_args_omits_function_name_when_none.FakeArgs.uml_function: build_uml_tool_args_omits_function_name_when_none().FakeArgs#uml_function.
  test_node_text_returns_empty_on_decode_exception.BadText.decode: node_text_returns_empty_on_decode_exception().BadText#decode().
  test_find_function_node_identifier_decode_error.BadBytes.decode: find_function_node_identifier_decode_error().BadBytes#decode().
  test_activity_diagram_no_file_path_returns_not_found.FakeCache.search_symbols: activity_diagram_no_file_path_returns_not_found().FakeCache#search_symbols().
  test_activity_diagram_no_file_path_returns_not_found.FakeCache.close: activity_diagram_no_file_path_returns_not_found().FakeCache#close().
  test_parse_file_for_activity_direct_parse_failure.FakeParser.parse_file: parse_file_for_activity_direct_parse_failure().FakeParser#parse_file().
  test_activity_diagram_no_file_path_index_unique_resolves.FakeCache.search_symbols: activity_diagram_no_file_path_index_unique_resolves().FakeCache#search_symbols().
  test_activity_diagram_no_file_path_index_unique_resolves.FakeCache.close: activity_diagram_no_file_path_index_unique_resolves().FakeCache#close().
  test_activity_diagram_no_file_path_index_not_found_message.FakeCache.search_symbols: activity_diagram_no_file_path_index_not_found_message().FakeCache#search_symbols().
  test_activity_diagram_no_file_path_index_not_found_message.FakeCache.close: activity_diagram_no_file_path_index_not_found_message().FakeCache#close().
  test_activity_diagram_no_file_path_index_ambiguous_lists_files.FakeCache.search_symbols: activity_diagram_no_file_path_index_ambiguous_lists_files().FakeCache#search_symbols().
  test_activity_diagram_no_file_path_index_ambiguous_lists_files.FakeCache.close: activity_diagram_no_file_path_index_ambiguous_lists_files().FakeCache#close().
  test_activity_index_lookup_ignores_non_python_same_name.PolyglotCache.search_symbols: activity_index_lookup_ignores_non_python_same_name().PolyglotCache#search_symbols().
  test_activity_index_lookup_ignores_non_python_same_name.PolyglotCache.close: activity_index_lookup_ignores_non_python_same_name().PolyglotCache#close().
---
# Module: [`tests/unit/test_uml_activity.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py)

## Classes
### `BadBytes`
- def: [`tests/unit/test_uml_activity.py:809`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L809)
- signature: `class BadBytes:`
- members:
  - `decode(self, *a, **kw)` — [`L810`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L810)
- used by: (1 test-only callers)

### `BadText`
- def: [`tests/unit/test_uml_activity.py:656`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L656)
- signature: `class BadText:`
- members:
  - `decode(self, *a, **kw)` — [`L657`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L657)
- used by: (1 test-only callers)

### `FakeArgs`
- def: [`tests/unit/test_uml_activity.py:582`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L582)
- signature: `class FakeArgs:`
- members:
  - `uml` — [`L556`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L556)
  - `uml` — [`L583`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L583)
  - `uml_class_name` — [`L565`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L565)
  - `uml_class_name` — [`L592`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L592)
  - `uml_file_path` — [`L564`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L564)
  - `uml_file_path` — [`L591`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L591)
  - `uml_function` — [`L567`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L567)
  - `uml_function` — [`L594`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L594)
  - `uml_include_tests` — [`L566`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L566)
  - `uml_include_tests` — [`L593`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L593)
  - `uml_max_depth` — [`L560`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L560)
  - `uml_max_depth` — [`L587`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L587)
  - `uml_max_edges` — [`L559`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L559)
  - `uml_max_edges` — [`L586`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L586)
  - `uml_max_nodes` — [`L568`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L568)
  - `uml_max_nodes` — [`L595`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L595)
  - `uml_max_paths` — [`L561`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L561)
  - `uml_max_paths` — [`L588`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L588)
  - `uml_no_external_bases` — [`L563`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L563)
  - `uml_no_external_bases` — [`L590`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L590)
  - `uml_package_depth` — [`L562`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L562)
  - `uml_package_depth` — [`L589`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L589)
  - `uml_source` — [`L557`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L557)
  - `uml_source` — [`L584`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L584)
  - `uml_target` — [`L558`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L558)
  - `uml_target` — [`L585`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L585)
- uses (calls/refs, reference-scoped): [`_build_uml_tool_args`](../../tree_sitter_analyzer/cli/commands/mcp_commands/_builders.md#_build_uml_tool_args)  (1 test-only)

### `FakeCache`
- def: [`tests/unit/test_uml_activity.py:1525`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L1525)
- signature: `class FakeCache:`
- members:
  - `close(self)` — [`L1205`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L1205)
  - `close(self)` — [`L1479`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L1479)
  - `close(self)` — [`L1504`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L1504)
  - `close(self)` — [`L1532`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L1532)
  - `search_symbols(self, query: str, language: str | None = None)` — [`L1202`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L1202)
  - `search_symbols(self, query: str, language: str | None = None)` — [`L1474`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L1474)
  - `search_symbols(self, query: str, language: str | None = None)` — [`L1501`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L1501)
  - `search_symbols(self, query: str, language: str | None = None)` — [`L1526`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L1526)
- used by: (1 test-only callers)

### `FakeParser`
- def: [`tests/unit/test_uml_activity.py:1318`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L1318)
- signature: `class FakeParser:`
- members:
  - `parse_file(self, file_path, language)` — [`L1319`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L1319)
- used by: (1 test-only callers)

### `PolyglotCache`
- def: [`tests/unit/test_uml_activity.py:1551`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L1551)
- signature: `class PolyglotCache:`
- members:
  - `close(self)` — [`L1568`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L1568)
  - `search_symbols(self, query: str, language: str | None = None)` — [`L1552`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L1552)
- used by: (1 test-only callers)

## Functions
- `counting_parse(file_path: str, language: str = "python")` — [`L251`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L251)
- `counting_parse(file_path: str, language: str = "python")` — [`L287`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L287)
- `make_child(ctype, text_bytes)` — [`L708`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L708)
- `test_activity_diagram_empty_function_returns_not_found(tmp_path: Path)` — [`L174`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L174) — Empty (stub) function: zero CFG nodes -> NOT_FOUND with next_step.
- `test_activity_diagram_for_loop(tmp_path: Path)` — [`L116`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L116) — For loop: entry + loop-header + return = 3 nodes.
- `test_activity_diagram_function_not_found_in_file_returns_not_found(tmp_path: Path)` — [`L198`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L198) — When the function name doesn't exist in the file, return NOT_FOUND.
- `test_activity_diagram_large_function_parse_count(tmp_path: Path)` — [`L265`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L265) — ~100-line function: parse count must be exactly 1 (rule-11 invariant).
- `test_activity_diagram_max_nodes_cap(tmp_path: Path)` — [`L212`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L212) — max_nodes=2 truncates: only 2 nodes emitted + truncated flag set.
- `test_activity_diagram_mermaid_type_and_comment(tmp_path: Path)` — [`L76`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L76) — activity_diagram returns flowchart TD with the RFC comment header.
- `test_activity_diagram_metadata_analysis_kind(tmp_path: Path)` — [`L92`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L92)
- `test_activity_diagram_metadata_note_always_set(tmp_path: Path)` — [`L372`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L372) — Successful activity diagram must carry metadata['note'] (RFC-0015 stale-file contract).
- `test_activity_diagram_missing_file_returns_not_found(tmp_path: Path)` — [`L186`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L186) — When the file no longer exists, return NOT_FOUND.
- `test_activity_diagram_missing_function_name_error(tmp_path: Path)` — [`L627`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L627) — activity without function_name returns error response via execute().
- `test_activity_diagram_no_file_path_index_ambiguous_lists_files(tmp_path)` — [`L1515`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L1515) — RED → GREEN (#477 STRONG): multiple index hits → NOT_FOUND with candidate files.
- `test_activity_diagram_no_file_path_index_not_found_message(tmp_path)` — [`L1492`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L1492) — RED → GREEN (#477 STRONG): no index hit → NOT_FOUND with 'not found in the index'.
- `test_activity_diagram_no_file_path_index_unique_resolves(tmp_path)` — [`L1461`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L1461) — RED → GREEN (#477 STRONG): unique index hit → resolve file and build CFG.
- `test_activity_diagram_no_file_path_returns_not_found(tmp_path)` — [`L1193`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L1193) — activity_diagram with file_path=None AND no index hit returns NOT_FOUND.
- `test_activity_diagram_node_count_simple_if(tmp_path: Path)` — [`L102`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L102) — Simple if/else function: entry + condition + two return branches = 4 nodes.
- `test_activity_diagram_parse_count_exactly_one(tmp_path: Path)` — [`L230`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L230) — Activity diagram triggers exactly ONE tree-sitter parse, not more.
- `test_activity_diagram_parse_failed_via_exporter(tmp_path)` — [`L1228`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L1228) — activity_diagram returns verdict=NOT_FOUND on PARSE_FAILED (line 587).
- `test_activity_diagram_raise_statement(tmp_path: Path)` — [`L162`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L162) — Raise: entry + raise = 2 nodes.
- `test_activity_diagram_relative_file_path(tmp_path)` — [`L1215`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L1215) — activity_diagram resolves relative file_path relative to project_root (line 513).
- `test_activity_diagram_requires_function_name()` — [`L53`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L53)
- `test_activity_diagram_try_except(tmp_path: Path)` — [`L144`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L144) — Try/except: entry + try + except + exit = 4 nodes.
- `test_activity_diagram_unknown_value_still_rejected()` — [`L65`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L65)
- `test_activity_diagram_via_execute(tmp_path: Path)` — [`L607`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L607) — activity diagram via the real execute() boundary (MCP tool path).
- `test_activity_diagram_while_loop(tmp_path: Path)` — [`L130`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L130) — While loop: entry + while-condition + return = 3 nodes.
- `test_activity_diagram_with_function_name_passes_validation()` — [`L59`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L59)
- `test_activity_in_diagram_enum()` — [`L28`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L28)
- `test_activity_index_lookup_ignores_non_python_same_name(tmp_path)` — [`L1543`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L1543) — Codex P2 (#498): a same-name JS symbol must not make the Python
- `test_build_activity_cfg_exit_node_truncated_no_extra_edge(tmp_path)` — [`L891`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L891) — When exit node cannot be added (max_nodes reached), no pred→exit edge added (lines 264-266).
- `test_build_activity_cfg_max_nodes_zero_returns_truncated()` — [`L843`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L843) — max_nodes=0: entry node itself cannot be added → truncated=True (line 244).
- `test_build_activity_cfg_no_block_child_uses_func_node(tmp_path)` — [`L862`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L862) — When func_node has no block/body child, walker uses func_node itself (lines 252-254).
- `test_build_activity_cfg_parse_failed(tmp_path)` — [`L758`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L758) — When _parse_file_for_activity returns None → error='PARSE_FAILED' (line 459).
- `test_build_all_terminal_paths_no_exit(tmp_path)` — [`L1341`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L1341) — When all paths from last_nodes terminate, non_terminal is empty → no exit (line 262→268).
- `test_build_uml_tool_args_omits_function_name_when_none()` — [`L576`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L576) — _build_uml_tool_args must NOT include function_name key when not provided.
- `test_build_uml_tool_args_passes_function_name()` — [`L549`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L549) — _build_uml_tool_args must forward function_name when set.
- `test_condition_text_for_only_right_side(tmp_path)` — [`L701`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L701) — for-loop where left side parses empty falls back to right or full text (line 116).
- `test_condition_text_for_statement_skips_empty_text_children(tmp_path)` — [`L684`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L684) — for-loop with a non-empty right side: label includes both sides.
- `test_condition_text_non_for_all_keywords_fallback(tmp_path)` — [`L731`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L731) — _condition_text non-for: all children are keywords → returns node full text (line 123).
- `test_escape_label_strips_newlines()` — [`L342`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L342) — _escape_label must replace \n and \r with space (Mermaid ["..."] safety).
- `test_file_matches_returns_false_for_empty_inputs()` — [`L1176`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L1176) — _file_matches returns False when cls_file or filter_path is empty (line 230).
- `test_find_function_bare_name_picks_outermost(tmp_path: Path)` — [`L436`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L436) — DFS-preorder: bare name returns the outermost match (first encountered).
- `test_find_function_node_function_without_identifier_child(tmp_path)` — [`L1358`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L1358) — _find_function_node: function_definition with no identifier child is skipped (line 181→190).
- `test_find_function_node_identifier_decode_error()` — [`L798`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L798) — _find_function_node when identifier.text.decode raises → name='' (lines 185-186).
- `test_find_function_node_qualified_outer_missing(tmp_path)` — [`L788`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L788) — Qualified 'missing.inner' returns None when outer not found (line 172).
- `test_find_function_node_root_none()` — [`L780`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L780) — _find_function_node(None, name) returns None immediately (line 176).
- `test_find_function_qualified_name_picks_inner(tmp_path: Path)` — [`L451`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L451) — Qualified 'outer.inner' lookup navigates into outer's scope to find inner.
- `test_for_loop_label_includes_both_sides(tmp_path: Path)` — [`L511`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L511) — For loop node label must be 'item in items', not just 'item'.
- `test_function_name_declared_in_schema()` — [`L33`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L33)
- `test_handle_if_cond_none_when_max_nodes_reached(tmp_path)` — [`L973`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L973) — When _add_node returns None for cond (truncated), _handle_if returns incoming (line 323).
- `test_handle_if_elif_else_full(tmp_path)` — [`L929`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L929) — if/elif/else: exercises elif_clause (349-359) and else_clause (360-369) paths.
- `test_handle_if_elif_no_else(tmp_path)` — [`L952`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L952) — if/elif without else: exercises elif path (349-359) + false_live pending label (375).
- `test_handle_if_elif_node_none_skip(tmp_path)` — [`L1384`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L1384) — elif_clause where elif_node is None (max_nodes reached): elif body not walked (line 351→369).
- `test_handle_if_no_else_false_live_has_non_condition(tmp_path)` — [`L1434`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L1434) — false_live after if without else contains condition; its pending label is set (line 374→376).
- `test_handle_if_with_else_false_live_non_condition(tmp_path)` — [`L986`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L986) — else_clause processing where false_live contains a loop node (not condition).
- `test_handle_loop_body_with_return_inside(tmp_path)` — [`L1036`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L1036) — Loop body with return inside: exercises _walk_body from loop (lines 392-396).
- `test_handle_loop_node_none_when_truncated(tmp_path)` — [`L1021`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L1021) — When loop_node cannot be added (max_nodes=1), _handle_loop returns incoming (line 387).
- `test_handle_try_bare_except(tmp_path)` — [`L1097`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L1097) — bare 'except:' (no exception type): exc_text='' → label='except' (lines 415-419).
- `test_handle_try_exc_node_path(tmp_path)` — [`L1405`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L1405) — except_clause where exc_node is not None: edges and walk happen (line 421→408 arc exercised).
- `test_handle_try_no_except_returns_try_node(tmp_path)` — [`L1077`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L1077) — try block with no except clause: branches_processed=True but outgoing may be empty.
- `test_handle_try_node_none_when_truncated(tmp_path)` — [`L1063`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L1063) — When try_node cannot be added (max_nodes=1), _handle_try returns incoming (line 401).
- `test_handle_try_only_no_except_uses_try_node(tmp_path)` — [`L1110`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L1110) — try body with no except_clause at all → branches_processed=True, return outgoing.
- `test_if_true_false_edge_labels_no_else(tmp_path: Path)` — [`L489`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L489) — Condition→true-body is 'True'; condition falls through to next stmt as 'False'.
- `test_if_true_false_edge_labels_with_else(tmp_path: Path)` — [`L471`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L471) — Condition→true-body edge is labeled 'True'; condition→else-body is 'False'.
- `test_is_neighbourhood_center_none_returns_false()` — [`L1185`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L1185) — _is_neighbourhood returns False immediately when center is None (line 248).
- `test_max_nodes_declared_in_schema()` — [`L40`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L40)
- `test_multiline_condition_no_newline_in_mermaid(tmp_path: Path)` — [`L351`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L351) — Mermaid output must contain no raw newline inside a ["..."] label.
- `test_node_text_returns_empty_on_decode_exception()` — [`L652`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L652) — _node_text returns '' when node.text.decode raises (lines 83-84).
- `test_node_text_returns_empty_when_text_is_none()` — [`L642`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L642) — _node_text returns '' when node.text is None (line 78).
- `test_node_text_truncates_long_text()` — [`L666`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L666) — _node_text appends … when text > max_len (line 81).
- `test_parse_file_for_activity_direct_parse_failure(tmp_path)` — [`L1303`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L1303) — _parse_file_for_activity itself returns None when parser returns no tree (line 146).
- `test_parse_file_for_activity_returns_none_on_parse_failure(tmp_path)` — [`L1275`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L1275) — _parse_file_for_activity returns None when parser.parse_file fails (line 146).
- `test_phase2_cli_flags_registered()` — [`L530`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L530) — --uml-function and --uml-max-nodes must be registered in the CLI parser.
- `test_raise_label_exact_text(tmp_path: Path)` — [`L324`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L324) — Raise node label must be 'raise ValueError…' NOT 'raise raise ValueError…'.
- `test_raise_node_not_added_when_truncated(tmp_path)` — [`L1329`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L1329) — When max_nodes reached during raise_statement, raise_node is None (line 313→316).
- `test_render_flowchart_mermaid_empty_nodes_and_edges()` — [`L1167`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L1167) — render_flowchart_mermaid with no nodes/edges renders 'No edges found' (lines 180-181).
- `test_return_label_exact_text(tmp_path: Path)` — [`L308`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L308) — Return node label must be 'return x' NOT 'return return x'.
- `test_return_node_not_added_when_truncated(tmp_path)` — [`L911`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L911) — When max_nodes is reached, return_statement's _add_node returns None → no node added.
- `test_safe_id_empty_string_prepends_N()` — [`L1157`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L1157) — _safe_id prepends 'N_' when safe is empty after substitution (line 86).
- `test_safe_id_prepends_N_for_digit_start()` — [`L1149`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L1149) — _safe_id prepends 'N_' when name starts with a digit (line 86).
- `test_try_except_both_return_no_exit_edge(tmp_path: Path)` — [`L394`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L394) — When every try/except branch terminates (return/raise), NO exit node is added.
- `test_uml_enum_includes_activity_in_cli()` — [`L540`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L540) — --uml choices must include 'activity'.
- `test_uml_tool_meta_verdict_from_not_found_function(tmp_path)` — [`L1252`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L1252) — execute() with a missing function sets verdict from metadata (line 212).
- `test_uml_tool_schema_lists_diagrams_with_activity()` — [`L21`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_activity.py#L21) — Enum after P2-A + P2-B integration — exactly 6 members (re-pinned).

