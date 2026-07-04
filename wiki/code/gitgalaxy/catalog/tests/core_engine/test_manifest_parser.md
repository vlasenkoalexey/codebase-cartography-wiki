---
title: 'Module: tests/core_engine/test_manifest_parser.py'
type: catalog
provenance: extracted
module: tests/core_engine/test_manifest_parser.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `tests.core_engine.test_manifest_parser`/
symbols:
  parser: parser().
  test_package_json_npm_aliasing: test_package_json_npm_aliasing().
  test_package_json_direct_uri_resolution: test_package_json_direct_uri_resolution().
  test_package_json_invalid_json: test_package_json_invalid_json().
  test_package_json_empty_dependencies: test_package_json_empty_dependencies().
  test_package_lock_registry_spoofing: test_package_lock_registry_spoofing().
  test_requirements_txt_direct_uri_references: test_requirements_txt_direct_uri_references().
  test_requirements_txt_complex_constraints: test_requirements_txt_complex_constraints().
  test_pip_conf_insecure_registry: test_pip_conf_insecure_registry().
  test_pip_conf_trusted_registry: test_pip_conf_trusted_registry().
  test_multiple_manifests_simultaneously: test_multiple_manifests_simultaneously().
  test_unsupported_manifest_bypass: test_unsupported_manifest_bypass().
---
# Module: [`tests/core_engine/test_manifest_parser.py`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_manifest_parser.py)

## Functions
- `parser()` — [`L10`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_manifest_parser.py#L10) — Provides a fresh ManifestParser instance with a silenced logger for clean test output.
- `test_multiple_manifests_simultaneously(parser, tmp_path)` — [`L214`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_manifest_parser.py#L214) — Verifies the parser can handle a monorepo setup with multiple manifest formats at once.
- `test_package_json_direct_uri_resolution(parser, tmp_path)` — [`L50`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_manifest_parser.py#L50) — Verifies that direct file system or git repository overrides are flagged.
- `test_package_json_empty_dependencies(parser, tmp_path)` — [`L85`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_manifest_parser.py#L85) — Proves the parser does not crash when a manifest lacks dependency blocks entirely.
- `test_package_json_invalid_json(parser, tmp_path)` — [`L75`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_manifest_parser.py#L75) — Ensures the parser degrades gracefully without crashing if the structural definition is corrupted.
- `test_package_json_npm_aliasing(parser, tmp_path)` — [`L20`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_manifest_parser.py#L20) — Verifies that npm: aliases and scoped aliases are correctly dereferenced to their
- `test_package_lock_registry_spoofing(parser, tmp_path)` — [`L97`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_manifest_parser.py#L97) — Verifies that external, non-NPM registry resolutions are intercepted.
- `test_pip_conf_insecure_registry(parser, tmp_path)` — [`L179`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_manifest_parser.py#L179) — Verifies that HTTP (MitM vulnerable) or ngrok tunnel registries are instantly flagged
- `test_pip_conf_trusted_registry(parser, tmp_path)` — [`L198`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_manifest_parser.py#L198) — Ensures legitimate HTTPS internal registries (like Artifactory) do not trigger false positives.
- `test_requirements_txt_complex_constraints(parser, tmp_path)` — [`L157`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_manifest_parser.py#L157) — Proves the Regex engine correctly extracts the base package name even when
- `test_requirements_txt_direct_uri_references(parser, tmp_path)` — [`L132`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_manifest_parser.py#L132) — Verifies standard python packages are indexed and Direct URI references
- `test_unsupported_manifest_bypass(parser, tmp_path)` — [`L229`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_manifest_parser.py#L229) — Proves the parser gracefully skips unrelated files without crashing the loop.

