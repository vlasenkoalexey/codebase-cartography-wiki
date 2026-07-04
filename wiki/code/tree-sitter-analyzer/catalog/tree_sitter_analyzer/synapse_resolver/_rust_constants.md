---
title: 'Module: tree_sitter_analyzer/synapse_resolver/_rust_constants.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/synapse_resolver/_rust_constants.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.synapse_resolver._rust_constants`/
symbols:
  is_std_assoc_call: is_std_assoc_call().
  is_std_path: is_std_path().
  STD_PATH_PREFIXES.STD_PATH_PREFIXES: STD_PATH_PREFIXES.STD_PATH_PREFIXES.
  _STD_ASSOC_TYPES._STD_ASSOC_TYPES: _STD_ASSOC_TYPES._STD_ASSOC_TYPES.
  _STD_ASSOC_FNS._STD_ASSOC_FNS: _STD_ASSOC_FNS._STD_ASSOC_FNS.
  __all__: __all__.
---
# Module: [`tree_sitter_analyzer/synapse_resolver/_rust_constants.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_rust_constants.py)

## Functions
- `is_std_assoc_call(receiver: str, simple: str)` — [`L79`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_rust_constants.py#L79) — True for a ``StdContainer::ctor`` associated call (``Vec::new``).
- `is_std_path(callee_full: str)` — [`L74`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_rust_constants.py#L74) — True when ``callee_full`` begins with a std distribution path prefix.

## Module values
- `STD_PATH_PREFIXES` — [`L32`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_rust_constants.py#L32)
- `_STD_ASSOC_FNS` — [`L64`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_rust_constants.py#L64)
- `_STD_ASSOC_TYPES` — [`L44`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_rust_constants.py#L44)
- `__all__` — [`L90`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_rust_constants.py#L90)

