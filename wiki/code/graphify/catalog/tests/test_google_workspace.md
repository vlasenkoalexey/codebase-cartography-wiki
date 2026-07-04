---
title: 'Module: tests/test_google_workspace.py'
type: catalog
provenance: extracted
module: tests/test_google_workspace.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_google_workspace`/test_
symbols:
  test_convert_gdoc_to_markdown_sidecar: convert_gdoc_to_markdown_sidecar().
  test_convert_gsheet_uses_xlsx_markdown_callback: convert_gsheet_uses_xlsx_markdown_callback().
  test_run_gws_export_uses_output_directory_as_cwd: run_gws_export_uses_output_directory_as_cwd().
  test_run_gws_export_does_not_send_resource_key_as_query_param: run_gws_export_does_not_send_resource_key_as_query_param().
  test_run_gws_export_uses_output_directory_as_cwd.fake_run: run_gws_export_uses_output_directory_as_cwd().fake_run().
  test_run_gws_export_does_not_send_resource_key_as_query_param.fake_run: run_gws_export_does_not_send_resource_key_as_query_param().fake_run().
  test_read_google_shortcut_doc_id: read_google_shortcut_doc_id().
  test_read_google_shortcut_extracts_id_from_url: read_google_shortcut_extracts_id_from_url().
  test_google_workspace_enabled_env: google_workspace_enabled_env().
  test_convert_gdoc_to_markdown_sidecar.fake_export: convert_gdoc_to_markdown_sidecar().fake_export().
  test_convert_gsheet_uses_xlsx_markdown_callback.fake_export: convert_gsheet_uses_xlsx_markdown_callback().fake_export().
  test_run_gws_export_uses_output_directory_as_cwd.Result: run_gws_export_uses_output_directory_as_cwd().Result#
  test_run_gws_export_does_not_send_resource_key_as_query_param.Result: run_gws_export_does_not_send_resource_key_as_query_param().Result#
  test_run_gws_export_uses_output_directory_as_cwd.Result.returncode: run_gws_export_uses_output_directory_as_cwd().Result#returncode.
  test_run_gws_export_uses_output_directory_as_cwd.Result.stdout: run_gws_export_uses_output_directory_as_cwd().Result#stdout.
  test_run_gws_export_uses_output_directory_as_cwd.Result.stderr: run_gws_export_uses_output_directory_as_cwd().Result#stderr.
  test_run_gws_export_does_not_send_resource_key_as_query_param.Result.returncode: run_gws_export_does_not_send_resource_key_as_query_param().Result#returncode.
  test_run_gws_export_does_not_send_resource_key_as_query_param.Result.stdout: run_gws_export_does_not_send_resource_key_as_query_param().Result#stdout.
  test_run_gws_export_does_not_send_resource_key_as_query_param.Result.stderr: run_gws_export_does_not_send_resource_key_as_query_param().Result#stderr.
---
# Module: [`tests/test_google_workspace.py`](../../../../../raw/code/graphify/tests/test_google_workspace.py)

## Classes
### `Result`
- def: [`tests/test_google_workspace.py:106`](../../../../../raw/code/graphify/tests/test_google_workspace.py#L106)
- signature: `class Result:`
- members:
  - `returncode` — [`L82`](../../../../../raw/code/graphify/tests/test_google_workspace.py#L82)
  - `returncode` — [`L107`](../../../../../raw/code/graphify/tests/test_google_workspace.py#L107)
  - `stderr` — [`L84`](../../../../../raw/code/graphify/tests/test_google_workspace.py#L84)
  - `stderr` — [`L109`](../../../../../raw/code/graphify/tests/test_google_workspace.py#L109)
  - `stdout` — [`L83`](../../../../../raw/code/graphify/tests/test_google_workspace.py#L83)
  - `stdout` — [`L108`](../../../../../raw/code/graphify/tests/test_google_workspace.py#L108)
- used by: (1 test-only callers)

## Functions
- `fake_export(file_id, mime_type, output, resource_key=None)` — [`L40`](../../../../../raw/code/graphify/tests/test_google_workspace.py#L40)
- `fake_export(file_id, mime_type, output, resource_key=None)` — [`L60`](../../../../../raw/code/graphify/tests/test_google_workspace.py#L60)
- `fake_run(cmd, **kwargs)` — [`L86`](../../../../../raw/code/graphify/tests/test_google_workspace.py#L86)
- `fake_run(cmd, **kwargs)` — [`L111`](../../../../../raw/code/graphify/tests/test_google_workspace.py#L111)
- `test_convert_gdoc_to_markdown_sidecar(tmp_path, monkeypatch)` — [`L33`](../../../../../raw/code/graphify/tests/test_google_workspace.py#L33)
- `test_convert_gsheet_uses_xlsx_markdown_callback(tmp_path, monkeypatch)` — [`L56`](../../../../../raw/code/graphify/tests/test_google_workspace.py#L56)
- `test_google_workspace_enabled_env(monkeypatch)` — [`L124`](../../../../../raw/code/graphify/tests/test_google_workspace.py#L124)
- `test_read_google_shortcut_doc_id(tmp_path)` — [`L7`](../../../../../raw/code/graphify/tests/test_google_workspace.py#L7)
- `test_read_google_shortcut_extracts_id_from_url(tmp_path)` — [`L20`](../../../../../raw/code/graphify/tests/test_google_workspace.py#L20)
- `test_run_gws_export_does_not_send_resource_key_as_query_param(tmp_path, monkeypatch)` — [`L102`](../../../../../raw/code/graphify/tests/test_google_workspace.py#L102)
- `test_run_gws_export_uses_output_directory_as_cwd(tmp_path, monkeypatch)` — [`L77`](../../../../../raw/code/graphify/tests/test_google_workspace.py#L77)

