---
title: 'Module: scripts/compare_backend_snapshots.py'
type: catalog
provenance: extracted
module: scripts/compare_backend_snapshots.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `scripts.compare_backend_snapshots`/
symbols:
  main: main().
  extract_entities: extract_entities().
  print_list: print_list().
  normalize_json: normalize_json().
  compare_json_recursive: compare_json_recursive().
  classify_severity: classify_severity().
  compare_text: compare_text().
  compare_lists: compare_lists().
  load_text_lines: load_text_lines().
  canonical_json: canonical_json().
  normalize_line: normalize_line().
  load_json: load_json().
  jaccard_similarity: jaccard_similarity().
  SeveritySummary: SeveritySummary#
  SeveritySummary.critical: SeveritySummary#critical.
  SeveritySummary.minor: SeveritySummary#minor.
  normalize_whitespace: normalize_whitespace().
  parse_args: parse_args().
  ensure_exists: ensure_exists().
---
# Module: [`scripts/compare_backend_snapshots.py`](../../../../../raw/code/codegraphcontext/scripts/compare_backend_snapshots.py)

## Classes
### `SeveritySummary`
- def: [`scripts/compare_backend_snapshots.py:189`](../../../../../raw/code/codegraphcontext/scripts/compare_backend_snapshots.py#L189)
- signature: `class SeveritySummary:`
- members:
  - `critical` — [`L190`](../../../../../raw/code/codegraphcontext/scripts/compare_backend_snapshots.py#L190)
  - `minor` — [`L191`](../../../../../raw/code/codegraphcontext/scripts/compare_backend_snapshots.py#L191)
- used by: [`main`](compare_backend_snapshots.md#main), [`classify_severity`](compare_backend_snapshots.md#classify_severity)

## Functions
- `canonical_json(value: Any)` — [`L55`](../../../../../raw/code/codegraphcontext/scripts/compare_backend_snapshots.py#L55)
- `classify_severity(callers: Dict[str, Any], deps: Dict[str, Any], content: Dict[str, Any])` — [`L194`](../../../../../raw/code/codegraphcontext/scripts/compare_backend_snapshots.py#L194)
- `compare_json_recursive(neo: Any, kuzu: Any, path: str = "$")` — [`L114`](../../../../../raw/code/codegraphcontext/scripts/compare_backend_snapshots.py#L114)
- `compare_lists(path: str, neo_list: List[Any], kuzu_list: List[Any])` — [`L96`](../../../../../raw/code/codegraphcontext/scripts/compare_backend_snapshots.py#L96)
- `compare_text(neo_path: Path, kuzu_path: Path, lowercase: bool)` — [`L73`](../../../../../raw/code/codegraphcontext/scripts/compare_backend_snapshots.py#L73)
- `ensure_exists(path: Path)` — [`L231`](../../../../../raw/code/codegraphcontext/scripts/compare_backend_snapshots.py#L231)
- `extract_entities(obj: Any, path: str = "$", out: Set[str] | None = None)` — [`L173`](../../../../../raw/code/codegraphcontext/scripts/compare_backend_snapshots.py#L173)
- `jaccard_similarity(a: Set[str], b: Set[str])` — [`L66`](../../../../../raw/code/codegraphcontext/scripts/compare_backend_snapshots.py#L66)
- `load_json(path: Path)` — [`L59`](../../../../../raw/code/codegraphcontext/scripts/compare_backend_snapshots.py#L59)
- `load_text_lines(path: Path, lowercase: bool)` — [`L34`](../../../../../raw/code/codegraphcontext/scripts/compare_backend_snapshots.py#L34)
- `main()` — [`L244`](../../../../../raw/code/codegraphcontext/scripts/compare_backend_snapshots.py#L244)
- `normalize_json(value: Any)` — [`L41`](../../../../../raw/code/codegraphcontext/scripts/compare_backend_snapshots.py#L41) — Normalize JSON recursively while ignoring ordering differences.
- `normalize_line(line: str, lowercase: bool)` — [`L27`](../../../../../raw/code/codegraphcontext/scripts/compare_backend_snapshots.py#L27)
- `normalize_whitespace(text: str)` — [`L23`](../../../../../raw/code/codegraphcontext/scripts/compare_backend_snapshots.py#L23)
- `parse_args()` — [`L218`](../../../../../raw/code/codegraphcontext/scripts/compare_backend_snapshots.py#L218)
- `print_list(label: str, items: List[Any], max_items: int)` — [`L236`](../../../../../raw/code/codegraphcontext/scripts/compare_backend_snapshots.py#L236)

