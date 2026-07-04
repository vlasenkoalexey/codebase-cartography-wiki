---
title: 'Module: graphify/dedup.py'
type: catalog
provenance: extracted
module: graphify/dedup.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `graphify.dedup`/
symbols:
  deduplicate_entities: deduplicate_entities().
  _llm_tiebreak: _llm_tiebreak().
  _norm: _norm().
  _is_variant_pair: _is_variant_pair().
  _numeric_tokens_differ: _numeric_tokens_differ().
  _UF._parent: _UF#_parent.
  _UF.union: _UF#union().
  _UF.find: _UF#find().
  _make_minhash: _make_minhash().
  _entropy: _entropy().
  _pick_winner: _pick_winner().
  _UF.components: _UF#components().
  _crossfile_fileanchored_blocked: _crossfile_fileanchored_blocked().
  _shingles: _shingles().
  _short_label_blocked: _short_label_blocked().
  _pick_winner._score: _pick_winner()._score().
  _VARIANT_SUFFIX: _VARIANT_SUFFIX.
  _DIGIT_RUN: _DIGIT_RUN.
  _FILE_ANCHORED_NONCODE: _FILE_ANCHORED_NONCODE.
  _UF: _UF#
  _COMMUNITY_BOOST: _COMMUNITY_BOOST.
  _is_code: _is_code().
  _ENTROPY_THRESHOLD: _ENTROPY_THRESHOLD.
  _LSH_THRESHOLD: _LSH_THRESHOLD.
  _MERGE_THRESHOLD: _MERGE_THRESHOLD.
  _NUM_PERM: _NUM_PERM.
  _CHUNK_SUFFIX: _CHUNK_SUFFIX.
  _UF.__init__: _UF#__init__().
---
# Module: [`graphify/dedup.py`](../../../../../raw/code/graphify/graphify/dedup.py)

## Classes
### `_UF`
- def: [`graphify/dedup.py:141`](../../../../../raw/code/graphify/graphify/dedup.py#L141)
- signature: `class _UF:`
- members:
  - `components(self)` — [`L159`](../../../../../raw/code/graphify/graphify/dedup.py#L159) — documented in [graphify-dedup](../../concepts/graphify-dedup.md)
  - `find(self, x: str)` — [`L145`](../../../../../raw/code/graphify/graphify/dedup.py#L145) — documented in [graphify-dedup](../../concepts/graphify-dedup.md)
  - `union(self, x: str, y: str)` — [`L152`](../../../../../raw/code/graphify/graphify/dedup.py#L152) — documented in [graphify-dedup](../../concepts/graphify-dedup.md)
- protocol/private: `__init__`[`L142`](../../../../../raw/code/graphify/graphify/dedup.py#L142), `_parent`[`L143`](../../../../../raw/code/graphify/graphify/dedup.py#L143)
- used by: [`deduplicate_entities`](dedup.md#deduplicate_entities), [`_llm_tiebreak`](dedup.md#_llm_tiebreak)

## Functions
- `_crossfile_fileanchored_blocked(node: dict, neighbor: dict)` — [`L124`](../../../../../raw/code/graphify/graphify/dedup.py#L124) — Block label-based merging of file-anchored non-code nodes across files (#1284). — documented in [graphify-dedup](../../concepts/graphify-dedup.md)
- `_entropy(label: str)` — [`L27`](../../../../../raw/code/graphify/graphify/dedup.py#L27) — Shannon entropy in bits/char of the normalised label. — documented in [graphify-dedup](../../concepts/graphify-dedup.md)
- `_is_code(node: dict)` — [`L176`](../../../../../raw/code/graphify/graphify/dedup.py#L176) — True for AST-extracted code symbols.
- `_is_variant_pair(a: str, b: str)` — [`L61`](../../../../../raw/code/graphify/graphify/dedup.py#L61) — True if a and b are sibling model/SKU variants (same stem, different suffix). — documented in [graphify-dedup](../../concepts/graphify-dedup.md)
- `_llm_tiebreak(candidates: list[dict], uf: _UF, communities: dict[str, int], *, backend: str, batch_size: int = 30, low: float = 75, high: float = 92)` — [`L463`](../../../../../raw/code/graphify/graphify/dedup.py#L463) — Batch-resolve ambiguous pairs (score in [low, high)) via LLM. — documented in [graphify-dedup](../../concepts/graphify-dedup.md)
- `_make_minhash(text: str, num_perm: int = 128)` — [`L46`](../../../../../raw/code/graphify/graphify/dedup.py#L46) — documented in [graphify-_minhash](../../concepts/graphify-_minhash.md)
- `_norm(label: str | None)` — [`L19`](../../../../../raw/code/graphify/graphify/dedup.py#L19) — Lowercase + collapse non-alphanumeric runs to space (Unicode-aware). — documented in [graphify-dedup](../../concepts/graphify-dedup.md)
- `_numeric_tokens_differ(a: str, b: str)` — [`L96`](../../../../../raw/code/graphify/graphify/dedup.py#L96) — True when two labels carry different embedded numbers (#1284). — documented in [graphify-dedup](../../concepts/graphify-dedup.md)
- `_pick_winner(nodes: list[dict])` — [`L451`](../../../../../raw/code/graphify/graphify/dedup.py#L451) — Pick the canonical survivor: prefer no chunk suffix, then shorter ID. — documented in [graphify-dedup](../../concepts/graphify-dedup.md)
- `_score(n: dict)` — [`L456`](../../../../../raw/code/graphify/graphify/dedup.py#L456)
- `_shingles(text: str, k: int = 3)` — [`L39`](../../../../../raw/code/graphify/graphify/dedup.py#L39) — Return k-gram character shingles of text. — documented in [graphify-dedup](../../concepts/graphify-dedup.md)
- `_short_label_blocked(a: str, b: str, jw_score: float)` — [`L76`](../../../../../raw/code/graphify/graphify/dedup.py#L76) — Block fuzzy merge for short labels unless it's a same-length single-char substitution. — documented in [graphify-dedup](../../concepts/graphify-dedup.md)
- `deduplicate_entities(nodes: list[dict], edges: list[dict], *, communities: dict[str, int], dedup_llm_backend: str | None = None)` — [`L192`](../../../../../raw/code/graphify/graphify/dedup.py#L192) — Deduplicate near-identical entities in a knowledge graph. — documented in [graphify-__main__](../../concepts/graphify-__main__.md)

## Module values
- `_CHUNK_SUFFIX` — [`L173`](../../../../../raw/code/graphify/graphify/dedup.py#L173)
- `_COMMUNITY_BOOST` — [`L171`](../../../../../raw/code/graphify/graphify/dedup.py#L171)
- `_DIGIT_RUN` — [`L93`](../../../../../raw/code/graphify/graphify/dedup.py#L93)
- `_ENTROPY_THRESHOLD` — [`L168`](../../../../../raw/code/graphify/graphify/dedup.py#L168)
- `_FILE_ANCHORED_NONCODE` — [`L121`](../../../../../raw/code/graphify/graphify/dedup.py#L121)
- `_LSH_THRESHOLD` — [`L169`](../../../../../raw/code/graphify/graphify/dedup.py#L169)
- `_MERGE_THRESHOLD` — [`L170`](../../../../../raw/code/graphify/graphify/dedup.py#L170)
- `_NUM_PERM` — [`L172`](../../../../../raw/code/graphify/graphify/dedup.py#L172)
- `_VARIANT_SUFFIX` — [`L58`](../../../../../raw/code/graphify/graphify/dedup.py#L58)

