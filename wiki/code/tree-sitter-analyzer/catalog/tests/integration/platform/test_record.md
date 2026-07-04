---
title: 'Module: tests/integration/platform/test_record.py'
type: catalog
provenance: extracted
module: tests/integration/platform/test_record.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.platform.test_record`/TestRecordCLI#
symbols:
  TestRecordCLI.test_main_success: test_main_success().
  TestRecordCLI.test_main_with_default_output_dir: test_main_with_default_output_dir().
  TestRecordCLI.test_main_failure_exits: test_main_failure_exits().
  TestRecordCLI: ''
  TestRecordCLI.test_module_runnable_as_main: test_module_runnable_as_main().
  TestRecordCLI.test_main_importable: test_main_importable().
---
# Module: [`tests/integration/platform/test_record.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/platform/test_record.py)

## Classes
### `TestRecordCLI`
- def: [`tests/integration/platform/test_record.py:9`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/platform/test_record.py#L9)
- doc: Test the record CLI tool functions.
- signature: `class TestRecordCLI:`
- members:
  - `test_main_failure_exits(self, tmp_path)` — [`L55`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/platform/test_record.py#L55) — Test that errors cause sys.exit(1).
  - `test_main_importable(self)` — [`L79`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/platform/test_record.py#L79)
  - `test_main_success(self, tmp_path)` — [`L12`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/platform/test_record.py#L12) — Test successful profile recording.
  - `test_main_with_default_output_dir(self)` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/platform/test_record.py#L33) — Test recording with default output directory.
  - `test_module_runnable_as_main(self)` — [`L72`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/platform/test_record.py#L72) — Test that module can be run as __main__.
- uses (calls/refs, reference-scoped): [`main`](../../../tree_sitter_analyzer/platform_compat/record.md#main)

