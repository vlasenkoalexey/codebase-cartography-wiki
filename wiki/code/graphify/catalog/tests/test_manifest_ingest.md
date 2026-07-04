---
title: 'Module: tests/test_manifest_ingest.py'
type: catalog
provenance: extracted
module: tests/test_manifest_ingest.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_manifest_ingest`/
symbols:
  test_manifests_classify_as_code_not_document: test_manifests_classify_as_code_not_document().
  _write: _write().
  test_apm_parses_name_and_deps: test_apm_parses_name_and_deps().
  test_pyproject_parses_pep508_deps: test_pyproject_parses_pep508_deps().
  test_gomod_parses_module_and_requires: test_gomod_parses_module_and_requires().
  test_pom_parses_artifact_and_deps: test_pom_parses_artifact_and_deps().
  test_apm_dependency_collapses_to_single_canonical_node: test_apm_dependency_collapses_to_single_canonical_node().
  test_external_dependency_edge_pruned_not_orphaned: test_external_dependency_edge_pruned_not_orphaned().
  test_malformed_manifest_does_not_crash: test_malformed_manifest_does_not_crash().
  _pkg_nodes: _pkg_nodes().
---
# Module: [`tests/test_manifest_ingest.py`](../../../../../raw/code/graphify/tests/test_manifest_ingest.py)

## Functions
- `_pkg_nodes(result)` — [`L33`](../../../../../raw/code/graphify/tests/test_manifest_ingest.py#L33)
- `_write(p: Path, text: str)` — [`L14`](../../../../../raw/code/graphify/tests/test_manifest_ingest.py#L14)
- `test_apm_dependency_collapses_to_single_canonical_node(tmp_path)` — [`L80`](../../../../../raw/code/graphify/tests/test_manifest_ingest.py#L80)
- `test_apm_parses_name_and_deps(tmp_path)` — [`L37`](../../../../../raw/code/graphify/tests/test_manifest_ingest.py#L37)
- `test_external_dependency_edge_pruned_not_orphaned(tmp_path)` — [`L102`](../../../../../raw/code/graphify/tests/test_manifest_ingest.py#L102)
- `test_gomod_parses_module_and_requires(tmp_path)` — [`L57`](../../../../../raw/code/graphify/tests/test_manifest_ingest.py#L57)
- `test_malformed_manifest_does_not_crash(tmp_path)` — [`L111`](../../../../../raw/code/graphify/tests/test_manifest_ingest.py#L111)
- `test_manifests_classify_as_code_not_document(tmp_path)` — [`L22`](../../../../../raw/code/graphify/tests/test_manifest_ingest.py#L22)
- `test_pom_parses_artifact_and_deps(tmp_path)` — [`L67`](../../../../../raw/code/graphify/tests/test_manifest_ingest.py#L67)
- `test_pyproject_parses_pep508_deps(tmp_path)` — [`L47`](../../../../../raw/code/graphify/tests/test_manifest_ingest.py#L47)

