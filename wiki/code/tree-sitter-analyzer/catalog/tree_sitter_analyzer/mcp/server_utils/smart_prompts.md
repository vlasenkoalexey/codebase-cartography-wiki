---
title: 'Module: tree_sitter_analyzer/mcp/server_utils/smart_prompts.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/server_utils/smart_prompts.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.server_utils.smart_prompts`/
symbols:
  build_smart_analyze_response: build_smart_analyze_response().
  build_smart_explore_response: build_smart_explore_response().
  _ANALYZE_INSTRUCTIONS_TEMPLATE: _ANALYZE_INSTRUCTIONS_TEMPLATE.
  _EXPLORE_INSTRUCTIONS_TEMPLATE: _EXPLORE_INSTRUCTIONS_TEMPLATE.
  _smart_user_message: _smart_user_message().
---
# Module: [`tree_sitter_analyzer/mcp/server_utils/smart_prompts.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server_utils/smart_prompts.py)

## Functions
- `_smart_user_message(text: str)` — [`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server_utils/smart_prompts.py#L41) — Wrap ``text`` in the MCP ``messages[]`` user-text envelope.
- `build_smart_analyze_response(file_path: str, question: str)` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server_utils/smart_prompts.py#L49) — Build the SMART analyze prompt response for AI agents.
- `build_smart_explore_response(project_root: str)` — [`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server_utils/smart_prompts.py#L58) — Build the SMART explore prompt response for AI agents.

## Module values
- `_ANALYZE_INSTRUCTIONS_TEMPLATE` — [`L12`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server_utils/smart_prompts.py#L12)
- `_EXPLORE_INSTRUCTIONS_TEMPLATE` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server_utils/smart_prompts.py#L26)

