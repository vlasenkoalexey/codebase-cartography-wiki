---
title: 'Module: tests/unit/test_uml_tool.py'
type: catalog
provenance: extracted
module: tests/unit/test_uml_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_uml_tool`/test_
symbols:
  test_execute_dispatches_non_class_diagrams.FakeExporter._diagram: execute_dispatches_non_class_diagrams().FakeExporter#_diagram().
  test_class_diagram_execute_with_mock_exporter.FakeExporter.class_diagram: class_diagram_execute_with_mock_exporter().FakeExporter#class_diagram().
  test_class_diagram_execute_with_mock_exporter: class_diagram_execute_with_mock_exporter().
  test_execute_dispatches_non_class_diagrams: execute_dispatches_non_class_diagrams().
  test_uml_tool_definition: uml_tool_definition().
  test_uml_tool_schema_lists_diagrams: uml_tool_schema_lists_diagrams().
  test_sequence_requires_source_and_target: sequence_requires_source_and_target().
  test_positive_integer_validation: positive_integer_validation().
  test_unsupported_diagram_validation: unsupported_diagram_validation().
  test_execute_dispatches_non_class_diagrams.FakeExporter.package_diagram: execute_dispatches_non_class_diagrams().FakeExporter#package_diagram().
  test_execute_dispatches_non_class_diagrams.FakeExporter.component_diagram: execute_dispatches_non_class_diagrams().FakeExporter#component_diagram().
  test_execute_dispatches_non_class_diagrams.FakeExporter.sequence_diagram: execute_dispatches_non_class_diagrams().FakeExporter#sequence_diagram().
  test_no_project_root_returns_error: no_project_root_returns_error().
  test_class_diagram_execute_with_mock_exporter.FakeHub.uml_exporter: class_diagram_execute_with_mock_exporter().FakeHub#uml_exporter().
  test_execute_dispatches_non_class_diagrams.FakeHub.uml_exporter: execute_dispatches_non_class_diagrams().FakeHub#uml_exporter().
  test_class_diagram_execute_with_mock_exporter.FakeExporter: class_diagram_execute_with_mock_exporter().FakeExporter#
  test_execute_dispatches_non_class_diagrams.FakeExporter: execute_dispatches_non_class_diagrams().FakeExporter#
  test_class_diagram_execute_with_mock_exporter.FakeHub: class_diagram_execute_with_mock_exporter().FakeHub#
  test_execute_dispatches_non_class_diagrams.FakeHub: execute_dispatches_non_class_diagrams().FakeHub#
  test_class_diagram_execute_with_mock_exporter.FakeHub.__init__: class_diagram_execute_with_mock_exporter().FakeHub#__init__().
  test_execute_dispatches_non_class_diagrams.FakeHub.__init__: execute_dispatches_non_class_diagrams().FakeHub#__init__().
---
# Module: [`tests/unit/test_uml_tool.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_tool.py)

## Classes
### `FakeExporter`
- def: [`tests/unit/test_uml_tool.py:123`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_tool.py#L123)
- signature: `class FakeExporter:`
- members:
  - `class_diagram(self, max_edges: int, include_external_bases: bool, *, file_path: str | None = None, class_name: str | None = None, include_tests: bool = False)` — [`L62`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_tool.py#L62)
  - `component_diagram(self, max_edges: int)` — [`L128`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_tool.py#L128)
  - `package_diagram(self, max_edges: int, package_depth: int)` — [`L124`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_tool.py#L124)
  - `sequence_diagram(self, source: str, target: str, max_depth: int, max_paths: int)` — [`L132`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_tool.py#L132)
- protocol/private: `_diagram`[`L147`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_tool.py#L147)
- uses (calls/refs, reference-scoped): [`UMLEdge`](../../tree_sitter_analyzer/uml_export.md#UMLEdge), [`mermaid`](../../tree_sitter_analyzer/uml_export.md#UMLDiagram.mermaid), [`nodes`](../../tree_sitter_analyzer/uml_export.md#UMLDiagram.nodes), [`UMLDiagram`](../../tree_sitter_analyzer/uml_export.md#UMLDiagram), [`edges`](../../tree_sitter_analyzer/uml_export.md#UMLDiagram.edges), [`diagram_type`](../../tree_sitter_analyzer/uml_export.md#UMLDiagram.diagram_type), [`mermaid_type`](../../tree_sitter_analyzer/uml_export.md#UMLDiagram.mermaid_type)
- used by: (1 test-only callers)

### `FakeHub`
- def: [`tests/unit/test_uml_tool.py:158`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_tool.py#L158)
- signature: `class FakeHub:`
- members:
  - `uml_exporter(self)` — [`L85`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_tool.py#L85)
  - `uml_exporter(self)` — [`L162`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_tool.py#L162)
- protocol/private: `__init__`[`L82`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_tool.py#L82), `__init__`[`L159`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_tool.py#L159)
- uses (calls/refs, reference-scoped): (2 test-only callers)
- used by: (1 test-only callers)

## Functions
- `test_class_diagram_execute_with_mock_exporter(monkeypatch)` — [`L57`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_tool.py#L57)
- `test_execute_dispatches_non_class_diagrams(monkeypatch, diagram: str, expected_mermaid: str)` — [`L115`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_tool.py#L115)
- `test_no_project_root_returns_error()` — [`L185`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_tool.py#L185)
- `test_positive_integer_validation()` — [`L42`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_tool.py#L42)
- `test_sequence_requires_source_and_target()` — [`L35`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_tool.py#L35)
- `test_uml_tool_definition()` — [`L10`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_tool.py#L10)
- `test_uml_tool_schema_lists_diagrams()` — [`L19`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_tool.py#L19)
- `test_unsupported_diagram_validation()` — [`L49`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_tool.py#L49)

