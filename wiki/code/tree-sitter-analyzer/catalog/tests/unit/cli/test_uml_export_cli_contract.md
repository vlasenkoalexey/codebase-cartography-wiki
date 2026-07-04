---
title: 'Module: tests/unit/cli/test_uml_export_cli_contract.py'
type: catalog
provenance: extracted
module: tests/unit/cli/test_uml_export_cli_contract.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.cli.test_uml_export_cli_contract`/
symbols:
  test_existing_class_hierarchy_all_mode_is_uml_class_source: test_existing_class_hierarchy_all_mode_is_uml_class_source().
  test_existing_codegraph_visualize_cli_maps_function_diagram_inputs: test_existing_codegraph_visualize_cli_maps_function_diagram_inputs().
  test_codegraph_visualize_cli_maps_sigma_format: test_codegraph_visualize_cli_maps_sigma_format().
  test_uml_cli_delegates_to_codegraph_uml_tool: test_uml_cli_delegates_to_codegraph_uml_tool().
  test_uml_sequence_cli_forwards_source_target_and_path_limits: test_uml_sequence_cli_forwards_source_target_and_path_limits().
  _args: _args().
  test_uml_parser_accepts_phase1_diagram_types: test_uml_parser_accepts_phase1_diagram_types().
  test_uml_parser_accepts_sequence_source_target_and_limits: test_uml_parser_accepts_sequence_source_target_and_limits().
  test_codegraph_visualize_parser_accepts_sigma_format: test_codegraph_visualize_parser_accepts_sigma_format().
  test_uml_parser_accepts_package_and_class_tuning_flags: test_uml_parser_accepts_package_and_class_tuning_flags().
  test_existing_class_hierarchy_all_mode_is_uml_class_source.FakeClassHierarchyTool: test_existing_class_hierarchy_all_mode_is_uml_class_source().FakeClassHierarchyTool#
  test_existing_codegraph_visualize_cli_maps_function_diagram_inputs.FakeCodeGraphVisualizeTool: test_existing_codegraph_visualize_cli_maps_function_diagram_inputs().FakeCodeGraphVisualizeTool#
  test_codegraph_visualize_cli_maps_sigma_format.FakeCodeGraphVisualizeTool: test_codegraph_visualize_cli_maps_sigma_format().FakeCodeGraphVisualizeTool#
  test_uml_cli_delegates_to_codegraph_uml_tool.FakeUMLTool: test_uml_cli_delegates_to_codegraph_uml_tool().FakeUMLTool#
  test_uml_sequence_cli_forwards_source_target_and_path_limits.FakeUMLTool: test_uml_sequence_cli_forwards_source_target_and_path_limits().FakeUMLTool#
  test_existing_class_hierarchy_all_mode_is_uml_class_source.FakeClassHierarchyTool.__init__: test_existing_class_hierarchy_all_mode_is_uml_class_source().FakeClassHierarchyTool#__init__().
  test_existing_class_hierarchy_all_mode_is_uml_class_source.FakeClassHierarchyTool.execute: test_existing_class_hierarchy_all_mode_is_uml_class_source().FakeClassHierarchyTool#execute().
  test_existing_codegraph_visualize_cli_maps_function_diagram_inputs.FakeCodeGraphVisualizeTool.__init__: test_existing_codegraph_visualize_cli_maps_function_diagram_inputs().FakeCodeGraphVisualizeTool#__init__().
  test_existing_codegraph_visualize_cli_maps_function_diagram_inputs.FakeCodeGraphVisualizeTool.execute: test_existing_codegraph_visualize_cli_maps_function_diagram_inputs().FakeCodeGraphVisualizeTool#execute().
  test_codegraph_visualize_cli_maps_sigma_format.FakeCodeGraphVisualizeTool.__init__: test_codegraph_visualize_cli_maps_sigma_format().FakeCodeGraphVisualizeTool#__init__().
  test_codegraph_visualize_cli_maps_sigma_format.FakeCodeGraphVisualizeTool.execute: test_codegraph_visualize_cli_maps_sigma_format().FakeCodeGraphVisualizeTool#execute().
  test_uml_cli_delegates_to_codegraph_uml_tool.FakeUMLTool.__init__: test_uml_cli_delegates_to_codegraph_uml_tool().FakeUMLTool#__init__().
  test_uml_cli_delegates_to_codegraph_uml_tool.FakeUMLTool.execute: test_uml_cli_delegates_to_codegraph_uml_tool().FakeUMLTool#execute().
  test_uml_sequence_cli_forwards_source_target_and_path_limits.FakeUMLTool.__init__: test_uml_sequence_cli_forwards_source_target_and_path_limits().FakeUMLTool#__init__().
  test_uml_sequence_cli_forwards_source_target_and_path_limits.FakeUMLTool.execute: test_uml_sequence_cli_forwards_source_target_and_path_limits().FakeUMLTool#execute().
---
# Module: [`tests/unit/cli/test_uml_export_cli_contract.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_uml_export_cli_contract.py)

