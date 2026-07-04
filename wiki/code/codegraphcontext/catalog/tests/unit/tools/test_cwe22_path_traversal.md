---
title: 'Module: tests/unit/tools/test_cwe22_path_traversal.py'
type: catalog
provenance: extracted
module: tests/unit/tools/test_cwe22_path_traversal.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `tests.unit.tools.test_cwe22_path_traversal`/
symbols:
  _make_mocks: _make_mocks().
  test_rejects_absolute_path_outside_cwd: test_rejects_absolute_path_outside_cwd().
  test_rejects_relative_path_traversal: test_rejects_relative_path_traversal().
  test_rejects_home_ssh_directory: test_rejects_home_ssh_directory().
  test_rejects_symlink_escape: test_rejects_symlink_escape().
  test_rejects_dot_dot_encoding_variants: test_rejects_dot_dot_encoding_variants().
  test_allows_subdirectory_of_cwd: test_allows_subdirectory_of_cwd().
  test_allows_path_via_env_allowlist: test_allows_path_via_env_allowlist().
  test_allows_multiple_env_roots: test_allows_multiple_env_roots().
---
# Module: [`tests/unit/tools/test_cwe22_path_traversal.py`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cwe22_path_traversal.py)

## Functions
- `_make_mocks()` — [`L22`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cwe22_path_traversal.py#L22) — Create mock dependencies for add_code_to_graph.
- `test_allows_multiple_env_roots()` — [`L160`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cwe22_path_traversal.py#L160) — Multiple colon-separated paths in CGC_ALLOWED_ROOTS all work.
- `test_allows_path_via_env_allowlist()` — [`L142`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cwe22_path_traversal.py#L142) — Paths in CGC_ALLOWED_ROOTS should be allowed even if outside cwd.
- `test_allows_subdirectory_of_cwd()` — [`L119`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cwe22_path_traversal.py#L119) — Paths that are subdirectories of cwd should be allowed.
- `test_rejects_absolute_path_outside_cwd()` — [`L33`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cwe22_path_traversal.py#L33) — Indexing /etc (or any path outside cwd) should be rejected.
- `test_rejects_dot_dot_encoding_variants()` — [`L104`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cwe22_path_traversal.py#L104) — Various path encoding tricks should all be rejected.
- `test_rejects_home_ssh_directory()` — [`L65`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cwe22_path_traversal.py#L65) — Indexing ~/.ssh should be rejected.
- `test_rejects_relative_path_traversal()` — [`L49`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cwe22_path_traversal.py#L49) — Paths with .. that escape the working directory should be rejected.
- `test_rejects_symlink_escape(tmp_path)` — [`L82`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_cwe22_path_traversal.py#L82) — A symlink inside cwd that points outside should be rejected after resolution.

