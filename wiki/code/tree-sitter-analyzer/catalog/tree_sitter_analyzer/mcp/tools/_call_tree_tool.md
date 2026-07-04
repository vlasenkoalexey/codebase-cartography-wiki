---
title: 'Module: tree_sitter_analyzer/mcp/tools/_call_tree_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/_call_tree_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools._call_tree_tool`/
symbols:
  _CallTreeBase.execute: _CallTreeBase#execute().
  _CallTreeBase._make_expander: _CallTreeBase#_make_expander().
  CodeGraphCalleeTreeTool: CodeGraphCalleeTreeTool#
  _CallTreeBase: _CallTreeBase#
  CodeGraphCallerTreeTool: CodeGraphCallerTreeTool#
  _CallTreeBase.expand: _CallTreeBase#expand().
  _CallTreeBase.get_tool_schema: _CallTreeBase#get_tool_schema().
  _CallTreeBase.get_tool_definition: _CallTreeBase#get_tool_definition().
  _CallTreeBase.__init__: _CallTreeBase#__init__().
  _CallTreeBase._direction: _CallTreeBase#_direction.
  _CallTreeBase.validate_arguments: _CallTreeBase#validate_arguments().
  logger: logger.
  _CallTreeBase._on_project_root_changed: _CallTreeBase#_on_project_root_changed().
  CodeGraphCalleeTreeTool._deterrent: CodeGraphCalleeTreeTool#_deterrent.
  _dedup_nodes: _dedup_nodes().
  _CALLEE_DETERRENT: _CALLEE_DETERRENT.
  _CALLER_DETERRENT: _CALLER_DETERRENT.
  _TRUNCATION_HINT: _TRUNCATION_HINT.
  _normalize_callee: _normalize_callee().
  _normalize_caller: _normalize_caller().
  _CallTreeBase._tool_name: _CallTreeBase#_tool_name.
  _CallTreeBase._deterrent: _CallTreeBase#_deterrent.
  CodeGraphCalleeTreeTool._tool_name: CodeGraphCalleeTreeTool#_tool_name.
  CodeGraphCalleeTreeTool._direction: CodeGraphCalleeTreeTool#_direction.
  CodeGraphCallerTreeTool._tool_name: CodeGraphCallerTreeTool#_tool_name.
  CodeGraphCallerTreeTool._direction: CodeGraphCallerTreeTool#_direction.
  CodeGraphCallerTreeTool._deterrent: CodeGraphCallerTreeTool#_deterrent.
---
# Module: [`tree_sitter_analyzer/mcp/tools/_call_tree_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_call_tree_tool.py)

