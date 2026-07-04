---
title: 'Module: tests/unit/cli/test_codegraph_index_commands.py'
type: catalog
provenance: extracted
module: tests/unit/cli/test_codegraph_index_commands.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.cli.test_codegraph_index_commands`/
symbols:
  _args: _args().
  TestRunAutoindex.test_success_returns_0: TestRunAutoindex#test_success_returns_0().
  TestRunFullIndex.test_success_returns_0: TestRunFullIndex#test_success_returns_0().
  TestRunIncrementalSync.test_success_returns_0: TestRunIncrementalSync#test_success_returns_0().
  TestRunKnowledgeGraphIndex.test_success_returns_0: TestRunKnowledgeGraphIndex#test_success_returns_0().
  TestRunCodegraphMetrics.test_success_with_sections: TestRunCodegraphMetrics#test_success_with_sections().
  TestRunAutoindex.test_execute_failure_returns_1: TestRunAutoindex#test_execute_failure_returns_1().
  TestRunFullIndex.test_execute_failure_returns_1: TestRunFullIndex#test_execute_failure_returns_1().
  TestRunIncrementalSync.test_execute_failure_returns_1: TestRunIncrementalSync#test_execute_failure_returns_1().
  TestRunKnowledgeGraphIndex.test_execute_failure_returns_1: TestRunKnowledgeGraphIndex#test_execute_failure_returns_1().
  TestRunCodegraphMetrics.test_execute_failure_returns_1: TestRunCodegraphMetrics#test_execute_failure_returns_1().
  TestProjectRoot.test_returns_project_root_attr: TestProjectRoot#test_returns_project_root_attr().
  TestProjectRoot.test_falls_back_to_cwd_when_none: TestProjectRoot#test_falls_back_to_cwd_when_none().
  TestProjectRoot.test_falls_back_to_cwd_when_missing: TestProjectRoot#test_falls_back_to_cwd_when_missing().
  TestAutoindexPayload.test_default_values: TestAutoindexPayload#test_default_values().
  TestAutoindexPayload.test_custom_mode: TestAutoindexPayload#test_custom_mode().
  TestAutoindexPayload.test_empty_mode_falls_back_to_status: TestAutoindexPayload#test_empty_mode_falls_back_to_status().
  TestFullIndexPayload.test_default_values: TestFullIndexPayload#test_default_values().
  TestFullIndexPayload.test_include_activation_true: TestFullIndexPayload#test_include_activation_true().
  TestIncrementalSyncPayload.test_default_values: TestIncrementalSyncPayload#test_default_values().
  TestIncrementalSyncPayload.test_custom_mode: TestIncrementalSyncPayload#test_custom_mode().
  TestKnowledgeGraphIndexPayload.test_default_values: TestKnowledgeGraphIndexPayload#test_default_values().
  TestKnowledgeGraphIndexPayload.test_custom_values: TestKnowledgeGraphIndexPayload#test_custom_values().
  TestMetricsPayload.test_no_sections: TestMetricsPayload#test_no_sections().
  TestMetricsPayload.test_with_sections: TestMetricsPayload#test_with_sections().
  _OUTPUT_FMT: _OUTPUT_FMT.
  TestRunAutoindex.test_import_error_returns_1: TestRunAutoindex#test_import_error_returns_1().
  TestExitCodeFor.test_returns_0_on_success: TestExitCodeFor#test_returns_0_on_success().
  TestExitCodeFor.test_returns_1_on_failure: TestExitCodeFor#test_returns_1_on_failure().
  TestExitCodeFor.test_returns_1_when_key_missing: TestExitCodeFor#test_returns_1_when_key_missing().
  TestPrint.test_toon_format_prints_toon_content: TestPrint#test_toon_format_prints_toon_content().
  TestPrint.test_json_format_prints_json: TestPrint#test_json_format_prints_json().
  TestPrint.test_toon_format_missing_key_prints_empty: TestPrint#test_toon_format_missing_key_prints_empty().
  _AUTOINDEX_CLS: _AUTOINDEX_CLS.
  _FULLINDEX_CLS: _FULLINDEX_CLS.
  _INCSYNC_CLS: _INCSYNC_CLS.
  _METRICS_CLS: _METRICS_CLS.
  _KNOWLEDGE_INDEX_CLS: _KNOWLEDGE_INDEX_CLS.
  TestProjectRoot: TestProjectRoot#
  TestExitCodeFor: TestExitCodeFor#
  TestPrint: TestPrint#
  TestAutoindexPayload: TestAutoindexPayload#
  TestFullIndexPayload: TestFullIndexPayload#
  TestIncrementalSyncPayload: TestIncrementalSyncPayload#
  TestKnowledgeGraphIndexPayload: TestKnowledgeGraphIndexPayload#
  TestMetricsPayload: TestMetricsPayload#
  TestRunAutoindex: TestRunAutoindex#
  TestRunFullIndex: TestRunFullIndex#
  TestRunIncrementalSync: TestRunIncrementalSync#
  TestRunKnowledgeGraphIndex: TestRunKnowledgeGraphIndex#
  TestRunCodegraphMetrics: TestRunCodegraphMetrics#
---
# Module: [`tests/unit/cli/test_codegraph_index_commands.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_codegraph_index_commands.py)

