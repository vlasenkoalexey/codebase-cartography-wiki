---
title: 'Module: tests/test_cargo_introspect.py'
type: catalog
provenance: extracted
module: tests/test_cargo_introspect.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_cargo_introspect`/
symbols:
  _write_manifest: _write_manifest().
  test_cargo_introspect_workspace_internal_dependency_only: test_cargo_introspect_workspace_internal_dependency_only().
  test_cargo_introspect_malformed_toml_reports_parser_error: test_cargo_introspect_malformed_toml_reports_parser_error().
  test_cargo_introspect_degenerate_manifests_return_empty_or_skip_bad_deps: test_cargo_introspect_degenerate_manifests_return_empty_or_skip_bad_deps().
  test_cargo_introspect_old_manifest_keeps_internal_path_dep_and_skips_external: test_cargo_introspect_old_manifest_keeps_internal_path_dep_and_skips_external().
  test_cargo_introspect_modern_virtual_and_root_package_workspaces: test_cargo_introspect_modern_virtual_and_root_package_workspaces().
  test_cargo_introspect_large_workspace_dependency_chain: test_cargo_introspect_large_workspace_dependency_chain().
---
# Module: [`tests/test_cargo_introspect.py`](../../../../../raw/code/graphify/tests/test_cargo_introspect.py)

## Functions
- `_write_manifest(path, content)` — [`L6`](../../../../../raw/code/graphify/tests/test_cargo_introspect.py#L6)
- `test_cargo_introspect_degenerate_manifests_return_empty_or_skip_bad_deps(tmp_path)` — [`L93`](../../../../../raw/code/graphify/tests/test_cargo_introspect.py#L93) — Degenerate but parseable manifests should not invent graph data or crash.
- `test_cargo_introspect_large_workspace_dependency_chain(tmp_path)` — [`L306`](../../../../../raw/code/graphify/tests/test_cargo_introspect.py#L306) — Large deterministic workspace proves chain extraction scales by shape, not timing.
- `test_cargo_introspect_malformed_toml_reports_parser_error(tmp_path)` — [`L76`](../../../../../raw/code/graphify/tests/test_cargo_introspect.py#L76) — Malformed manifests surface the TOML parser failure, not an arbitrary crash.
- `test_cargo_introspect_modern_virtual_and_root_package_workspaces(tmp_path)` — [`L194`](../../../../../raw/code/graphify/tests/test_cargo_introspect.py#L194) — Modern workspace forms cover virtual roots, workspace deps, and root packages.
- `test_cargo_introspect_old_manifest_keeps_internal_path_dep_and_skips_external(tmp_path)` — [`L147`](../../../../../raw/code/graphify/tests/test_cargo_introspect.py#L147) — Legacy manifests still resolve path deps and ignore bare-string externals.
- `test_cargo_introspect_workspace_internal_dependency_only(tmp_path)` — [`L10`](../../../../../raw/code/graphify/tests/test_cargo_introspect.py#L10) — Real workspace: pin raw graph fields while excluding registry-only deps.

