---
title: 'Module: tree_sitter_analyzer/mcp/tools/_response_builder.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/_response_builder.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools._response_builder`/
symbols:
  build_response: build_response().
  build_error: build_error().
  CANONICAL_VERDICTS.CANONICAL_VERDICTS: CANONICAL_VERDICTS.CANONICAL_VERDICTS.
  InvalidVerdictError: InvalidVerdictError#
  __all__: __all__.
---
# Module: [`tree_sitter_analyzer/mcp/tools/_response_builder.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_response_builder.py)

## Classes
### `InvalidVerdictError`  ·  implements/extends ValueError
- def: [`tree_sitter_analyzer/mcp/tools/_response_builder.py:70`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_response_builder.py#L70)
- doc: Raised when a tool tries to emit a verdict outside the canonical set.
- signature: `class InvalidVerdictError(ValueError):`
- used by: [`build_response`](_response_builder.md#build_response)  (3 test-only)

## Functions
- `build_error(*, error: str, verdict: str = "ERROR", **fields: Any)` — [`L124`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_response_builder.py#L124) — Construct an error envelope with default ``verdict="ERROR"``.
- `build_response(*, verdict: str, success: bool = True, warnings: list[str] | None = None, **fields: Any)` — [`L79`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_response_builder.py#L79) — Construct a tool response envelope with verdict validation.

## Module values
- `CANONICAL_VERDICTS` — [`L56`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_response_builder.py#L56)
- `__all__` — [`L146`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_response_builder.py#L146)