## Classes
### `TestAutoindexPayload`
- def: [`tests/unit/cli/test_codegraph_index_commands.py:99`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_codegraph_index_commands.py#L99)
- signature: `class TestAutoindexPayload:`
- members:
  - `test_custom_mode(self)` — [`L107`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_codegraph_index_commands.py#L107)
  - `test_default_values(self)` — [`L100`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_codegraph_index_commands.py#L100)
  - `test_empty_mode_falls_back_to_status(self)` — [`L113`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_codegraph_index_commands.py#L113)
- uses (calls/refs, reference-scoped): [`_autoindex_payload`](../../../tree_sitter_analyzer/cli/commands/codegraph_index_commands.md#_autoindex_payload)  (1 test-only)

### `TestExitCodeFor`
- def: [`tests/unit/cli/test_codegraph_index_commands.py:60`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_codegraph_index_commands.py#L60)
- signature: `class TestExitCodeFor:`
- members:
  - `test_returns_0_on_success(self)` — [`L61`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_codegraph_index_commands.py#L61)
  - `test_returns_1_on_failure(self)` — [`L64`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_codegraph_index_commands.py#L64)
  - `test_returns_1_when_key_missing(self)` — [`L67`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_codegraph_index_commands.py#L67)
- uses (calls/refs, reference-scoped): [`_exit_code_for`](../../../tree_sitter_analyzer/cli/commands/codegraph_index_commands.md#_exit_code_for)

### `TestFullIndexPayload`
- def: [`tests/unit/cli/test_codegraph_index_commands.py:119`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_codegraph_index_commands.py#L119)
- signature: `class TestFullIndexPayload:`
- members:
  - `test_default_values(self)` — [`L120`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_codegraph_index_commands.py#L120)
  - `test_include_activation_true(self)` — [`L128`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_codegraph_index_commands.py#L128)
- uses (calls/refs, reference-scoped): [`_full_index_payload`](../../../tree_sitter_analyzer/cli/commands/codegraph_index_commands.md#_full_index_payload)  (1 test-only)

### `TestIncrementalSyncPayload`
- def: [`tests/unit/cli/test_codegraph_index_commands.py:134`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_codegraph_index_commands.py#L134)
- signature: `class TestIncrementalSyncPayload:`
- members:
  - `test_custom_mode(self)` — [`L141`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_codegraph_index_commands.py#L141)
  - `test_default_values(self)` — [`L135`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_codegraph_index_commands.py#L135)
- uses (calls/refs, reference-scoped): [`_incremental_sync_payload`](../../../tree_sitter_analyzer/cli/commands/codegraph_index_commands.md#_incremental_sync_payload)  (1 test-only)

### `TestKnowledgeGraphIndexPayload`
- def: [`tests/unit/cli/test_codegraph_index_commands.py:147`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_codegraph_index_commands.py#L147)
- signature: `class TestKnowledgeGraphIndexPayload:`
- members:
  - `test_custom_values(self)` — [`L159`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_codegraph_index_commands.py#L159)
  - `test_default_values(self)` — [`L148`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_codegraph_index_commands.py#L148)
- uses (calls/refs, reference-scoped): [`_knowledge_graph_index_payload`](../../../tree_sitter_analyzer/cli/commands/codegraph_index_commands.md#_knowledge_graph_index_payload)  (1 test-only)

### `TestMetricsPayload`
- def: [`tests/unit/cli/test_codegraph_index_commands.py:178`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_codegraph_index_commands.py#L178)
- signature: `class TestMetricsPayload:`
- members:
  - `test_no_sections(self)` — [`L179`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_codegraph_index_commands.py#L179)
  - `test_with_sections(self)` — [`L185`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_codegraph_index_commands.py#L185)
- uses (calls/refs, reference-scoped): [`_metrics_payload`](../../../tree_sitter_analyzer/cli/commands/codegraph_index_commands.md#_metrics_payload)  (1 test-only)

### `TestPrint`
- def: [`tests/unit/cli/test_codegraph_index_commands.py:76`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_codegraph_index_commands.py#L76)
- signature: `class TestPrint:`
- members:
  - `test_json_format_prints_json(self, capsys)` — [`L82`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_codegraph_index_commands.py#L82)
  - `test_toon_format_missing_key_prints_empty(self, capsys)` — [`L88`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_codegraph_index_commands.py#L88)
  - `test_toon_format_prints_toon_content(self, capsys)` — [`L77`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_codegraph_index_commands.py#L77)
- uses (calls/refs, reference-scoped): [`_print`](../../../tree_sitter_analyzer/cli/commands/codegraph_index_commands.md#_print)

### `TestProjectRoot`
- def: [`tests/unit/cli/test_codegraph_index_commands.py:38`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_codegraph_index_commands.py#L38)
- signature: `class TestProjectRoot:`
- members:
  - `test_falls_back_to_cwd_when_missing(self, monkeypatch)` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_codegraph_index_commands.py#L49)
  - `test_falls_back_to_cwd_when_none(self, monkeypatch, tmp_path)` — [`L43`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_codegraph_index_commands.py#L43)
  - `test_returns_project_root_attr(self)` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_codegraph_index_commands.py#L39)
- uses (calls/refs, reference-scoped): [`_project_root`](../../../tree_sitter_analyzer/cli/commands/codegraph_index_commands.md#_project_root)  (1 test-only)

### `TestRunAutoindex`
- def: [`tests/unit/cli/test_codegraph_index_commands.py:212`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_codegraph_index_commands.py#L212)
- signature: `class TestRunAutoindex:`
- members:
  - `test_execute_failure_returns_1(self, tmp_path)` — [`L225`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_codegraph_index_commands.py#L225)
  - `test_import_error_returns_1(self, tmp_path)` — [`L213`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_codegraph_index_commands.py#L213) — Module absent from sys.modules → import failure → return 1.
  - `test_success_returns_0(self, tmp_path, capsys)` — [`L239`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_codegraph_index_commands.py#L239)
- uses (calls/refs, reference-scoped): [`run_autoindex`](../../../tree_sitter_analyzer/cli/commands/codegraph_index_commands.md#run_autoindex)  (3 test-only)

### `TestRunCodegraphMetrics`
- def: [`tests/unit/cli/test_codegraph_index_commands.py:349`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_codegraph_index_commands.py#L349)
- signature: `class TestRunCodegraphMetrics:`
- members:
  - `test_execute_failure_returns_1(self, tmp_path)` — [`L350`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_codegraph_index_commands.py#L350)
  - `test_success_with_sections(self, tmp_path, capsys)` — [`L360`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_codegraph_index_commands.py#L360)
- uses (calls/refs, reference-scoped): [`run_codegraph_metrics`](../../../tree_sitter_analyzer/cli/commands/codegraph_index_commands.md#run_codegraph_metrics)  (3 test-only)

### `TestRunFullIndex`
- def: [`tests/unit/cli/test_codegraph_index_commands.py:259`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_codegraph_index_commands.py#L259)
- signature: `class TestRunFullIndex:`
- members:
  - `test_execute_failure_returns_1(self, tmp_path)` — [`L260`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_codegraph_index_commands.py#L260)
  - `test_success_returns_0(self, tmp_path, capsys)` — [`L270`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_codegraph_index_commands.py#L270)
- uses (calls/refs, reference-scoped): [`run_full_index`](../../../tree_sitter_analyzer/cli/commands/codegraph_index_commands.md#run_full_index)  (3 test-only)

### `TestRunIncrementalSync`
- def: [`tests/unit/cli/test_codegraph_index_commands.py:288`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_codegraph_index_commands.py#L288)
- signature: `class TestRunIncrementalSync:`
- members:
  - `test_execute_failure_returns_1(self, tmp_path)` — [`L289`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_codegraph_index_commands.py#L289)
  - `test_success_returns_0(self, tmp_path)` — [`L299`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_codegraph_index_commands.py#L299)
- uses (calls/refs, reference-scoped): [`run_incremental_sync`](../../../tree_sitter_analyzer/cli/commands/codegraph_index_commands.md#run_incremental_sync)  (3 test-only)

### `TestRunKnowledgeGraphIndex`
- def: [`tests/unit/cli/test_codegraph_index_commands.py:317`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_codegraph_index_commands.py#L317)
- signature: `class TestRunKnowledgeGraphIndex:`
- members:
  - `test_execute_failure_returns_1(self, tmp_path)` — [`L318`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_codegraph_index_commands.py#L318)
  - `test_success_returns_0(self, tmp_path, capsys)` — [`L329`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_codegraph_index_commands.py#L329)
- uses (calls/refs, reference-scoped): [`run_knowledge_graph_index`](../../../tree_sitter_analyzer/cli/commands/codegraph_index_commands.md#run_knowledge_graph_index)  (3 test-only)

## Functions
- `_args(**kwargs: object)` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_codegraph_index_commands.py#L29)

## Module values
- `_AUTOINDEX_CLS` — [`L196`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_codegraph_index_commands.py#L196)
- `_FULLINDEX_CLS` — [`L197`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_codegraph_index_commands.py#L197)
- `_INCSYNC_CLS` — [`L198`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_codegraph_index_commands.py#L198)
- `_KNOWLEDGE_INDEX_CLS` — [`L204`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_codegraph_index_commands.py#L204)
- `_METRICS_CLS` — [`L201`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_codegraph_index_commands.py#L201)
- `_OUTPUT_FMT` — [`L207`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_codegraph_index_commands.py#L207)

