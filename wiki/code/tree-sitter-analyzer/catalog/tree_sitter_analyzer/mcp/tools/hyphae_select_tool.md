---
title: 'Module: tree_sitter_analyzer/mcp/tools/hyphae_select_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/hyphae_select_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.hyphae_select_tool`/
symbols:
  HyphaeSelectTool.execute: HyphaeSelectTool#execute().
  HyphaeSelectTool: HyphaeSelectTool#
  HyphaeSelectTool._cache: HyphaeSelectTool#_cache.
  HyphaeSelectTool._get_cache: HyphaeSelectTool#_get_cache().
  _cap_selector_echo: _cap_selector_echo().
  HyphaeSelectTool.get_tool_definition: HyphaeSelectTool#get_tool_definition().
  HyphaeSelectTool.__init__: HyphaeSelectTool#__init__().
  HyphaeSelectTool._on_project_root_changed: HyphaeSelectTool#_on_project_root_changed().
  _SELECTOR_ECHO_CAP: _SELECTOR_ECHO_CAP.
  HyphaeSelectTool.validate_arguments: HyphaeSelectTool#validate_arguments().
  HyphaeSelectTool.get_tool_schema: HyphaeSelectTool#get_tool_schema().
  HyphaeSelectTool._detect_index_state: HyphaeSelectTool#_detect_index_state().
---
# Module: [`tree_sitter_analyzer/mcp/tools/hyphae_select_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/hyphae_select_tool.py)

## Classes
### `HyphaeSelectTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/hyphae_select_tool.py:27`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/hyphae_select_tool.py#L27)
- doc: Execute a Hyphae selector and return matching symbols.
- signature: `class HyphaeSelectTool(BaseMCPTool):`
- members:
  - `_detect_index_state(self, cache: Any)` — [`L209`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/hyphae_select_tool.py#L209) — Determine (index_state, indexed_files).
  - `execute(self, arguments: dict[str, Any])` — [`L103`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/hyphae_select_tool.py#L103)
  - `get_tool_definition(self)` — [`L46`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/hyphae_select_tool.py#L46)
  - `get_tool_schema(self)` — [`L71`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/hyphae_select_tool.py#L71)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L98`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/hyphae_select_tool.py#L98)
- protocol/private: `__init__`[`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/hyphae_select_tool.py#L30), `_cache`[`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/hyphae_select_tool.py#L31), `_get_cache`[`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/hyphae_select_tool.py#L37), `_on_project_root_changed`[`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/hyphae_select_tool.py#L34)
- uses (calls/refs, reference-scoped): [`ASTCache`](../../ast_cache.md#ASTCache), [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`project_root`](base_tool.md#BaseMCPTool.project_root), [`apply_toon_format_to_response`](../utils/format_helper.md#apply_toon_format_to_response), [`parse`](../../hyphae/parser.md#parse), [`__init__`](base_tool.md#BaseMCPTool.__init__), [`eval`](../../hyphae/evaluator.md#Evaluator.eval), [`HyphaeSyntaxError`](../../hyphae/parser.md#HyphaeSyntaxError), [`Evaluator`](../../hyphae/evaluator.md#Evaluator), [`total_matches`](../../hyphae/evaluator.md#Evaluator.total_matches), [`was_truncated`](../../hyphae/evaluator.md#Evaluator.was_truncated), [`_cap_selector_echo`](hyphae_select_tool.md#_cap_selector_echo)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`_on_project_root_changed`](base_tool.md#BaseMCPTool._on_project_root_changed), [`build_search_facade`](search_facade.md#build_search_facade)  (19 test-only)

## Functions
- `_cap_selector_echo(selector: str)` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/hyphae_select_tool.py#L21)

## Module values
- `_SELECTOR_ECHO_CAP` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/hyphae_select_tool.py#L18)

