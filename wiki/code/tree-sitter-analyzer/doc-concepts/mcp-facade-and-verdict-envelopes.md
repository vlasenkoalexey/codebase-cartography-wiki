---
title: MCP facade surface + verdict envelopes — agent-native design
type: doc-concept
provenance: doc
source: README.md
updated: 2026-07-04
status: fresh
---
# MCP facade surface + verdict envelopes — agent-native design

## Definition
The README frames "8 MCP tools" (down from 55+ fine-grained inner tools) and "verdict envelopes" as
the two pillars of being "Built agent-native." Every response carries a `verdict` field drawn from a
fixed vocabulary (`SAFE | CAUTION | UNSAFE | INFO | REVIEW | WARN | ERROR | NOT_FOUND`), described as
letting "orchestrators branch on outcomes without re-prompting." The doc also names 13 curated "Skills"
(`.claude/skills/tsa-*/`) as pre-baked tool subsets so "the agent doesn't have to triage 8 tools on
every question," contrasted directly against the comparator: "CodeGraph has zero skills."

## In tree-sitter-analyzer (grounded)
The 8-tool consolidation is the exact mechanism this silo's
[`tree_sitter_analyzer-mcp-tools-facade_tool`](../concepts/tree_sitter_analyzer-mcp-tools-facade_tool.md)
page documents: [`FacadeTool`](../catalog/tree_sitter_analyzer/mcp/tools/facade_tool.md#FacadeTool) is a
pure routing layer whose
[`action_map`](../catalog/tree_sitter_analyzer/mcp/tools/facade_tool.md#FacadeTool.action_map) dispatches
an `action` argument to one of many inner tools without re-implementing their logic; eight concrete
facades (`nav`, `structure`, `search`, `health`, `edit`, `project`, `viz`, `index`) are what an MCP
client actually sees, matching the README's "8 MCP tools" figure exactly. The server that registers this
facade surface,
[`TreeSitterAnalyzerMCPServer`](../catalog/tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer),
is documented in [`tree_sitter_analyzer-mcp-server`](../concepts/tree_sitter_analyzer-mcp-server.md),
including the deferred-construction fix for a startup-latency bug. Every concrete tool beneath the
facade layer shares the `verdict`-carrying response convention this silo's
[`tree_sitter_analyzer-mcp-tools-base_tool`](../concepts/tree_sitter_analyzer-mcp-tools-base_tool.md)
page documents as *convention, not an abstract-method requirement* — the base contract
(`execute`/`get_tool_definition`/`get_tool_schema`/`validate_arguments`) says nothing about a verdict
field, yet every concrete tool's `execute` converges on piping its result through
[`apply_toon_format_to_response`](../catalog/tree_sitter_analyzer/mcp/utils/format_helper.md#apply_toon_format_to_response),
which that page documents as injecting a default `verdict="INFO"` onto any success response that forgot
to set one — the concrete safety net behind the README's "every response carries verdict" claim. Errors
that surface at this boundary are classified into a category/severity pair (not a verdict directly) by
[`ErrorHandler`](../catalog/tree_sitter_analyzer/mcp/utils/error_handler.md#ErrorHandler), documented in
[`tree_sitter_analyzer-mcp-utils-error_handler`](../concepts/tree_sitter_analyzer-mcp-utils-error_handler.md).

## Why it matters / when it applies
The README's framing is that a verdict vocabulary lets an agent *branch* on a response without a
follow-up LLM call to interpret free text — the same design instinct as a typed exception hierarchy, but
at the agent-protocol boundary rather than inside one process. The facade consolidation exists for a
narrower, more concrete reason the README states directly: exposing 55+ fine-grained tools to an LLM's
tool-selection context is itself a cost (more schema tokens, worse selection accuracy) — routing through
8 stable facade names amortizes that cost regardless of how many inner tools exist behind them, which is
exactly why [`tree_sitter_analyzer-mcp-tools-base_tool`](../concepts/tree_sitter_analyzer-mcp-tools-base_tool.md)
observes the safety-net convention (a default verdict) matters more, not less, once *many* independently
written inner tools share one facade surface — a single forgotten field would otherwise surface
inconsistently across dozens of tools instead of one.

## Connections
- Code concepts: [`tree_sitter_analyzer-mcp-tools-facade_tool`](../concepts/tree_sitter_analyzer-mcp-tools-facade_tool.md),
  [`tree_sitter_analyzer-mcp-tools-base_tool`](../concepts/tree_sitter_analyzer-mcp-tools-base_tool.md),
  [`tree_sitter_analyzer-mcp-server`](../concepts/tree_sitter_analyzer-mcp-server.md),
  [`tree_sitter_analyzer-mcp-utils-error_handler`](../concepts/tree_sitter_analyzer-mcp-utils-error_handler.md).
- Module catalogs: [`mcp/tools/facade_tool.py`](../catalog/tree_sitter_analyzer/mcp/tools/facade_tool.md),
  [`mcp/server.py`](../catalog/tree_sitter_analyzer/mcp/server.md),
  [`mcp/utils/format_helper.py`](../catalog/tree_sitter_analyzer/mcp/utils/format_helper.md).
- Related doc-concepts: [`toon-output-format`](toon-output-format.md) (the other property of the same
  response envelope).

## Source
Extracted from `README.md` (kept in place) — sections "Why it's different" and "Why Tree-sitter
Analyzer".
