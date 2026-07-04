---
title: 'Module: tests/unit/mcp/test_parser_readiness_tool.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_parser_readiness_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_parser_readiness_tool`/
symbols:
  _write_pyproject: _write_pyproject().
  test_parser_readiness_tool_returns_json_installed: test_parser_readiness_tool_returns_json_installed().
  test_parser_readiness_tool_returns_json_not_installed: test_parser_readiness_tool_returns_json_not_installed().
  test_parser_readiness_toon_installed_shows_version_and_url: test_parser_readiness_toon_installed_shows_version_and_url().
  test_parser_readiness_toon_not_installed_shows_empty_version: test_parser_readiness_toon_not_installed_shows_empty_version().
  test_parser_readiness_partial_install_plugin_without_loader: test_parser_readiness_partial_install_plugin_without_loader().
  test_parser_readiness_concurrent_calls_are_safe: test_parser_readiness_concurrent_calls_are_safe().
  test_parser_readiness_envelope_contract_holds_for_both_formats: test_parser_readiness_envelope_contract_holds_for_both_formats().
  test_parser_readiness_tool_defaults_to_toon: test_parser_readiness_tool_defaults_to_toon().
  test_parser_readiness_unknown_language_is_rejected_at_validation: test_parser_readiness_unknown_language_is_rejected_at_validation().
  test_parser_readiness_unknown_language_via_builder_returns_error: test_parser_readiness_unknown_language_via_builder_returns_error().
  test_parser_readiness_partial_install_missing_parser_package: test_parser_readiness_partial_install_missing_parser_package().
  test_parser_readiness_signals_surface_abi_and_scanner_state: test_parser_readiness_signals_surface_abi_and_scanner_state().
  _make_fake_importlib_metadata: _make_fake_importlib_metadata().
  test_parser_readiness_recommends_declared_parser_without_plugin: test_parser_readiness_recommends_declared_parser_without_plugin().
  test_parser_readiness_can_report_supported_language: test_parser_readiness_can_report_supported_language().
  test_parser_readiness_tool_validates_arguments: test_parser_readiness_tool_validates_arguments().
  test_parser_readiness_handles_corrupted_pyproject: test_parser_readiness_handles_corrupted_pyproject().
  _LEGAL_VERDICTS: _LEGAL_VERDICTS.
  _SWIFT_PYPROJECT: _SWIFT_PYPROJECT.
  _FAKE_SWIFT_DIST: _FAKE_SWIFT_DIST.
  _FakeMetadata.get: _FakeMetadata#get().
  _FakeMetadata.get_all: _FakeMetadata#get_all().
  _FakeDistribution.__init__: _FakeDistribution#__init__().
  _make_fake_importlib_metadata._FakeImportlibMetadata.distribution: _make_fake_importlib_metadata()._FakeImportlibMetadata#distribution().
  _FakeMetadata: _FakeMetadata#
  _FakeMetadata._home_page: _FakeMetadata#_home_page.
  _FakeMetadata._project_urls: _FakeMetadata#_project_urls.
  _FakeDistribution: _FakeDistribution#
  _make_fake_importlib_metadata._FakeImportlibMetadata: _make_fake_importlib_metadata()._FakeImportlibMetadata#
  _FakeMetadata.__init__: _FakeMetadata#__init__().
  _FakeDistribution.version: _FakeDistribution#version.
  _FakeDistribution.metadata: _FakeDistribution#metadata.
  _make_fake_importlib_metadata._FakeImportlibMetadata.PackageNotFoundError: _make_fake_importlib_metadata()._FakeImportlibMetadata#PackageNotFoundError.
---
# Module: [`tests/unit/mcp/test_parser_readiness_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_parser_readiness_tool.py)

