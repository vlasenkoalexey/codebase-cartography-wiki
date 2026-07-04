---
title: TOON output format — token-efficient MCP responses
type: doc-concept
provenance: doc
source: README.md
updated: 2026-07-04
status: fresh
---
# TOON output format — token-efficient MCP responses

## Definition
TOON ("Token-Oriented Object Notation" per the README's framing) is TSA's default MCP response
encoding — "a tabular JSON variant that cuts bulk/tabular payloads by roughly half vs raw JSON." The
README is careful to scope the claim rather than state a blanket number: bulk/tabular responses save
roughly half, but "small metadata-heavy decision-tool responses are currently ~equal-to-larger than
JSON under the present envelope wiring" — a gap tracked by an explicit RFC (RFC-0018) rather than
hidden.

## In tree-sitter-analyzer (grounded)
This silo's own concept page,
[`tree_sitter_analyzer-formatters-toon_encoder`](../concepts/tree_sitter_analyzer-formatters-toon_encoder.md),
documents the encoder mechanics: an iterative, explicit-stack tree walk (never recursive, so a
pathologically deep structure can't blow the Python call stack) implemented in
[`ToonEncoder`](../catalog/tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder), with a
JSON-fallback on any encoding error. The layer that actually decides *whether* to emit TOON for a given
MCP response sits one level up, in
[`ToonFormatter`](../catalog/tree_sitter_analyzer/formatters/toon_formatter.md#ToonFormatter) —
[`format_mcp_response`](../catalog/tree_sitter_analyzer/formatters/toon_formatter.md#ToonFormatter.format_mcp_response)
and
[`format_analysis_result`](../catalog/tree_sitter_analyzer/formatters/toon_formatter.md#ToonFormatter.format_analysis_result)
are the adapters between a tool's real result object and the encoder's generic dict/list input. The
README's own measured-invariant claim points at a real test module,
`tests/unit/mcp/test_output_cost_invariants.py` — precisely the kind of differential/ratchet invariant
(`toon ≤ json`, never a hand-waved ceiling) this repo's own `CLAUDE.md` documents as a hard-learned rule
after a real incident (a ~1.96× TOON-larger-than-JSON regression that ~18,000 conformance tests failed
to catch, per that file's "non-functional claim is a belief until it is an executable invariant"
section) — i.e. the README's careful hedging on the decision-tool case is not marketing caution, it's
the direct product of that incident.

## Why it matters / when it applies
The repo's own `CLAUDE.md` records this as a LOCKED design decision: MCP defaults to TOON, CLI defaults
to JSON, specifically because "MCP callers are LLM agents — token cost is real money" while "CLI callers
are humans / shells — JSON is human-readable and pipes into `jq`." The README's "Correction (2026-06)"
callout is worth preserving here too: an earlier version of the README claimed TSA beat CodeGraph on
*agent token cost* generally (a "−11% median" table) — that number came from a harness bug (the TSA arm
analyzed its own source instead of the target repo) and was withdrawn once caught, leaving CodeGraph
still ahead on raw token cost for context-heavy calls (progressive disclosure, RFC-0006, closes "most
of the gap" per the README, from ~2.9× to ~1.5× CodeGraph's payload on the dominant context call — not
to parity).

## Connections
- Code concepts: [`tree_sitter_analyzer-formatters-toon_encoder`](../concepts/tree_sitter_analyzer-formatters-toon_encoder.md).
- Module catalogs: [`formatters/toon_encoder.py`](../catalog/tree_sitter_analyzer/formatters/toon_encoder.md),
  [`formatters/toon_formatter.py`](../catalog/tree_sitter_analyzer/formatters/toon_formatter.md).
- Related doc-concepts: [`mcp-facade-and-verdict-envelopes`](mcp-facade-and-verdict-envelopes.md) (TOON
  is one property of the same MCP response envelope that carries `verdict`).

## Source
Extracted from `README.md` (kept in place) — sections "Why Tree-sitter Analyzer" and "On token cost —
and a benchmark we corrected".
