---
title: 'Module: tree_sitter_analyzer/mcp/tools/structure_facade.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/structure_facade.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.structure_facade`/
symbols:
  build_structure_facade: build_structure_facade().
  _STRUCTURE_DESCRIPTION: _STRUCTURE_DESCRIPTION.
  build_structure_facade._read_route: build_structure_facade()._read_route().
  build_structure_facade._class_detail_route: build_structure_facade()._class_detail_route().
  build_structure_facade._read_route._as_int: build_structure_facade()._read_route()._as_int().
  build_structure_facade._signatures_route: build_structure_facade()._signatures_route().
  _STRUCTURE_ANNOTATIONS._STRUCTURE_ANNOTATIONS: _STRUCTURE_ANNOTATIONS._STRUCTURE_ANNOTATIONS.
---
# Module: [`tree_sitter_analyzer/mcp/tools/structure_facade.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/structure_facade.py)

## Functions
- `_as_int(value: Any)` — [`L170`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/structure_facade.py#L170)
- `_class_detail_route(args: dict[str, Any])` — [`L214`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/structure_facade.py#L214) — Bespoke route: normalise query/symbol → class_name before dispatch.
- `_read_route(args: dict[str, Any])` — [`L145`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/structure_facade.py#L145) — F5 bespoke: single-vs-batch reshape for extract_code_section.
- `_signatures_route(args: dict[str, Any])` — [`L126`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/structure_facade.py#L126) — Return signatures-format output for a file.
- `build_structure_facade(project_root: str | None = None)` — [`L96`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/structure_facade.py#L96) — Construct the ``structure`` facade wired to live inner tool instances. — documented in [tree_sitter_analyzer-mcp-tools-facade_tool](../../../../concepts/tree_sitter_analyzer-mcp-tools-facade_tool.md)

## Module values
- `_STRUCTURE_ANNOTATIONS` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/structure_facade.py#L45)
- `_STRUCTURE_DESCRIPTION` — [`L55`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/structure_facade.py#L55)

