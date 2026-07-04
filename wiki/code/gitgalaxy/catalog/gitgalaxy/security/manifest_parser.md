---
title: 'Module: gitgalaxy/security/manifest_parser.py'
type: catalog
provenance: extracted
module: gitgalaxy/security/manifest_parser.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `gitgalaxy.security.manifest_parser`/ManifestParser#
symbols:
  ManifestParser.build_resolution_map: build_resolution_map().
  ManifestParser._parse_requirements_txt: _parse_requirements_txt().
  ManifestParser.logger: logger.
  ManifestParser: ''
  ManifestParser._parse_package_json: _parse_package_json().
  ManifestParser._parse_package_lock: _parse_package_lock().
  ManifestParser._parse_pip_conf: _parse_pip_conf().
  ManifestParser.python_pkg_regex: python_pkg_regex.
  ManifestParser.python_direct_uri_regex: python_direct_uri_regex.
  ManifestParser.__init__: __init__().
---
# Module: [`gitgalaxy/security/manifest_parser.py`](../../../../../../raw/code/gitgalaxy/gitgalaxy/security/manifest_parser.py)

## Classes
### `ManifestParser`
- def: [`gitgalaxy/security/manifest_parser.py:13`](../../../../../../raw/code/gitgalaxy/gitgalaxy/security/manifest_parser.py#L13)
- doc: Software Supply Chain Security (SSCS) Manifest Parser.
- signature: `class ManifestParser:`
- members:
  - `_parse_package_json(self, filepath: Path, resolution_map: dict)` — [`L61`](../../../../../../raw/code/gitgalaxy/gitgalaxy/security/manifest_parser.py#L61) — Parses active NPM dependencies. Normalizes NPM aliases to their upstream package names
  - `_parse_package_lock(self, filepath: Path, resolution_map: dict)` — [`L93`](../../../../../../raw/code/gitgalaxy/gitgalaxy/security/manifest_parser.py#L93) — Extracts absolute resolution URLs from package-lock.json v2/v3.
  - `_parse_pip_conf(self, filepath: Path, resolution_map: dict)` — [`L144`](../../../../../../raw/code/gitgalaxy/gitgalaxy/security/manifest_parser.py#L144) — Audits Python configuration files (pip.conf, .pypirc) for Dependency Confusion vulnerabilities
  - `_parse_requirements_txt(self, filepath: Path, resolution_map: dict)` — [`L118`](../../../../../../raw/code/gitgalaxy/gitgalaxy/security/manifest_parser.py#L118) — Extracts direct Python packages and flags absolute VCS/URI references.
  - `build_resolution_map(self, manifest_paths: list)` — [`L33`](../../../../../../raw/code/gitgalaxy/gitgalaxy/security/manifest_parser.py#L33) — Accepts a list of exact file paths and builds a global O(1) dependency resolution — documented in [gitgalaxy-galaxyscope](../../../concepts/gitgalaxy-galaxyscope.md)
  - `logger` — [`L23`](../../../../../../raw/code/gitgalaxy/gitgalaxy/security/manifest_parser.py#L23)
  - `python_direct_uri_regex` — [`L31`](../../../../../../raw/code/gitgalaxy/gitgalaxy/security/manifest_parser.py#L31)
  - `python_pkg_regex` — [`L28`](../../../../../../raw/code/gitgalaxy/gitgalaxy/security/manifest_parser.py#L28)
- protocol/private: `__init__`[`L22`](../../../../../../raw/code/gitgalaxy/gitgalaxy/security/manifest_parser.py#L22)
- used by: [`execute_pipeline`](../galaxyscope.md#Orchestrator.execute_pipeline)  (1 test-only)

