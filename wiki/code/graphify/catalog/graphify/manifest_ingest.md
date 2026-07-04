---
title: 'Module: graphify/manifest_ingest.py'
type: catalog
provenance: extracted
module: graphify/manifest_ingest.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `graphify.manifest_ingest`/
symbols:
  extract_package_manifest: extract_package_manifest().
  _PARSERS: _PARSERS.
  is_package_manifest_path: is_package_manifest_path().
  _parse_apm: _parse_apm().
  _pkg_id: _pkg_id().
  _parse_pyproject: _parse_pyproject().
  PACKAGE_MANIFEST_NAMES.PACKAGE_MANIFEST_NAMES: PACKAGE_MANIFEST_NAMES.PACKAGE_MANIFEST_NAMES.
  _MAX_MANIFEST_BYTES: _MAX_MANIFEST_BYTES.
  _coerce_deps: _coerce_deps().
  _parse_apm_fallback: _parse_apm_fallback().
  _pep508_name: _pep508_name().
  _parse_gomod: _parse_gomod().
  _parse_pom: _parse_pom().
  __all__: __all__.
---
# Module: [`graphify/manifest_ingest.py`](../../../../../raw/code/graphify/graphify/manifest_ingest.py)

## Functions
- `_coerce_deps(value: Any)` — [`L114`](../../../../../raw/code/graphify/graphify/manifest_ingest.py#L114) — A dependency block may be a list of names or a name->spec map.
- `_parse_apm(text: str)` — [`L129`](../../../../../raw/code/graphify/graphify/manifest_ingest.py#L129)
- `_parse_apm_fallback(text: str)` — [`L144`](../../../../../raw/code/graphify/graphify/manifest_ingest.py#L144) — Minimal line parser for apm.yml when PyYAML is unavailable: a top-level
- `_parse_gomod(text: str)` — [`L196`](../../../../../raw/code/graphify/graphify/manifest_ingest.py#L196)
- `_parse_pom(text: str)` — [`L224`](../../../../../raw/code/graphify/graphify/manifest_ingest.py#L224)
- `_parse_pyproject(text: str)` — [`L174`](../../../../../raw/code/graphify/graphify/manifest_ingest.py#L174)
- `_pep508_name(spec: str)` — [`L169`](../../../../../raw/code/graphify/graphify/manifest_ingest.py#L169) — `requests>=2.0` -> `requests`; `pkg[extra]==1; python_version<'3.9'` -> `pkg`.
- `_pkg_id(name: str)` — [`L44`](../../../../../raw/code/graphify/graphify/manifest_ingest.py#L44) — Canonical package node id, keyed by package NAME so every reference to the
- `extract_package_manifest(path: Path)` — [`L51`](../../../../../raw/code/graphify/graphify/manifest_ingest.py#L51) — Parse a package manifest into a canonical package node + ``depends_on`` edges.
- `is_package_manifest_path(path: Path)` — [`L39`](../../../../../raw/code/graphify/graphify/manifest_ingest.py#L39) — True if ``path`` is a recognized package manifest (by filename). — documented in [graphify-detect](../../concepts/graphify-detect.md)

## Module values
- `PACKAGE_MANIFEST_NAMES` — [`L28`](../../../../../raw/code/graphify/graphify/manifest_ingest.py#L28)
- `_MAX_MANIFEST_BYTES` — [`L36`](../../../../../raw/code/graphify/graphify/manifest_ingest.py#L36)
- `_PARSERS` — [`L242`](../../../../../raw/code/graphify/graphify/manifest_ingest.py#L242)
- `__all__` — [`L25`](../../../../../raw/code/graphify/graphify/manifest_ingest.py#L25)

