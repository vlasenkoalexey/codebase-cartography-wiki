---
title: 'Module: tree_sitter_analyzer/miswire_audit.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/miswire_audit.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.miswire_audit`/
symbols:
  audit: audit().
  render_terminal: render_terminal().
  render_card: render_card().
  AuditResult.naive_miswires: AuditResult#naive_miswires.
  _caller_builtins: _caller_builtins().
  AuditResult.tsa_miswires: AuditResult#tsa_miswires.
  AuditResult.total_call_edges: AuditResult#total_call_edges.
  AuditResult.genuine_offenders: AuditResult#genuine_offenders.
  _CALLER_BUILTINS: _CALLER_BUILTINS.
  AuditResult.naive_offenders: AuditResult#naive_offenders.
  main: main().
  AuditResult.multiplier: AuditResult#multiplier().
  AuditResult: AuditResult#
  Offender.callee_name: Offender#callee_name.
  AuditResult.naive_genuine_miswires: AuditResult#naive_genuine_miswires.
  _iter_symbol_defs: _iter_symbol_defs().
  Offender: Offender#
  AuditResult.project_root: AuditResult#project_root.
  AuditResult.tsa_offenders: AuditResult#tsa_offenders.
  _fmt_pct: _fmt_pct().
  _build_name_maps: _build_name_maps().
  AuditResult.languages: AuditResult#languages.
  AuditResult.call_edges_available: AuditResult#call_edges_available.
  Offender.callee_lang: Offender#callee_lang.
  _DEF_KINDS: _DEF_KINDS.
  Offender.caller_file: Offender#caller_file.
  Offender.caller_lang: Offender#caller_lang.
  Offender.callee_file: Offender#callee_file.
  Offender.line: Offender#line.
  AuditResult.resolvable_edges: AuditResult#resolvable_edges.
---
# Module: [`tree_sitter_analyzer/miswire_audit.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/miswire_audit.py)

## Classes
### `AuditResult`
- def: [`tree_sitter_analyzer/miswire_audit.py:306`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/miswire_audit.py#L306)
- signature: `class AuditResult:`
- members:
  - `multiplier(self)` — [`L325`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/miswire_audit.py#L325) — How many times cleaner TSA is (naive / TSA), guarded for 0.
  - `call_edges_available` — [`L317`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/miswire_audit.py#L317)
  - `genuine_offenders` — [`L322`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/miswire_audit.py#L322)
  - `languages` — [`L314`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/miswire_audit.py#L314)
  - `naive_genuine_miswires` — [`L321`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/miswire_audit.py#L321)
  - `naive_miswires` — [`L310`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/miswire_audit.py#L310)
  - `naive_offenders` — [`L312`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/miswire_audit.py#L312)
  - `project_root` — [`L307`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/miswire_audit.py#L307)
  - `resolvable_edges` — [`L309`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/miswire_audit.py#L309)
  - `total_call_edges` — [`L308`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/miswire_audit.py#L308)
  - `tsa_miswires` — [`L311`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/miswire_audit.py#L311)
  - `tsa_offenders` — [`L313`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/miswire_audit.py#L313)
- uses (calls/refs, reference-scoped): [`Offender`](miswire_audit.md#Offender)
- used by: [`audit`](miswire_audit.md#audit), [`render_terminal`](miswire_audit.md#render_terminal), [`render_card`](miswire_audit.md#render_card)  (6 test-only)

### `Offender`
- def: [`tree_sitter_analyzer/miswire_audit.py:296`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/miswire_audit.py#L296)
- signature: `class Offender:`
- members:
  - `callee_file` — [`L300`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/miswire_audit.py#L300)
  - `callee_lang` — [`L301`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/miswire_audit.py#L301)
  - `callee_name` — [`L297`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/miswire_audit.py#L297)
  - `caller_file` — [`L298`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/miswire_audit.py#L298)
  - `caller_lang` — [`L299`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/miswire_audit.py#L299)
  - `line` — [`L302`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/miswire_audit.py#L302)
- used by: [`audit`](miswire_audit.md#audit), [`render_terminal`](miswire_audit.md#render_terminal), [`genuine_offenders`](miswire_audit.md#AuditResult.genuine_offenders), [`naive_offenders`](miswire_audit.md#AuditResult.naive_offenders), [`tsa_offenders`](miswire_audit.md#AuditResult.tsa_offenders)  (2 test-only)

## Functions
- `_build_name_maps(conn: Any, present: set[str] | None)` — [`L372`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/miswire_audit.py#L372) — Build name->languages and name->[(file,lang)] from current-repo defs.
- `_caller_builtins()` — [`L39`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/miswire_audit.py#L39) — Per-caller-language bare builtin names a basic name-only index could
- `_fmt_pct(n: int, total: int)` — [`L511`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/miswire_audit.py#L511)
- `_iter_symbol_defs(conn: Any)` — [`L332`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/miswire_audit.py#L332) — Yield ``(name, file_path, language)`` for every function/method/class def.
- `audit(project_root: str, *, reindex: bool = True, top: int = 5)` — [`L386`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/miswire_audit.py#L386) — Run the mis-wire audit against ``project_root`` using TSA's index. — documented in [tree_sitter_analyzer-ast_cache](../../concepts/tree_sitter_analyzer-ast_cache.md)
- `main(argv: list[str] | None = None)` — [`L604`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/miswire_audit.py#L604)
- `render_card(r: AuditResult)` — [`L579`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/miswire_audit.py#L579) — A copy-paste markdown social card.
- `render_terminal(r: AuditResult)` — [`L515`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/miswire_audit.py#L515)

## Module values
- `_CALLER_BUILTINS` — [`L292`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/miswire_audit.py#L292)
- `_DEF_KINDS` — [`L36`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/miswire_audit.py#L36)

