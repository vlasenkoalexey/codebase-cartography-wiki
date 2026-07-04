---
title: 'Module: understand-anything-plugin/skills/understand/merge-batch-graphs.py'
type: catalog
provenance: extracted
module: understand-anything-plugin/skills/understand/merge-batch-graphs.py
status: fresh
symbol_base: scip-python python understand-anything 0.0.0 `understand-anything-plugin.skills.understand.merge-batch-graphs`/
symbols:
  production_candidates: production_candidates().
  _add_unique: _add_unique().
  merge_and_normalize: merge_and_normalize().
  link_tests: link_tests().
  _join: _join().
  is_test_path: is_test_path().
  main: main().
  VALID_NODE_PREFIXES: VALID_NODE_PREFIXES.
  _js_ts_sibling_candidates: _js_ts_sibling_candidates().
  normalize_direction: normalize_direction().
  normalize_node_id: normalize_node_id().
  normalize_complexity: normalize_complexity().
  _JS_TS_TEST_EXTS._JS_TS_TEST_EXTS: _JS_TS_TEST_EXTS._JS_TS_TEST_EXTS.
  _num: _num().
  classify_id_fix: classify_id_fix().
  _basename: _basename().
  _swap_tested_by_in_place: _swap_tested_by_in_place().
  TYPE_TO_PREFIX.TYPE_TO_PREFIX: TYPE_TO_PREFIX.TYPE_TO_PREFIX.
  COMPLEXITY_MAP.COMPLEXITY_MAP: COMPLEXITY_MAP.COMPLEXITY_MAP.
  _JS_TS_EXTS._JS_TS_EXTS: _JS_TS_EXTS._JS_TS_EXTS.
  _MIRROR_PRODUCTION_ROOTS._MIRROR_PRODUCTION_ROOTS: _MIRROR_PRODUCTION_ROOTS._MIRROR_PRODUCTION_ROOTS.
  VALID_COMPLEXITY: VALID_COMPLEXITY.
  load_batch: load_batch().
  _path_segments: _path_segments().
  _strip_test_infix: _strip_test_infix().
  _file_node_path: _file_node_path().
  _ensure_tested_tag: _ensure_tested_tag().
  recover_imports_from_scan: recover_imports_from_scan().
  _TEST_NAME_PATTERNS._TEST_NAME_PATTERNS: _TEST_NAME_PATTERNS._TEST_NAME_PATTERNS.
  _DIRECTION_ALIASES._DIRECTION_ALIASES: _DIRECTION_ALIASES._DIRECTION_ALIASES.
  _VALID_DIRECTIONS._VALID_DIRECTIONS: _VALID_DIRECTIONS._VALID_DIRECTIONS.
---
# Module: [`understand-anything-plugin/skills/understand/merge-batch-graphs.py`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand/merge-batch-graphs.py)

