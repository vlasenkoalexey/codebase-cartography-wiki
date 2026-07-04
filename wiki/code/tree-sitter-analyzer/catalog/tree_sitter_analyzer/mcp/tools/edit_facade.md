---
title: 'Module: tree_sitter_analyzer/mcp/tools/edit_facade.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/edit_facade.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.edit_facade`/
symbols:
  build_edit_facade: build_edit_facade().
  _EDIT_DESCRIPTION: _EDIT_DESCRIPTION.
  _EDIT_ANNOTATIONS._EDIT_ANNOTATIONS: _EDIT_ANNOTATIONS._EDIT_ANNOTATIONS.
  build_edit_facade._PRReviewViaFacade: build_edit_facade()._PRReviewViaFacade#
  build_edit_facade._PRReviewViaFacade.execute: build_edit_facade()._PRReviewViaFacade#execute().
---
# Module: [`tree_sitter_analyzer/mcp/tools/edit_facade.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/edit_facade.py)

## Classes
### `_PRReviewViaFacade`  ·  implements/extends CodeGraphPRReviewTool
- def: [`tree_sitter_analyzer/mcp/tools/edit_facade.py:106`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/edit_facade.py#L106)
- doc: Facade `action=pr` implies `mode=pr`.
- signature: `class _PRReviewViaFacade(CodeGraphPRReviewTool):`
- members:
  - `execute(self, arguments: dict[str, Any])` — [`L115`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/edit_facade.py#L115)
- uses (calls/refs, reference-scoped): [`execute`](codegraph_pr_review_tool.md#CodeGraphPRReviewTool.execute), [`CodeGraphPRReviewTool`](codegraph_pr_review_tool.md#CodeGraphPRReviewTool)
- used by: [`execute`](codegraph_pr_review_tool.md#CodeGraphPRReviewTool.execute), [`build_edit_facade`](edit_facade.md#build_edit_facade), [`CodeGraphPRReviewTool`](codegraph_pr_review_tool.md#CodeGraphPRReviewTool)

## Functions
- `build_edit_facade(project_root: str | None = None)` — [`L93`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/edit_facade.py#L93) — Construct the ``edit`` facade wired to live inner tool instances. — documented in [tree_sitter_analyzer-mcp-tools-facade_tool](../../../../concepts/tree_sitter_analyzer-mcp-tools-facade_tool.md)

## Module values
- `_EDIT_ANNOTATIONS` — [`L46`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/edit_facade.py#L46)
- `_EDIT_DESCRIPTION` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/edit_facade.py#L53)

