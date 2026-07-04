---
title: 'Module: tree_sitter_analyzer/mcp/intent_aliases.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/intent_aliases.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.intent_aliases`/
symbols:
  IntentAliasResolver.resolve: IntentAliasResolver#resolve().
  IntentAliasResolver: IntentAliasResolver#
  is_valid_alias: is_valid_alias().
  get_tool_name_from_alias: get_tool_name_from_alias().
  IntentAliasResolver._aliases: IntentAliasResolver#_aliases.
  get_all_aliases: get_all_aliases().
  INTENT_ALIASES.INTENT_ALIASES: INTENT_ALIASES.INTENT_ALIASES.
  IntentAliasResolver.__init__: IntentAliasResolver#__init__().
---
# Module: [`tree_sitter_analyzer/mcp/intent_aliases.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/intent_aliases.py)

## Classes
### `IntentAliasResolver`
- def: [`tree_sitter_analyzer/mcp/intent_aliases.py:37`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/intent_aliases.py#L37)
- doc: Intent Alias を tool名に解決するリゾルバー
- signature: `class IntentAliasResolver:`
- members:
  - `__init__(self, aliases: dict[str, str] | None = None)` — [`L46`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/intent_aliases.py#L46) — Initialize IntentAliasResolver
  - `resolve(self, name: str)` — [`L56`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/intent_aliases.py#L56) — Tool名または alias を正規の tool名に解決
- protocol/private: `_aliases`[`L54`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/intent_aliases.py#L54)
- uses (calls/refs, reference-scoped): [`INTENT_ALIASES`](intent_aliases.md#INTENT_ALIASES.INTENT_ALIASES)
- used by: [`call_tool`](server.md#TreeSitterAnalyzerMCPServer.call_tool), [`is_valid_alias`](intent_aliases.md#is_valid_alias), [`get_tool_name_from_alias`](intent_aliases.md#get_tool_name_from_alias)  (14 test-only)

## Functions
- `get_all_aliases()` — [`L112`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/intent_aliases.py#L112) — 全ての intent alias マッピングを取得
- `get_tool_name_from_alias(name: str)` — [`L95`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/intent_aliases.py#L95) — Helper function: alias を tool名に変換
- `is_valid_alias(name: str)` — [`L122`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/intent_aliases.py#L122) — 名前が有効な alias または tool名かチェック

## Module values
- `INTENT_ALIASES` — [`L21`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/intent_aliases.py#L21)

