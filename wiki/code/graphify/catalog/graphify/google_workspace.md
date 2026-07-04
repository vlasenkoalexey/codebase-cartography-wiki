---
title: 'Module: graphify/google_workspace.py'
type: catalog
provenance: extracted
module: graphify/google_workspace.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `graphify.google_workspace`/
symbols:
  convert_google_workspace_file: convert_google_workspace_file().
  read_google_shortcut: read_google_shortcut().
  _with_frontmatter: _with_frontmatter().
  _run_gws_export: _run_gws_export().
  GOOGLE_WORKSPACE_EXTENSIONS: GOOGLE_WORKSPACE_EXTENSIONS.
  google_workspace_enabled: google_workspace_enabled().
  _safe_yaml_str: _safe_yaml_str().
  _extract_file_id_from_url: _extract_file_id_from_url().
  _extract_resource_key: _extract_resource_key().
  _sidecar_path: _sidecar_path().
---
# Module: [`graphify/google_workspace.py`](../../../../../raw/code/graphify/graphify/google_workspace.py)

## Functions
- `_extract_file_id_from_url(url: str)` — [`L35`](../../../../../raw/code/graphify/graphify/google_workspace.py#L35) — Extract a Drive file ID from common Google Docs/Drive URL shapes.
- `_extract_resource_key(url: str, data: dict[str, Any])` — [`L49`](../../../../../raw/code/graphify/graphify/google_workspace.py#L49)
- `_run_gws_export(file_id: str, mime_type: str, output: Path, resource_key: str | None = None)` — [`L94`](../../../../../raw/code/graphify/graphify/google_workspace.py#L94)
- `_safe_yaml_str(value: str)` — [`L31`](../../../../../raw/code/graphify/graphify/google_workspace.py#L31)
- `_sidecar_path(path: Path, out_dir: Path)` — [`L124`](../../../../../raw/code/graphify/graphify/google_workspace.py#L124)
- `_with_frontmatter(path: Path, shortcut: dict[str, str | None], body: str, exported_mime_type: str)` — [`L129`](../../../../../raw/code/graphify/graphify/google_workspace.py#L129)
- `convert_google_workspace_file(path: Path, out_dir: Path, *, xlsx_to_markdown: Callable[[Path], str] | None = None)` — [`L150`](../../../../../raw/code/graphify/graphify/google_workspace.py#L150) — Export a Google Workspace shortcut to a Markdown sidecar. — documented in [graphify-detect](../../concepts/graphify-detect.md)
- `google_workspace_enabled(value: str | None = None)` — [`L25`](../../../../../raw/code/graphify/graphify/google_workspace.py#L25) — Return True when Google Workspace shortcut export is enabled.
- `read_google_shortcut(path: Path)` — [`L63`](../../../../../raw/code/graphify/graphify/google_workspace.py#L63) — Read a .gdoc/.gsheet/.gslides shortcut and return export metadata.

## Module values
- `GOOGLE_WORKSPACE_EXTENSIONS` — [`L22`](../../../../../raw/code/graphify/graphify/google_workspace.py#L22)

