---
title: 'Module: graphify/semantic_cleanup.py'
type: catalog
provenance: extracted
module: graphify/semantic_cleanup.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `graphify.semantic_cleanup`/
symbols:
  validate_semantic_fragment: validate_semantic_fragment().
  sanitize_semantic_fragment: sanitize_semantic_fragment().
  _validate_semantic_id: _validate_semantic_id().
  load_validated_semantic_fragment: load_validated_semantic_fragment().
  _is_sentence_like_rationale_label: _is_sentence_like_rationale_label().
  MAX_SEMANTIC_FRAGMENT_BYTES: MAX_SEMANTIC_FRAGMENT_BYTES.
  MAX_SEMANTIC_FRAGMENT_NODES: MAX_SEMANTIC_FRAGMENT_NODES.
  MAX_SEMANTIC_FRAGMENT_EDGES: MAX_SEMANTIC_FRAGMENT_EDGES.
  MAX_SEMANTIC_FRAGMENT_HYPEREDGES: MAX_SEMANTIC_FRAGMENT_HYPEREDGES.
  MAX_SEMANTIC_HYPEREDGE_NODES: MAX_SEMANTIC_HYPEREDGE_NODES.
  MAX_SEMANTIC_ID_LENGTH: MAX_SEMANTIC_ID_LENGTH.
  VALID_SEMANTIC_FILE_TYPES: VALID_SEMANTIC_FILE_TYPES.
  _RATIONALE_MIN_CHARS: _RATIONALE_MIN_CHARS.
  _RATIONALE_MIN_WORDS: _RATIONALE_MIN_WORDS.
  _SEMANTIC_ID_RE: _SEMANTIC_ID_RE.
  _append_rationale_attr: _append_rationale_attr().
---
# Module: [`graphify/semantic_cleanup.py`](../../../../../raw/code/graphify/graphify/semantic_cleanup.py)

## Functions
- `_append_rationale_attr(node: dict, texts: list[str])` — [`L317`](../../../../../raw/code/graphify/graphify/semantic_cleanup.py#L317) — Append one or more rationale strings to *node*'s ``rationale`` attribute.
- `_is_sentence_like_rationale_label(label: str)` — [`L296`](../../../../../raw/code/graphify/graphify/semantic_cleanup.py#L296) — Return True if *label* looks like prose / rationale text rather than an
- `_validate_semantic_id(errors: list[str], field: str, value: object)` — [`L150`](../../../../../raw/code/graphify/graphify/semantic_cleanup.py#L150)
- `load_validated_semantic_fragment(path: Path)` — [`L126`](../../../../../raw/code/graphify/graphify/semantic_cleanup.py#L126) — Load and validate a semantic chunk, rejecting oversize files before parsing.
- `sanitize_semantic_fragment(fragment: dict)` — [`L165`](../../../../../raw/code/graphify/graphify/semantic_cleanup.py#L165) — Clean up a semantic extraction fragment in-place.
- `validate_semantic_fragment(fragment: object)` — [`L37`](../../../../../raw/code/graphify/graphify/semantic_cleanup.py#L37) — Return validation errors for an untrusted semantic extraction fragment.

## Module values
- `MAX_SEMANTIC_FRAGMENT_BYTES` — [`L27`](../../../../../raw/code/graphify/graphify/semantic_cleanup.py#L27)
- `MAX_SEMANTIC_FRAGMENT_EDGES` — [`L29`](../../../../../raw/code/graphify/graphify/semantic_cleanup.py#L29)
- `MAX_SEMANTIC_FRAGMENT_HYPEREDGES` — [`L30`](../../../../../raw/code/graphify/graphify/semantic_cleanup.py#L30)
- `MAX_SEMANTIC_FRAGMENT_NODES` — [`L28`](../../../../../raw/code/graphify/graphify/semantic_cleanup.py#L28)
- `MAX_SEMANTIC_HYPEREDGE_NODES` — [`L31`](../../../../../raw/code/graphify/graphify/semantic_cleanup.py#L31)
- `MAX_SEMANTIC_ID_LENGTH` — [`L32`](../../../../../raw/code/graphify/graphify/semantic_cleanup.py#L32)
- `VALID_SEMANTIC_FILE_TYPES` — [`L33`](../../../../../raw/code/graphify/graphify/semantic_cleanup.py#L33)
- `_RATIONALE_MIN_CHARS` — [`L19`](../../../../../raw/code/graphify/graphify/semantic_cleanup.py#L19)
- `_RATIONALE_MIN_WORDS` — [`L20`](../../../../../raw/code/graphify/graphify/semantic_cleanup.py#L20)
- `_SEMANTIC_ID_RE` — [`L34`](../../../../../raw/code/graphify/graphify/semantic_cleanup.py#L34)