## Classes
### `FakeClassHierarchyTool`
- def: [`tests/unit/cli/test_uml_export_cli_contract.py:48`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_uml_export_cli_contract.py#L48)
- signature: `class FakeClassHierarchyTool:`
- members:
  - `execute(self, arguments: dict[str, Any])` — [`L52`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_uml_export_cli_contract.py#L52)
- protocol/private: `__init__`[`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_uml_export_cli_contract.py#L49)
- used by: (1 test-only callers)

### `FakeCodeGraphVisualizeTool`
- def: [`tests/unit/cli/test_uml_export_cli_contract.py:129`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_uml_export_cli_contract.py#L129)
- signature: `class FakeCodeGraphVisualizeTool:`
- members:
  - `execute(self, arguments: dict[str, Any])` — [`L86`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_uml_export_cli_contract.py#L86)
  - `execute(self, arguments: dict[str, Any])` — [`L133`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_uml_export_cli_contract.py#L133)
- protocol/private: `__init__`[`L83`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_uml_export_cli_contract.py#L83), `__init__`[`L130`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_uml_export_cli_contract.py#L130)
- used by: (1 test-only callers)

### `FakeUMLTool`
- def: [`tests/unit/cli/test_uml_export_cli_contract.py:277`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_uml_export_cli_contract.py#L277)
- signature: `class FakeUMLTool:`
- members:
  - `execute(self, arguments: dict[str, Any])` — [`L237`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_uml_export_cli_contract.py#L237)
  - `execute(self, arguments: dict[str, Any])` — [`L281`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_uml_export_cli_contract.py#L281)
- protocol/private: `__init__`[`L234`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_uml_export_cli_contract.py#L234), `__init__`[`L278`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_uml_export_cli_contract.py#L278)
- used by: (1 test-only callers)

## Functions
- `_args(**overrides: Any)` — [`L14`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_uml_export_cli_contract.py#L14)
- `test_codegraph_visualize_cli_maps_sigma_format(monkeypatch: pytest.MonkeyPatch)` — [`L124`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_uml_export_cli_contract.py#L124)
- `test_codegraph_visualize_parser_accepts_sigma_format()` — [`L199`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_uml_export_cli_contract.py#L199)
- `test_existing_class_hierarchy_all_mode_is_uml_class_source(monkeypatch: pytest.MonkeyPatch)` — [`L43`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_uml_export_cli_contract.py#L43)
- `test_existing_codegraph_visualize_cli_maps_function_diagram_inputs(monkeypatch: pytest.MonkeyPatch)` — [`L77`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_uml_export_cli_contract.py#L77)
- `test_uml_cli_delegates_to_codegraph_uml_tool(monkeypatch: pytest.MonkeyPatch)` — [`L228`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_uml_export_cli_contract.py#L228)
- `test_uml_parser_accepts_package_and_class_tuning_flags()` — [`L210`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_uml_export_cli_contract.py#L210)
- `test_uml_parser_accepts_phase1_diagram_types(diagram: str)` — [`L165`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_uml_export_cli_contract.py#L165)
- `test_uml_parser_accepts_sequence_source_target_and_limits()` — [`L174`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_uml_export_cli_contract.py#L174)
- `test_uml_sequence_cli_forwards_source_target_and_path_limits(monkeypatch: pytest.MonkeyPatch)` — [`L272`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_uml_export_cli_contract.py#L272)

