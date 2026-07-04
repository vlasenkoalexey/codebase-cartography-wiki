---
title: 'Module: tests/integration/formatters/golden_master.py'
type: catalog
provenance: extracted
module: tests/integration/formatters/golden_master.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.formatters.golden_master`/
symbols:
  GoldenMasterTester.assert_matches_golden_master: GoldenMasterTester#assert_matches_golden_master().
  GoldenMasterManager: GoldenMasterManager#
  GoldenMasterManager.get_tester: GoldenMasterManager#get_tester().
  GoldenMasterTester: GoldenMasterTester#
  GoldenMasterManager.create_test_suite_golden_masters: GoldenMasterManager#create_test_suite_golden_masters().
  GoldenMasterTester._get_file_extension: GoldenMasterTester#_get_file_extension().
  GoldenMasterTester._generate_diff: GoldenMasterTester#_generate_diff().
  GoldenMasterTester.reference_dir: GoldenMasterTester#reference_dir.
  GoldenMasterTester.create_golden_master: GoldenMasterTester#create_golden_master().
  GoldenMasterManager._testers: GoldenMasterManager#_testers.
  GoldenMasterTester.get_golden_master_content: GoldenMasterTester#get_golden_master_content().
  GoldenMasterManager.validate_all_formats: GoldenMasterManager#validate_all_formats().
  golden_master_manager: golden_master_manager().
  full_format_golden_tester: full_format_golden_tester().
  compact_format_golden_tester: compact_format_golden_tester().
  csv_format_golden_tester: csv_format_golden_tester().
  GoldenMasterTester.format_type: GoldenMasterTester#format_type.
  GoldenMasterTester.get_content_hash: GoldenMasterTester#get_content_hash().
  _normalize_storage_newline: _normalize_storage_newline().
  GoldenMasterManager.test_data_dir: GoldenMasterManager#test_data_dir.
  GoldenMasterTester.__init__: GoldenMasterTester#__init__().
  GoldenMasterManager.__init__: GoldenMasterManager#__init__().
---
# Module: [`tests/integration/formatters/golden_master.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/golden_master.py)

## Classes
### `GoldenMasterManager`
- def: [`tests/integration/formatters/golden_master.py:161`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/golden_master.py#L161)
- doc: Manager for multiple golden master testers
- signature: `class GoldenMasterManager:`
- members:
  - `__init__(self, test_data_dir: Path | None = None)` — [`L164`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/golden_master.py#L164) — Initialize golden master manager
  - `create_test_suite_golden_masters(self, test_cases: dict[str, dict[str, str]], overwrite: bool = False)` — [`L207`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/golden_master.py#L207) — Create golden masters for a complete test suite
  - `get_tester(self, format_type: str)` — [`L176`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/golden_master.py#L176) — Get or create a golden master tester for format type
  - `validate_all_formats(self, outputs: dict[str, str], test_name: str, update_golden: bool = False)` — [`L192`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/golden_master.py#L192) — Validate outputs for all formats against golden masters
  - `test_data_dir` — [`L171`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/golden_master.py#L171)
- protocol/private: `_testers`[`L174`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/golden_master.py#L174)
- uses (calls/refs, reference-scoped): (5 test-only callers)
- used by: [`_check_format_regression`](../../../scripts/format_monitoring_tool.md#FormatMonitor._check_format_regression), [`project_root`](../../../scripts/format_monitoring_tool.md#project_root), [`project_root`](../../../scripts/format_change_management.md#project_root), [`golden_master_manager`](../../../scripts/format_monitoring_tool.md#FormatMonitor.golden_master_manager), [`golden_master_manager`](../../../scripts/format_change_management.md#FormatChangeManager.golden_master_manager)  (4 test-only)

### `GoldenMasterTester`
- def: [`tests/integration/formatters/golden_master.py:16`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/golden_master.py#L16)
- doc: Golden master testing framework for format validation
- signature: `class GoldenMasterTester:`
- members:
  - `__init__(self, format_type: str, test_data_dir: Path | None = None)` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/golden_master.py#L19) — Initialize golden master tester
  - `_generate_diff(self, expected: str, actual: str, test_name: str)` — [`L110`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/golden_master.py#L110) — Generate detailed diff between expected and actual output
  - `_get_file_extension(self)` — [`L105`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/golden_master.py#L105) — Get appropriate file extension for format type
  - `assert_matches_golden_master(self, actual_output: str, test_name: str, update_golden: bool = False)` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/golden_master.py#L33) — Compare actual output against golden master reference
  - `create_golden_master(self, content: str, test_name: str)` — [`L78`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/golden_master.py#L78) — Create a new golden master file
  - `get_content_hash(self, content: str)` — [`L93`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/golden_master.py#L93) — Generate hash of content for change detection
  - `get_golden_master_content(self, test_name: str)` — [`L63`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/golden_master.py#L63) — Get the content of a golden master file
  - `format_type` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/golden_master.py#L27)
  - `reference_dir` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/golden_master.py#L30)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: [`_check_format_regression`](../../../scripts/format_monitoring_tool.md#FormatMonitor._check_format_regression)  (9 test-only)

## Functions
- `_normalize_storage_newline(expected: str, actual: str)` — [`L154`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/golden_master.py#L154) — Allow golden files to keep a POSIX EOF newline when payloads omit it.
- `compact_format_golden_tester()` — [`L253`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/golden_master.py#L253) — Fixture providing golden master tester for compact format
- `csv_format_golden_tester()` — [`L259`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/golden_master.py#L259) — Fixture providing golden master tester for CSV format
- `full_format_golden_tester()` — [`L247`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/golden_master.py#L247) — Fixture providing golden master tester for full format
- `golden_master_manager()` — [`L241`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/golden_master.py#L241) — Fixture providing GoldenMasterManager instance

