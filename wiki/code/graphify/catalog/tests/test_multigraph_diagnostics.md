---
title: 'Module: tests/test_multigraph_diagnostics.py'
type: catalog
provenance: extracted
module: tests/test_multigraph_diagnostics.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_multigraph_diagnostics`/
symbols:
  _diagnostic_fixture: _diagnostic_fixture().
  test_diagnose_file_reads_json_and_formats_report: test_diagnose_file_reads_json_and_formats_report().
  test_diagnostic_json_report_is_serializable: test_diagnostic_json_report_is_serializable().
  test_diagnose_extraction_categorizes_same_endpoint_collapse: test_diagnose_extraction_categorizes_same_endpoint_collapse().
  test_diagnose_extraction_accepts_node_link_links_key: test_diagnose_extraction_accepts_node_link_links_key().
  test_diagnose_extraction_does_not_mutate_input: test_diagnose_extraction_does_not_mutate_input().
  test_diagnose_extraction_bounds_examples: test_diagnose_extraction_bounds_examples().
  test_diagnose_extraction_stops_examples_at_requested_limit: test_diagnose_extraction_stops_examples_at_requested_limit().
  test_diagnose_extraction_defaults_raw_inputs_to_directed: test_diagnose_extraction_defaults_raw_inputs_to_directed().
  test_format_diagnostic_report_includes_build_and_suppression_errors: test_format_diagnostic_report_includes_build_and_suppression_errors().
  test_diagnose_file_rejects_oversized_graph: test_diagnose_file_rejects_oversized_graph().
  test_diagnose_file_defaults_to_json_directed_flag: test_diagnose_file_defaults_to_json_directed_flag().
  test_diagnose_file_explicit_directed_override: test_diagnose_file_explicit_directed_override().
  test_diagnose_multigraph_cli_human_output: test_diagnose_multigraph_cli_human_output().
  test_diagnose_multigraph_cli_undirected_override: test_diagnose_multigraph_cli_undirected_override().
  test_diagnose_multigraph_cli_max_examples_zero: test_diagnose_multigraph_cli_max_examples_zero().
  test_diagnose_multigraph_cli_json_output: test_diagnose_multigraph_cli_json_output().
  test_diagnose_multigraph_cli_rejects_conflicting_direction_flags: test_diagnose_multigraph_cli_rejects_conflicting_direction_flags().
  test_diagnose_extraction_handles_malformed_shapes_without_crashing: test_diagnose_extraction_handles_malformed_shapes_without_crashing().
  test_diagnose_extraction_handles_non_list_nodes_and_edges: test_diagnose_extraction_handles_non_list_nodes_and_edges().
  test_scan_producer_suppression_sites_finds_seen_sets: test_scan_producer_suppression_sites_finds_seen_sets().
  test_scan_producer_suppression_sites_handles_unknown_tuple_arity: test_scan_producer_suppression_sites_handles_unknown_tuple_arity().
  test_diagnose_file_rejects_non_object_json: test_diagnose_file_rejects_non_object_json().
  test_scan_producer_suppression_sites_reports_missing_file: test_scan_producer_suppression_sites_reports_missing_file().
  test_diagnose_multigraph_cli_usage_errors: test_diagnose_multigraph_cli_usage_errors().
---
# Module: [`tests/test_multigraph_diagnostics.py`](../../../../../raw/code/graphify/tests/test_multigraph_diagnostics.py)

## Functions
- `_diagnostic_fixture()` — [`L19`](../../../../../raw/code/graphify/tests/test_multigraph_diagnostics.py#L19)
- `test_diagnose_extraction_accepts_node_link_links_key()` — [`L106`](../../../../../raw/code/graphify/tests/test_multigraph_diagnostics.py#L106)
- `test_diagnose_extraction_bounds_examples()` — [`L164`](../../../../../raw/code/graphify/tests/test_multigraph_diagnostics.py#L164)
- `test_diagnose_extraction_categorizes_same_endpoint_collapse()` — [`L87`](../../../../../raw/code/graphify/tests/test_multigraph_diagnostics.py#L87)
- `test_diagnose_extraction_defaults_raw_inputs_to_directed(tmp_path: Path)` — [`L189`](../../../../../raw/code/graphify/tests/test_multigraph_diagnostics.py#L189)
- `test_diagnose_extraction_does_not_mutate_input()` — [`L116`](../../../../../raw/code/graphify/tests/test_multigraph_diagnostics.py#L116)
- `test_diagnose_extraction_handles_malformed_shapes_without_crashing()` — [`L125`](../../../../../raw/code/graphify/tests/test_multigraph_diagnostics.py#L125)
- `test_diagnose_extraction_handles_non_list_nodes_and_edges()` — [`L153`](../../../../../raw/code/graphify/tests/test_multigraph_diagnostics.py#L153)
- `test_diagnose_extraction_stops_examples_at_requested_limit()` — [`L171`](../../../../../raw/code/graphify/tests/test_multigraph_diagnostics.py#L171)
- `test_diagnose_file_defaults_to_json_directed_flag(tmp_path: Path)` — [`L296`](../../../../../raw/code/graphify/tests/test_multigraph_diagnostics.py#L296)
- `test_diagnose_file_explicit_directed_override(tmp_path: Path)` — [`L308`](../../../../../raw/code/graphify/tests/test_multigraph_diagnostics.py#L308)
- `test_diagnose_file_reads_json_and_formats_report(tmp_path: Path)` — [`L199`](../../../../../raw/code/graphify/tests/test_multigraph_diagnostics.py#L199)
- `test_diagnose_file_rejects_non_object_json(tmp_path: Path)` — [`L288`](../../../../../raw/code/graphify/tests/test_multigraph_diagnostics.py#L288)
- `test_diagnose_file_rejects_oversized_graph(monkeypatch, tmp_path: Path)` — [`L279`](../../../../../raw/code/graphify/tests/test_multigraph_diagnostics.py#L279)
- `test_diagnose_multigraph_cli_human_output(monkeypatch, tmp_path: Path, capsys)` — [`L328`](../../../../../raw/code/graphify/tests/test_multigraph_diagnostics.py#L328)
- `test_diagnose_multigraph_cli_json_output(monkeypatch, tmp_path: Path, capsys)` — [`L389`](../../../../../raw/code/graphify/tests/test_multigraph_diagnostics.py#L389)
- `test_diagnose_multigraph_cli_max_examples_zero(monkeypatch, tmp_path: Path, capsys)` — [`L366`](../../../../../raw/code/graphify/tests/test_multigraph_diagnostics.py#L366)
- `test_diagnose_multigraph_cli_rejects_conflicting_direction_flags(monkeypatch, tmp_path: Path, capsys)` — [`L434`](../../../../../raw/code/graphify/tests/test_multigraph_diagnostics.py#L434)
- `test_diagnose_multigraph_cli_undirected_override(monkeypatch, tmp_path: Path, capsys)` — [`L347`](../../../../../raw/code/graphify/tests/test_multigraph_diagnostics.py#L347)
- `test_diagnose_multigraph_cli_usage_errors(monkeypatch, capsys, argv_tail: list[str], expected: str)` — [`L418`](../../../../../raw/code/graphify/tests/test_multigraph_diagnostics.py#L418)
- `test_diagnostic_json_report_is_serializable(tmp_path: Path)` — [`L235`](../../../../../raw/code/graphify/tests/test_multigraph_diagnostics.py#L235)
- `test_format_diagnostic_report_includes_build_and_suppression_errors(tmp_path: Path)` — [`L215`](../../../../../raw/code/graphify/tests/test_multigraph_diagnostics.py#L215)
- `test_scan_producer_suppression_sites_finds_seen_sets(tmp_path: Path)` — [`L248`](../../../../../raw/code/graphify/tests/test_multigraph_diagnostics.py#L248)
- `test_scan_producer_suppression_sites_handles_unknown_tuple_arity(tmp_path: Path)` — [`L269`](../../../../../raw/code/graphify/tests/test_multigraph_diagnostics.py#L269)
- `test_scan_producer_suppression_sites_reports_missing_file(tmp_path: Path)` — [`L320`](../../../../../raw/code/graphify/tests/test_multigraph_diagnostics.py#L320)

