---
title: 'Module: graphify/ruby_resolution.py'
type: catalog
provenance: extracted
module: graphify/ruby_resolution.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `graphify.ruby_resolution`/
symbols:
  resolve_ruby_member_calls: resolve_ruby_member_calls().
  _key: _key().
  resolve_ruby_member_calls._unique_class: resolve_ruby_member_calls()._unique_class().
  resolve_ruby_member_calls._emit: resolve_ruby_member_calls()._emit().
  _BARE_CONST_RE: _BARE_CONST_RE.
  _ruby_raw_calls: _ruby_raw_calls().
---
# Module: [`graphify/ruby_resolution.py`](../../../../../raw/code/graphify/graphify/ruby_resolution.py)

## Functions
- `_emit(caller: str, target: str, rc: dict[str, Any])` — [`L97`](../../../../../raw/code/graphify/graphify/ruby_resolution.py#L97)
- `_key(label: str)` — [`L26`](../../../../../raw/code/graphify/graphify/ruby_resolution.py#L26) — Normalize a class/method label to a comparison key (drop punctuation).
- `_ruby_raw_calls(per_file: list[dict])` — [`L38`](../../../../../raw/code/graphify/graphify/ruby_resolution.py#L38)
- `_unique_class(name: str)` — [`L93`](../../../../../raw/code/graphify/graphify/ruby_resolution.py#L93)
- `resolve_ruby_member_calls(per_file: list[dict], all_nodes: list[dict], all_edges: list[dict])` — [`L52`](../../../../../raw/code/graphify/graphify/ruby_resolution.py#L52) — Resolve Ruby ``Class.new`` and typed ``var.method`` calls by receiver type.

## Module values
- `_BARE_CONST_RE` — [`L35`](../../../../../raw/code/graphify/graphify/ruby_resolution.py#L35)