## Classes
### `_FakeDistribution`
- def: [`tests/unit/mcp/test_parser_readiness_tool.py:118`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_parser_readiness_tool.py#L118)
- doc: Fake importlib.metadata.Distribution for patching.
- signature: `class _FakeDistribution:`
- members:
  - `metadata` — [`L123`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_parser_readiness_tool.py#L123)
  - `version` — [`L122`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_parser_readiness_tool.py#L122)
- protocol/private: `__init__`[`L121`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_parser_readiness_tool.py#L121)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `_FakeImportlibMetadata`
- def: [`tests/unit/mcp/test_parser_readiness_tool.py:153`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_parser_readiness_tool.py#L153)
- signature: `class _FakeImportlibMetadata:`
- members:
  - `distribution(name: str)` — [`L157`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_parser_readiness_tool.py#L157)
  - `PackageNotFoundError` — [`L154`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_parser_readiness_tool.py#L154)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `_FakeMetadata`
- def: [`tests/unit/mcp/test_parser_readiness_tool.py:100`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_parser_readiness_tool.py#L100)
- doc: Minimal email.message.Message stand-in for importlib distribution metadata.
- signature: `class _FakeMetadata:`
- members:
  - `get(self, key: str)` — [`L107`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_parser_readiness_tool.py#L107)
  - `get_all(self, key: str)` — [`L112`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_parser_readiness_tool.py#L112)
- protocol/private: `__init__`[`L103`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_parser_readiness_tool.py#L103), `_home_page`[`L104`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_parser_readiness_tool.py#L104), `_project_urls`[`L105`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_parser_readiness_tool.py#L105)
- used by: (1 test-only callers)

## Functions
- `_make_fake_importlib_metadata(*, installed: bool)` — [`L143`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_parser_readiness_tool.py#L143) — Return a fake importlib_metadata namespace for monkeypatching.
- `_write_pyproject(path, body: str)` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_parser_readiness_tool.py#L35)
- `test_parser_readiness_can_report_supported_language(tmp_path)` — [`L75`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_parser_readiness_tool.py#L75) — A requested implemented language should return a focused readiness record.
- `test_parser_readiness_concurrent_calls_are_safe(tmp_path)` — [`L551`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_parser_readiness_tool.py#L551) — Parallel execute calls must return independent results.
- `test_parser_readiness_envelope_contract_holds_for_both_formats(tmp_path)` — [`L593`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_parser_readiness_tool.py#L593) — Both JSON and TOON outputs must carry the canonical envelope.
- `test_parser_readiness_handles_corrupted_pyproject(tmp_path)` — [`L523`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_parser_readiness_tool.py#L523) — A malformed pyproject.toml must produce a clean error envelope.
- `test_parser_readiness_partial_install_missing_parser_package(tmp_path)` — [`L441`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_parser_readiness_tool.py#L441) — A language requested without any parser package or plugin is missing.
- `test_parser_readiness_partial_install_plugin_without_loader(tmp_path)` — [`L395`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_parser_readiness_tool.py#L395) — A plugin entrypoint without a loader mapping is a partial install.
- `test_parser_readiness_recommends_declared_parser_without_plugin(tmp_path)` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_parser_readiness_tool.py#L39) — A parser extra without a plugin should become an actionable candidate.
- `test_parser_readiness_signals_surface_abi_and_scanner_state(tmp_path)` — [`L472`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_parser_readiness_tool.py#L472) — The readiness signals must expose ABI / grammar / scanner status.
- `test_parser_readiness_tool_defaults_to_toon(tmp_path)` — [`L245`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_parser_readiness_tool.py#L245) — TOON output keeps MCP parser-readiness advice compact.
- `test_parser_readiness_tool_returns_json_installed(tmp_path, monkeypatch)` — [`L166`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_parser_readiness_tool.py#L166) — JSON output: installed state — parser_package_version == installed version.
- `test_parser_readiness_tool_returns_json_not_installed(tmp_path, monkeypatch)` — [`L208`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_parser_readiness_tool.py#L208) — JSON output: not-installed state — parser_package_version == "".
- `test_parser_readiness_tool_validates_arguments(tmp_path)` — [`L324`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_parser_readiness_tool.py#L324) — Invalid enum and type inputs should fail before project inspection.
- `test_parser_readiness_toon_installed_shows_version_and_url(tmp_path, monkeypatch)` — [`L264`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_parser_readiness_tool.py#L264) — TOON output: installed state — pkg_version and url are populated.
- `test_parser_readiness_toon_not_installed_shows_empty_version(tmp_path, monkeypatch)` — [`L294`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_parser_readiness_tool.py#L294) — TOON output: not-installed state — pkg_version=- and no url.
- `test_parser_readiness_unknown_language_is_rejected_at_validation(tmp_path)` — [`L345`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_parser_readiness_tool.py#L345) — Language names outside the safe identifier shape fail before any I/O.
- `test_parser_readiness_unknown_language_via_builder_returns_error(tmp_path)` — [`L372`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_parser_readiness_tool.py#L372) — The shared builder returns a structured error for unknown languages.

## Module values
- `_FAKE_SWIFT_DIST` — [`L126`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_parser_readiness_tool.py#L126)
- `_LEGAL_VERDICTS` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_parser_readiness_tool.py#L30)
- `_SWIFT_PYPROJECT` — [`L134`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_parser_readiness_tool.py#L134)

