---
title: 'Module: tests/integration/test_parser_goldens.py'
type: catalog
provenance: extracted
module: tests/integration/test_parser_goldens.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `tests.integration.test_parser_goldens`/
symbols:
  load_and_normalize: load_and_normalize().
  test_language_golden: test_language_golden().
  stable_node_sort_key: stable_node_sort_key().
  normalize_path: normalize_path().
  make_hashable: make_hashable().
  WORKSPACE_ROOT: WORKSPACE_ROOT.
  get_logical_key: get_logical_key().
  GOLDENS_DIR: GOLDENS_DIR.
  normalize_id: normalize_id().
  normalize_labels: normalize_labels().
  PROJECTS_DIR: PROJECTS_DIR.
  is_generated_build_artifact: is_generated_build_artifact().
  get_goldens_list: get_goldens_list().
  TEST_ROOT: TEST_ROOT.
  clean_path: clean_path().
  FIXTURES_MARKER: FIXTURES_MARKER.
  VOLATILE_NODE_KEYS: VOLATILE_NODE_KEYS.
  CONTAINER_KEY_LABELS: CONTAINER_KEY_LABELS.
  GENERATED_BUILD_DIRS: GENERATED_BUILD_DIRS.
---
# Module: [`tests/integration/test_parser_goldens.py`](../../../../../../raw/code/codegraphcontext/tests/integration/test_parser_goldens.py)

## Functions
- `clean_path(p)` — [`L19`](../../../../../../raw/code/codegraphcontext/tests/integration/test_parser_goldens.py#L19)
- `get_goldens_list()` — [`L223`](../../../../../../raw/code/codegraphcontext/tests/integration/test_parser_goldens.py#L223)
- `get_logical_key(node, normalized_path)` — [`L61`](../../../../../../raw/code/codegraphcontext/tests/integration/test_parser_goldens.py#L61)
- `is_generated_build_artifact(normalized_path)` — [`L57`](../../../../../../raw/code/codegraphcontext/tests/integration/test_parser_goldens.py#L57)
- `load_and_normalize(nodes_path, edges_path, current_repo_root, bundle_repo_root=None)` — [`L109`](../../../../../../raw/code/codegraphcontext/tests/integration/test_parser_goldens.py#L109)
- `make_hashable(val)` — [`L84`](../../../../../../raw/code/codegraphcontext/tests/integration/test_parser_goldens.py#L84)
- `normalize_id(val)` — [`L91`](../../../../../../raw/code/codegraphcontext/tests/integration/test_parser_goldens.py#L91)
- `normalize_labels(labels)` — [`L22`](../../../../../../raw/code/codegraphcontext/tests/integration/test_parser_goldens.py#L22)
- `normalize_path(p, current_repo_root, bundle_repo_root=None)` — [`L33`](../../../../../../raw/code/codegraphcontext/tests/integration/test_parser_goldens.py#L33)
- `stable_node_sort_key(node)` — [`L94`](../../../../../../raw/code/codegraphcontext/tests/integration/test_parser_goldens.py#L94)
- `test_language_golden(project_name, update_goldens, tmp_path)` — [`L229`](../../../../../../raw/code/codegraphcontext/tests/integration/test_parser_goldens.py#L229)

## Module values
- `CONTAINER_KEY_LABELS` — [`L15`](../../../../../../raw/code/codegraphcontext/tests/integration/test_parser_goldens.py#L15)
- `FIXTURES_MARKER` — [`L31`](../../../../../../raw/code/codegraphcontext/tests/integration/test_parser_goldens.py#L31)
- `GENERATED_BUILD_DIRS` — [`L16`](../../../../../../raw/code/codegraphcontext/tests/integration/test_parser_goldens.py#L16)
- `GOLDENS_DIR` — [`L11`](../../../../../../raw/code/codegraphcontext/tests/integration/test_parser_goldens.py#L11)
- `PROJECTS_DIR` — [`L12`](../../../../../../raw/code/codegraphcontext/tests/integration/test_parser_goldens.py#L12)
- `TEST_ROOT` — [`L10`](../../../../../../raw/code/codegraphcontext/tests/integration/test_parser_goldens.py#L10)
- `VOLATILE_NODE_KEYS` — [`L14`](../../../../../../raw/code/codegraphcontext/tests/integration/test_parser_goldens.py#L14)
- `WORKSPACE_ROOT` — [`L13`](../../../../../../raw/code/codegraphcontext/tests/integration/test_parser_goldens.py#L13)