## Classes
### `CodeGraphCalleeTreeTool`  ·  implements/extends _CallTreeBase
- def: [`tree_sitter_analyzer/mcp/tools/_call_tree_tool.py:243`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_call_tree_tool.py#L243)
- doc: One-call depth-limited NESTED callee tree (mycelium RFC-0020 parity).
- signature: `class CodeGraphCalleeTreeTool(_CallTreeBase):`
- protocol/private: `_deterrent`[`L248`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_call_tree_tool.py#L248), `_direction`[`L247`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_call_tree_tool.py#L247), `_tool_name`[`L246`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_call_tree_tool.py#L246)
- uses (calls/refs, reference-scoped): [`_CallTreeBase`](_call_tree_tool.md#_CallTreeBase), [`_CALLEE_DETERRENT`](_call_tree_tool.md#_CALLEE_DETERRENT)
- used by: [`build_nav_facade`](nav_facade.md#build_nav_facade), [`_CallTreeBase`](_call_tree_tool.md#_CallTreeBase)  (5 test-only)

### `CodeGraphCallerTreeTool`  ·  implements/extends _CallTreeBase
- def: [`tree_sitter_analyzer/mcp/tools/_call_tree_tool.py:251`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_call_tree_tool.py#L251)
- doc: One-call depth-limited NESTED caller tree (mycelium RFC-0021 parity).
- signature: `class CodeGraphCallerTreeTool(_CallTreeBase):`
- protocol/private: `_deterrent`[`L256`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_call_tree_tool.py#L256), `_direction`[`L255`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_call_tree_tool.py#L255), `_tool_name`[`L254`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_call_tree_tool.py#L254)
- uses (calls/refs, reference-scoped): [`_CallTreeBase`](_call_tree_tool.md#_CallTreeBase), [`_CALLER_DETERRENT`](_call_tree_tool.md#_CALLER_DETERRENT)
- used by: [`build_nav_facade`](nav_facade.md#build_nav_facade), [`_CallTreeBase`](_call_tree_tool.md#_CallTreeBase)  (2 test-only)

### `_CallTreeBase`  ·  implements/extends BaseMCPTool, CodeGraphRelationToolMixin
- def: [`tree_sitter_analyzer/mcp/tools/_call_tree_tool.py:73`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_call_tree_tool.py#L73)
- doc: Shared execution for callee/caller tree tools.
- signature: `class _CallTreeBase(CodeGraphRelationToolMixin, BaseMCPTool):`
- members:
  - `_make_expander(self)` — [`L156`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_call_tree_tool.py#L156) — Return a storage-agnostic single-hop expand(name, file) callback.
  - `execute(self, arguments: dict[str, Any])` — [`L186`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_call_tree_tool.py#L186)
  - `expand(name: str, file: str | None)` — [`L166`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_call_tree_tool.py#L166)
  - `get_tool_definition(self)` — [`L88`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_call_tree_tool.py#L88)
  - `get_tool_schema(self)` — [`L109`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_call_tree_tool.py#L109)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L149`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_call_tree_tool.py#L149)
- protocol/private: `__init__`[`L81`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_call_tree_tool.py#L81), `_deterrent`[`L79`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_call_tree_tool.py#L79), `_direction`[`L78`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_call_tree_tool.py#L78), `_on_project_root_changed`[`L85`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_call_tree_tool.py#L85), `_tool_name`[`L77`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_call_tree_tool.py#L77)
- uses (calls/refs, reference-scoped): [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`apply_toon_format_to_response`](../utils/format_helper.md#apply_toon_format_to_response), [`build_response`](_response_builder.md#build_response), [`__init__`](base_tool.md#BaseMCPTool.__init__), [`callees_of`](../../call_graph.md#CallGraph.callees_of), [`callers_of`](../../call_graph.md#CallGraph.callers_of), [`build_call_tree`](_call_tree.md#build_call_tree), [`_get_call_graph`](codegraph_relation_tool.md#CodeGraphRelationToolMixin._get_call_graph), [`CodeGraphRelationToolMixin`](codegraph_relation_tool.md#CodeGraphRelationToolMixin), [`_try_get_cache`](codegraph_relation_tool.md#CodeGraphRelationToolMixin._try_get_cache), [`CodeGraphCalleeTreeTool`](_call_tree_tool.md#CodeGraphCalleeTreeTool), [`project_root`](codegraph_relation_tool.md#CodeGraphRelationToolMixin.project_root), [`CodeGraphCallerTreeTool`](_call_tree_tool.md#CodeGraphCallerTreeTool), [`DEFAULT_MAX_NODES`](_call_tree.md#DEFAULT_MAX_NODES), [`_init_relation_state`](codegraph_relation_tool.md#CodeGraphRelationToolMixin._init_relation_state), [`_reset_relation_state`](codegraph_relation_tool.md#CodeGraphRelationToolMixin._reset_relation_state), [`_data_source`](codegraph_relation_tool.md#CodeGraphRelationToolMixin._data_source), [`DEFAULT_MAX_DEPTH`](_call_tree.md#DEFAULT_MAX_DEPTH), [`Expander`](_call_tree.md#Expander), [`MAX_DEPTH_CAP`](_call_tree.md#MAX_DEPTH_CAP), [`_dedup_nodes`](_call_tree_tool.md#_dedup_nodes), [`_TRUNCATION_HINT`](_call_tree_tool.md#_TRUNCATION_HINT), [`_normalize_callee`](_call_tree_tool.md#_normalize_callee), [`_normalize_caller`](_call_tree_tool.md#_normalize_caller)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`_on_project_root_changed`](base_tool.md#BaseMCPTool._on_project_root_changed), [`CodeGraphRelationToolMixin`](codegraph_relation_tool.md#CodeGraphRelationToolMixin), [`CodeGraphCalleeTreeTool`](_call_tree_tool.md#CodeGraphCalleeTreeTool), [`CodeGraphCallerTreeTool`](_call_tree_tool.md#CodeGraphCallerTreeTool)  (7 test-only)

## Functions
- `_dedup_nodes(nodes: Iterable[dict[str, Any]])` — [`L228`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_call_tree_tool.py#L228) — Drop empty-name rows and dedup by (file, name) preserving order.
- `_normalize_callee(edge: dict[str, Any])` — [`L52`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_call_tree_tool.py#L52) — SQL callee edge / graph callee dict → uniform {name,file,line}.
- `_normalize_caller(edge: dict[str, Any])` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_call_tree_tool.py#L65) — SQL caller edge / graph caller dict → uniform {name,file,line}.

## Module values
- `_CALLEE_DETERRENT` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_call_tree_tool.py#L35)
- `_CALLER_DETERRENT` — [`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_call_tree_tool.py#L40)
- `_TRUNCATION_HINT` — [`L46`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_call_tree_tool.py#L46)
- `logger` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_call_tree_tool.py#L33)