## Functions
- `_add_unique(out: list[str], path: str)` — [`L325`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand/merge-batch-graphs.py#L325) — Append `path` to `out` unless it is empty or already present. — documented in [understand-anything-plugin-skills-understand-merge-batch-graphs](../../../../concepts/understand-anything-plugin-skills-understand-merge-batch-graphs.md)
- `_basename(path: str)` — [`L283`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand/merge-batch-graphs.py#L283)
- `_ensure_tested_tag(node: dict[str, Any])` — [`L538`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand/merge-batch-graphs.py#L538) — Append "tested" to `node["tags"]`, coercing malformed `tags` to a — documented in [understand-anything-plugin-skills-understand-merge-batch-graphs](../../../../concepts/understand-anything-plugin-skills-understand-merge-batch-graphs.md)
- `_file_node_path(node: dict[str, Any])` — [`L509`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand/merge-batch-graphs.py#L509) — Return the relative project path for a `file:`-prefixed node, else None.
- `_join(dir_path: str, name: str)` — [`L319`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand/merge-batch-graphs.py#L319) — Join a (possibly empty) directory path to a basename with a single
- `_js_ts_sibling_candidates(dir_path: str, base_stem: str)` — [`L331`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand/merge-batch-graphs.py#L331) — Build sibling candidates for a JS/TS family base stem. — documented in [understand-anything-plugin-skills-understand-merge-batch-graphs](../../../../concepts/understand-anything-plugin-skills-understand-merge-batch-graphs.md)
- `_num(v: Any)` — [`L124`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand/merge-batch-graphs.py#L124) — Coerce a value to float for safe comparison (handles string weights). — documented in [understand-anything-plugin-skills-understand-merge-batch-graphs](../../../../concepts/understand-anything-plugin-skills-understand-merge-batch-graphs.md)
- `_path_segments(path: str)` — [`L278`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand/merge-batch-graphs.py#L278) — Split a relative POSIX-style path into segments (ignoring empties).
- `_strip_test_infix(stem: str)` — [`L310`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand/merge-batch-graphs.py#L310) — For a JS/TS-family stem like `foo.test` or `foo.spec`, strip the — documented in [understand-anything-plugin-skills-understand-merge-batch-graphs](../../../../concepts/understand-anything-plugin-skills-understand-merge-batch-graphs.md)
- `_swap_tested_by_in_place(edge: dict[str, Any], original_src: str, original_tgt: str)` — [`L520`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand/merge-batch-graphs.py#L520) — Flip an inverted `tested_by` edge so source becomes production and — documented in [understand-anything-plugin-skills-understand-merge-batch-graphs](../../../../concepts/understand-anything-plugin-skills-understand-merge-batch-graphs.md)
- `classify_id_fix(original: str, corrected: str)` — [`L154`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand/merge-batch-graphs.py#L154) — Return a human-readable pattern label for an ID correction. — documented in [understand-anything-plugin-skills-understand-merge-batch-graphs](../../../../concepts/understand-anything-plugin-skills-understand-merge-batch-graphs.md)
- `is_test_path(path: str)` — [`L287`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand/merge-batch-graphs.py#L287) — Return True if `path` looks like a test file by basename convention. — documented in [understand-anything-plugin-skills-understand-merge-batch-graphs](../../../../concepts/understand-anything-plugin-skills-understand-merge-batch-graphs.md)
- `link_tests(nodes_by_id: dict[str, dict[str, Any]], edges: list[dict[str, Any]])` — [`L556`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand/merge-batch-graphs.py#L556) — Canonicalize `tested_by` edges and link unmatched test files. — documented in [understand-anything-plugin-skills-understand-merge-batch-graphs](../../../../concepts/understand-anything-plugin-skills-understand-merge-batch-graphs.md)
- `load_batch(path: Path)` — [`L134`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand/merge-batch-graphs.py#L134) — Load a batch JSON file, tolerating malformed files.
- `main()` — [`L1003`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand/merge-batch-graphs.py#L1003) — documented in [understand-anything-plugin-skills-understand-merge-batch-graphs](../../../../concepts/understand-anything-plugin-skills-understand-merge-batch-graphs.md)
- `merge_and_normalize(batches: list[dict[str, Any]])` — [`L724`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand/merge-batch-graphs.py#L724) — Merge batch results and normalize. Returns (assembled_graph, report_lines). — documented in [understand-anything-plugin-skills-understand-merge-batch-graphs](../../../../concepts/understand-anything-plugin-skills-understand-merge-batch-graphs.md)
- `normalize_complexity(value: Any)` — [`L224`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand/merge-batch-graphs.py#L224) — Normalize a complexity value. Returns (normalized, status). — documented in [understand-anything-plugin-skills-understand-merge-batch-graphs](../../../../concepts/understand-anything-plugin-skills-understand-merge-batch-graphs.md)
- `normalize_direction(value: Any)` — [`L115`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand/merge-batch-graphs.py#L115) — Canonicalize an edge `direction` value to one of the schema enum members. — documented in [understand-anything-plugin-skills-understand-merge-batch-graphs](../../../../concepts/understand-anything-plugin-skills-understand-merge-batch-graphs.md)
- `normalize_node_id(node_id: str, node: dict[str, Any])` — [`L178`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand/merge-batch-graphs.py#L178) — Normalize a node ID, returning the corrected version. — documented in [understand-anything-plugin-skills-understand-merge-batch-graphs](../../../../concepts/understand-anything-plugin-skills-understand-merge-batch-graphs.md)
- `production_candidates(test_path: str)` — [`L340`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand/merge-batch-graphs.py#L340) — For a test file path, return ordered candidate production paths. — documented in [understand-anything-plugin-skills-understand-merge-batch-graphs](../../../../concepts/understand-anything-plugin-skills-understand-merge-batch-graphs.md)
- `recover_imports_from_scan(assembled: dict[str, Any], scan_result_path: Path)` — [`L913`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand/merge-batch-graphs.py#L913) — Re-emit any `imports` edges that exist in `scan-result.json#importMap`

## Module values
- `COMPLEXITY_MAP` — [`L68`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand/merge-batch-graphs.py#L68) — documented in [understand-anything-plugin-skills-understand-merge-batch-graphs](../../../../concepts/understand-anything-plugin-skills-understand-merge-batch-graphs.md)
- `TYPE_TO_PREFIX` — [`L42`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand/merge-batch-graphs.py#L42) — documented in [understand-anything-plugin-skills-understand-merge-batch-graphs](../../../../concepts/understand-anything-plugin-skills-understand-merge-batch-graphs.md)
- `VALID_COMPLEXITY` — [`L78`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand/merge-batch-graphs.py#L78) — documented in [understand-anything-plugin-skills-understand-merge-batch-graphs](../../../../concepts/understand-anything-plugin-skills-understand-merge-batch-graphs.md)
- `VALID_NODE_PREFIXES` — [`L32`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand/merge-batch-graphs.py#L32) — documented in [understand-anything-plugin-skills-understand-merge-batch-graphs](../../../../concepts/understand-anything-plugin-skills-understand-merge-batch-graphs.md)
- `_DIRECTION_ALIASES` — [`L111`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand/merge-batch-graphs.py#L111)
- `_JS_TS_EXTS` — [`L85`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand/merge-batch-graphs.py#L85) — documented in [understand-anything-plugin-skills-understand-merge-batch-graphs](../../../../concepts/understand-anything-plugin-skills-understand-merge-batch-graphs.md)
- `_JS_TS_TEST_EXTS` — [`L86`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand/merge-batch-graphs.py#L86) — documented in [understand-anything-plugin-skills-understand-merge-batch-graphs](../../../../concepts/understand-anything-plugin-skills-understand-merge-batch-graphs.md)
- `_MIRROR_PRODUCTION_ROOTS` — [`L90`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand/merge-batch-graphs.py#L90) — documented in [understand-anything-plugin-skills-understand-merge-batch-graphs](../../../../concepts/understand-anything-plugin-skills-understand-merge-batch-graphs.md)
- `_TEST_NAME_PATTERNS` — [`L97`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand/merge-batch-graphs.py#L97) — documented in [understand-anything-plugin-skills-understand-merge-batch-graphs](../../../../concepts/understand-anything-plugin-skills-understand-merge-batch-graphs.md)
- `_VALID_DIRECTIONS` — [`L112`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand/merge-batch-graphs.py#L112)

