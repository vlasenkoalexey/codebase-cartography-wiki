---
title: 'Module: tree_sitter_analyzer/mcp/tools/semantic_classify_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/semantic_classify_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.semantic_classify_tool`/
symbols:
  SemanticClassifyTool: SemanticClassifyTool#
  SemanticClassifyTool.execute: SemanticClassifyTool#execute().
  _compact_hunk: _compact_hunk().
  _compact_classification: _compact_classification().
  SemanticClassifyTool.validate_arguments: SemanticClassifyTool#validate_arguments().
  SemanticClassifyTool._diff_git: SemanticClassifyTool#_diff_git().
  SemanticClassifyTool._get_differ: SemanticClassifyTool#_get_differ().
  SemanticClassifyTool._resolve_mode: SemanticClassifyTool#_resolve_mode().
  SemanticClassifyTool.__init__: SemanticClassifyTool#__init__().
  SemanticClassifyTool._differ: SemanticClassifyTool#_differ.
  SemanticClassifyTool.get_tool_schema: SemanticClassifyTool#get_tool_schema().
  SemanticClassifyTool.get_tool_definition: SemanticClassifyTool#get_tool_definition().
  logger: logger.
  SemanticClassifyTool._on_project_root_changed: SemanticClassifyTool#_on_project_root_changed().
  _strip_children: _strip_children().
  _DEFAULT_HUNK_CAP: _DEFAULT_HUNK_CAP.
---
# Module: [`tree_sitter_analyzer/mcp/tools/semantic_classify_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/semantic_classify_tool.py)

## Classes
### `SemanticClassifyTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/semantic_classify_tool.py:66`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/semantic_classify_tool.py#L66)
- doc: MCP Tool for semantic change classification.
- signature: `class SemanticClassifyTool(BaseMCPTool):`
- members:
  - `_resolve_mode(arguments: dict[str, Any])` — [`L174`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/semantic_classify_tool.py#L174) — Effective mode.
  - `execute(self, arguments: dict[str, Any])` — [`L211`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/semantic_classify_tool.py#L211) — documented in [tree_sitter_analyzer-ast_diff](../../../../concepts/tree_sitter_analyzer-ast_diff.md)
  - `get_tool_definition(self)` — [`L81`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/semantic_classify_tool.py#L81)
  - `get_tool_schema(self)` — [`L99`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/semantic_classify_tool.py#L99)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L194`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/semantic_classify_tool.py#L194)
- protocol/private: `__init__`[`L69`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/semantic_classify_tool.py#L69), `_diff_git`[`L295`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/semantic_classify_tool.py#L295), `_differ`[`L70`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/semantic_classify_tool.py#L70), `_get_differ`[`L76`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/semantic_classify_tool.py#L76), `_on_project_root_changed`[`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/semantic_classify_tool.py#L73)
- uses (calls/refs, reference-scoped): [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`apply_toon_format_to_response`](../utils/format_helper.md#apply_toon_format_to_response), [`diff_strings`](../../ast_diff.md#ASTDiffer.diff_strings), [`_language_from_ext`](../../project_graph.md#_language_from_ext), [`__init__`](base_tool.md#BaseMCPTool.__init__), [`classify`](../../semantic_change_classifier.md#SemanticChangeClassifier.classify), [`to_dict`](../../semantic_change_classifier.md#SemanticClassification.to_dict), [`ASTDiffer`](../../ast_diff.md#ASTDiffer), [`SemanticChangeClassifier`](../../semantic_change_classifier.md#SemanticChangeClassifier), [`hunks`](../../ast_diff.md#ASTDiffResult.hunks), [`_compact_classification`](semantic_classify_tool.md#_compact_classification)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`_on_project_root_changed`](base_tool.md#BaseMCPTool._on_project_root_changed), [`build_edit_facade`](edit_facade.md#build_edit_facade)  (26 test-only)

## Functions
- `_compact_classification(entry: dict[str, Any], *, include_ast_nodes: bool)` — [`L44`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/semantic_classify_tool.py#L44) — Return a compact version of a ClassifiedHunk dict.
- `_compact_hunk(hunk_dict: dict[str, Any])` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/semantic_classify_tool.py#L33) — Strip children from hunk.old / hunk.new so only the top-level node is kept.
- `_strip_children(node_dict: dict[str, Any])` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/semantic_classify_tool.py#L28) — Return a copy of a serialised ASTNodeInfo without the recursive children list.

## Module values
- `_DEFAULT_HUNK_CAP` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/semantic_classify_tool.py#L25)
- `logger` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/semantic_classify_tool.py#L22)

