---
title: 'Module: graphify/_minhash.py'
type: catalog
provenance: extracted
module: graphify/_minhash.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `graphify._minhash`/
symbols:
  MinHash: MinHash#
  MinHashLSH.insert: MinHashLSH#insert().
  MinHashLSH.query: MinHashLSH#query().
  MinHash.update: MinHash#update().
  _optimal_lsh_params: _optimal_lsh_params().
  MinHash.__init__: MinHash#__init__().
  MinHashLSH: MinHashLSH#
  MinHashLSH.r: MinHashLSH#r.
  _mh_coeffs: _mh_coeffs().
  MinHashLSH._tables: MinHashLSH#_tables.
  _MP: _MP.
  _MH_COEFFS._MH_COEFFS: _MH_COEFFS._MH_COEFFS.
  _LSH_PARAMS_CACHE._LSH_PARAMS_CACHE: _LSH_PARAMS_CACHE._LSH_PARAMS_CACHE.
  _MH: _MH.
  _lsh_integrate: _lsh_integrate().
  MinHashLSH._keys: MinHashLSH#_keys.
  MinHashLSH.b: MinHashLSH#b.
  MinHash.__slots__: MinHash#__slots__.
  MinHashLSH.__init__: MinHashLSH#__init__().
---
# Module: [`graphify/_minhash.py`](../../../../../raw/code/graphify/graphify/_minhash.py)

## Classes
### `MinHash`
- def: [`graphify/_minhash.py:36`](../../../../../raw/code/graphify/graphify/_minhash.py#L36) — documented in [graphify-_minhash](../../concepts/graphify-_minhash.md)
- doc: MinHash sketch — same API as datasketch.MinHash for the subset used here.
- signature: `class MinHash:`
- members:
  - `update(self, v: bytes)` — [`L46`](../../../../../raw/code/graphify/graphify/_minhash.py#L46) — documented in [graphify-_minhash](../../concepts/graphify-_minhash.md)
- protocol/private: `__init__`[`L41`](../../../../../raw/code/graphify/graphify/_minhash.py#L41), `__slots__`[`L39`](../../../../../raw/code/graphify/graphify/_minhash.py#L39)
- uses (calls/refs, reference-scoped): [`_mh_coeffs`](_minhash.md#_mh_coeffs), [`_MP`](_minhash.md#_MP), [`_MH`](_minhash.md#_MH)
- used by: [`deduplicate_entities`](dedup.md#deduplicate_entities), [`insert`](_minhash.md#MinHashLSH.insert), [`query`](_minhash.md#MinHashLSH.query), [`_make_minhash`](dedup.md#_make_minhash)  (5 test-only)

### `MinHashLSH`
- def: [`graphify/_minhash.py:84`](../../../../../raw/code/graphify/graphify/_minhash.py#L84)
- doc: Band-hashing LSH — same API as datasketch.MinHashLSH for the subset used here.
- signature: `class MinHashLSH:`
- members:
  - `insert(self, key: str, minhash: MinHash)` — [`L92`](../../../../../raw/code/graphify/graphify/_minhash.py#L92) — documented in [graphify-_minhash](../../concepts/graphify-_minhash.md)
  - `query(self, minhash: MinHash)` — [`L101`](../../../../../raw/code/graphify/graphify/_minhash.py#L101) — documented in [graphify-_minhash](../../concepts/graphify-_minhash.md)
  - `b` — [`L88`](../../../../../raw/code/graphify/graphify/_minhash.py#L88) — documented in [graphify-_minhash](../../concepts/graphify-_minhash.md)
  - `r` — [`L88`](../../../../../raw/code/graphify/graphify/_minhash.py#L88) — documented in [graphify-_minhash](../../concepts/graphify-_minhash.md)
- protocol/private: `__init__`[`L87`](../../../../../raw/code/graphify/graphify/_minhash.py#L87), `_keys`[`L90`](../../../../../raw/code/graphify/graphify/_minhash.py#L90), `_tables`[`L89`](../../../../../raw/code/graphify/graphify/_minhash.py#L89)
- uses (calls/refs, reference-scoped): [`MinHash`](_minhash.md#MinHash), [`_optimal_lsh_params`](_minhash.md#_optimal_lsh_params)
- used by: [`deduplicate_entities`](dedup.md#deduplicate_entities)  (4 test-only)

## Functions
- `_lsh_integrate(f, lo: float, hi: float, n: int = 128)` — [`L52`](../../../../../raw/code/graphify/graphify/_minhash.py#L52) — Numerical integration — replaces scipy.integrate.quad for LSH param search. — documented in [graphify-_minhash](../../concepts/graphify-_minhash.md)
- `_mh_coeffs(num_perm: int)` — [`L27`](../../../../../raw/code/graphify/graphify/_minhash.py#L27)
- `_optimal_lsh_params(threshold: float, num_perm: int)` — [`L61`](../../../../../raw/code/graphify/graphify/_minhash.py#L61) — Find (bands, rows) that minimise weighted FP+FN error, without scipy. — documented in [graphify-_minhash](../../concepts/graphify-_minhash.md)

## Module values
- `_LSH_PARAMS_CACHE` — [`L58`](../../../../../raw/code/graphify/graphify/_minhash.py#L58) — documented in [graphify-_minhash](../../concepts/graphify-_minhash.md)
- `_MH` — [`L21`](../../../../../raw/code/graphify/graphify/_minhash.py#L21) — documented in [graphify-_minhash](../../concepts/graphify-_minhash.md)
- `_MH_COEFFS` — [`L24`](../../../../../raw/code/graphify/graphify/_minhash.py#L24)
- `_MP` — [`L20`](../../../../../raw/code/graphify/graphify/_minhash.py#L20) — documented in [graphify-_minhash](../../concepts/graphify-_minhash.md)

