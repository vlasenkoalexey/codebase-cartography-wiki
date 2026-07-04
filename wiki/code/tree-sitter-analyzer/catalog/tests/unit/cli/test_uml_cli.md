---
title: 'Module: tests/unit/cli/test_uml_cli.py'
type: catalog
provenance: extracted
module: tests/unit/cli/test_uml_cli.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.cli.test_uml_cli`/
symbols:
  test_uml_class_cli_forwards_arguments: test_uml_class_cli_forwards_arguments().
  test_uml_sequence_cli_forwards_source_target: test_uml_sequence_cli_forwards_source_target().
  test_uml_cli_forwards_file_path: test_uml_cli_forwards_file_path().
  test_uml_cli_forwards_class_name: test_uml_cli_forwards_class_name().
  test_uml_cli_forwards_include_tests: test_uml_cli_forwards_include_tests().
  test_phase1_cli_flags_registered: test_phase1_cli_flags_registered().
  _args: _args().
  test_uml_class_cli_forwards_arguments.FakeUMLTool: test_uml_class_cli_forwards_arguments().FakeUMLTool#
  test_uml_sequence_cli_forwards_source_target.FakeUMLTool: test_uml_sequence_cli_forwards_source_target().FakeUMLTool#
  test_uml_cli_forwards_file_path.FakeUMLTool: test_uml_cli_forwards_file_path().FakeUMLTool#
  test_uml_cli_forwards_class_name.FakeUMLTool: test_uml_cli_forwards_class_name().FakeUMLTool#
  test_uml_cli_forwards_include_tests.FakeUMLTool: test_uml_cli_forwards_include_tests().FakeUMLTool#
  test_uml_class_cli_forwards_arguments.FakeUMLTool.__init__: test_uml_class_cli_forwards_arguments().FakeUMLTool#__init__().
  test_uml_class_cli_forwards_arguments.FakeUMLTool.execute: test_uml_class_cli_forwards_arguments().FakeUMLTool#execute().
  test_uml_sequence_cli_forwards_source_target.FakeUMLTool.__init__: test_uml_sequence_cli_forwards_source_target().FakeUMLTool#__init__().
  test_uml_sequence_cli_forwards_source_target.FakeUMLTool.execute: test_uml_sequence_cli_forwards_source_target().FakeUMLTool#execute().
  test_uml_cli_forwards_file_path.FakeUMLTool.__init__: test_uml_cli_forwards_file_path().FakeUMLTool#__init__().
  test_uml_cli_forwards_file_path.FakeUMLTool.execute: test_uml_cli_forwards_file_path().FakeUMLTool#execute().
  test_uml_cli_forwards_class_name.FakeUMLTool.__init__: test_uml_cli_forwards_class_name().FakeUMLTool#__init__().
  test_uml_cli_forwards_class_name.FakeUMLTool.execute: test_uml_cli_forwards_class_name().FakeUMLTool#execute().
  test_uml_cli_forwards_include_tests.FakeUMLTool.__init__: test_uml_cli_forwards_include_tests().FakeUMLTool#__init__().
  test_uml_cli_forwards_include_tests.FakeUMLTool.execute: test_uml_cli_forwards_include_tests().FakeUMLTool#execute().
---
# Module: [`tests/unit/cli/test_uml_cli.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_uml_cli.py)

## Classes
### `FakeUMLTool`
- def: [`tests/unit/cli/test_uml_cli.py:201`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_uml_cli.py#L201)
- signature: `class FakeUMLTool:`
- members:
  - `execute(self, arguments: dict[str, Any])` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_uml_cli.py#L35)
  - `execute(self, arguments: dict[str, Any])` — [`L72`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_uml_cli.py#L72)
  - `execute(self, arguments: dict[str, Any])` — [`L122`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_uml_cli.py#L122)
  - `execute(self, arguments: dict[str, Any])` — [`L164`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_uml_cli.py#L164)
  - `execute(self, arguments: dict[str, Any])` — [`L205`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_uml_cli.py#L205)
- protocol/private: `__init__`[`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_uml_cli.py#L32), `__init__`[`L69`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_uml_cli.py#L69), `__init__`[`L119`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_uml_cli.py#L119), `__init__`[`L161`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_uml_cli.py#L161), `__init__`[`L202`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_uml_cli.py#L202)
- used by: (1 test-only callers)

## Functions
- `_args(**overrides: Any)` — [`L11`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_uml_cli.py#L11)
- `test_phase1_cli_flags_registered()` — [`L102`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_uml_cli.py#L102) — Phase-1 flags must be registered in the argument parser.
- `test_uml_class_cli_forwards_arguments(monkeypatch)` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_uml_cli.py#L28)
- `test_uml_cli_forwards_class_name(monkeypatch)` — [`L156`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_uml_cli.py#L156) — --uml-class-name is wired through _build_uml_tool_args → execute.
- `test_uml_cli_forwards_file_path(monkeypatch)` — [`L114`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_uml_cli.py#L114) — --uml-file-path is wired through _build_uml_tool_args → execute.
- `test_uml_cli_forwards_include_tests(monkeypatch)` — [`L197`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_uml_cli.py#L197) — --uml-include-tests is wired through _build_uml_tool_args → execute.
- `test_uml_sequence_cli_forwards_source_target(monkeypatch)` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_uml_cli.py#L65)

