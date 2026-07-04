---
title: 'Module: tests/test_image_vision.py'
type: catalog
provenance: extracted
module: tests/test_image_vision.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_image_vision`/
symbols:
  test_build_image_refs_sets_rel_media_and_bytes: test_build_image_refs_sets_rel_media_and_bytes().
  test_claude_cli_adds_dir_and_read_instruction: test_claude_cli_adds_dir_and_read_instruction().
  _make_corpus: _make_corpus().
  test_claude_cli_passes_oversized_image_by_path: test_claude_cli_passes_oversized_image_by_path().
  test_builders_fall_back_to_string_without_pixels: test_builders_fall_back_to_string_without_pixels().
  test_call_bedrock_sends_raw_image_bytes: test_call_bedrock_sends_raw_image_bytes().
  test_path_backend_skips_byte_read_and_size_cap: test_path_backend_skips_byte_read_and_size_cap().
  test_chunk_packing_caps_images_per_chunk: test_chunk_packing_caps_images_per_chunk().
  test_anthropic_content_has_base64_block: test_anthropic_content_has_base64_block().
  test_openai_content_has_data_uri: test_openai_content_has_data_uri().
  test_bedrock_content_uses_raw_bytes: test_bedrock_content_uses_raw_bytes().
  test_call_claude_sends_image_block: test_call_claude_sends_image_block().
  test_call_openai_compat_sends_image_url: test_call_openai_compat_sends_image_url().
  test_build_image_refs_drops_oversized: test_build_image_refs_drops_oversized().
  test_image_token_estimate_is_flat: test_image_token_estimate_is_flat().
  test_extract_files_direct_gates_pixels_by_capability: test_extract_files_direct_gates_pixels_by_capability().
  _PNG_BYTES: _PNG_BYTES.
  _fake_openai: _fake_openai().
  _NODE_JSON: _NODE_JSON.
  test_partition_splits_raster_from_text: test_partition_splits_raster_from_text().
  test_build_image_refs_skips_out_of_root_symlink: test_build_image_refs_skips_out_of_root_symlink().
  test_no_images_is_byte_identical: test_no_images_is_byte_identical().
  test_call_openai_compat_text_only_without_images: test_call_openai_compat_text_only_without_images().
  _fake_anthropic: _fake_anthropic().
  _fake_boto3: _fake_boto3().
  test_pdf_routed_through_pypdf_not_readtext: test_pdf_routed_through_pypdf_not_readtext().
  test_pdf_is_not_treated_as_vision_image: test_pdf_is_not_treated_as_vision_image().
  test_non_pdf_still_read_as_plain_text: test_non_pdf_still_read_as_plain_text().
  test_read_files_skips_out_of_root_symlink: test_read_files_skips_out_of_root_symlink().
  test_capability_flags: test_capability_flags().
  _fake_anthropic._Messages.create: _fake_anthropic()._Messages#create().
  _fake_openai._Completions.create: _fake_openai()._Completions#create().
  _fake_boto3._Client.converse: _fake_boto3()._Client#converse().
  test_claude_cli_passes_oversized_image_by_path.fake_run: test_claude_cli_passes_oversized_image_by_path().fake_run().
  _fake_anthropic._Messages: _fake_anthropic()._Messages#
  _fake_openai._Completions: _fake_openai()._Completions#
  _fake_boto3._Client: _fake_boto3()._Client#
  test_claude_cli_adds_dir_and_read_instruction.fake_run: test_claude_cli_adds_dir_and_read_instruction().fake_run().
---
# Module: [`tests/test_image_vision.py`](../../../../../raw/code/graphify/tests/test_image_vision.py)

## Classes
### `_Client`
- def: [`tests/test_image_vision.py:274`](../../../../../raw/code/graphify/tests/test_image_vision.py#L274)
- signature: `class _Client:`
- members:
  - `converse(self, **kw)` — [`L275`](../../../../../raw/code/graphify/tests/test_image_vision.py#L275)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `_Completions`
- def: [`tests/test_image_vision.py:260`](../../../../../raw/code/graphify/tests/test_image_vision.py#L260)
- signature: `class _Completions:`
- members:
  - `create(self, **kw)` — [`L261`](../../../../../raw/code/graphify/tests/test_image_vision.py#L261)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `_Messages`
- def: [`tests/test_image_vision.py:246`](../../../../../raw/code/graphify/tests/test_image_vision.py#L246)
- signature: `class _Messages:`
- members:
  - `create(self, **kw)` — [`L247`](../../../../../raw/code/graphify/tests/test_image_vision.py#L247)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

## Functions
- `_fake_anthropic(monkeypatch, captured)` — [`L245`](../../../../../raw/code/graphify/tests/test_image_vision.py#L245)
- `_fake_boto3(monkeypatch, captured)` — [`L273`](../../../../../raw/code/graphify/tests/test_image_vision.py#L273)
- `_fake_openai(monkeypatch, captured)` — [`L259`](../../../../../raw/code/graphify/tests/test_image_vision.py#L259)
- `_make_corpus(tmp_path)` — [`L33`](../../../../../raw/code/graphify/tests/test_image_vision.py#L33) — A corpus with one raster image, one svg (text), and one markdown doc.
- `fake_run(args, **kw)` — [`L152`](../../../../../raw/code/graphify/tests/test_image_vision.py#L152)
- `fake_run(args, **kw)` — [`L343`](../../../../../raw/code/graphify/tests/test_image_vision.py#L343)
- `test_anthropic_content_has_base64_block(tmp_path)` — [`L196`](../../../../../raw/code/graphify/tests/test_image_vision.py#L196)
- `test_bedrock_content_uses_raw_bytes(tmp_path)` — [`L217`](../../../../../raw/code/graphify/tests/test_image_vision.py#L217)
- `test_build_image_refs_drops_oversized(tmp_path, monkeypatch)` — [`L122`](../../../../../raw/code/graphify/tests/test_image_vision.py#L122)
- `test_build_image_refs_sets_rel_media_and_bytes(tmp_path)` — [`L97`](../../../../../raw/code/graphify/tests/test_image_vision.py#L97)
- `test_build_image_refs_skips_out_of_root_symlink(tmp_path)` — [`L107`](../../../../../raw/code/graphify/tests/test_image_vision.py#L107)
- `test_builders_fall_back_to_string_without_pixels(tmp_path)` — [`L227`](../../../../../raw/code/graphify/tests/test_image_vision.py#L227)
- `test_call_bedrock_sends_raw_image_bytes(tmp_path, monkeypatch)` — [`L322`](../../../../../raw/code/graphify/tests/test_image_vision.py#L322)
- `test_call_claude_sends_image_block(tmp_path, monkeypatch)` — [`L295`](../../../../../raw/code/graphify/tests/test_image_vision.py#L295)
- `test_call_openai_compat_sends_image_url(tmp_path, monkeypatch)` — [`L305`](../../../../../raw/code/graphify/tests/test_image_vision.py#L305)
- `test_call_openai_compat_text_only_without_images(monkeypatch)` — [`L315`](../../../../../raw/code/graphify/tests/test_image_vision.py#L315)
- `test_capability_flags(monkeypatch)` — [`L163`](../../../../../raw/code/graphify/tests/test_image_vision.py#L163)
- `test_chunk_packing_caps_images_per_chunk(tmp_path)` — [`L179`](../../../../../raw/code/graphify/tests/test_image_vision.py#L179)
- `test_claude_cli_adds_dir_and_read_instruction(tmp_path, monkeypatch)` — [`L337`](../../../../../raw/code/graphify/tests/test_image_vision.py#L337)
- `test_claude_cli_passes_oversized_image_by_path(tmp_path, monkeypatch)` — [`L142`](../../../../../raw/code/graphify/tests/test_image_vision.py#L142) — documented in [graphify-llm](../../concepts/graphify-llm.md)
- `test_extract_files_direct_gates_pixels_by_capability(tmp_path, monkeypatch)` — [`L361`](../../../../../raw/code/graphify/tests/test_image_vision.py#L361)
- `test_image_token_estimate_is_flat(tmp_path)` — [`L174`](../../../../../raw/code/graphify/tests/test_image_vision.py#L174)
- `test_no_images_is_byte_identical(tmp_path)` — [`L237`](../../../../../raw/code/graphify/tests/test_image_vision.py#L237)
- `test_non_pdf_still_read_as_plain_text(tmp_path)` — [`L67`](../../../../../raw/code/graphify/tests/test_image_vision.py#L67)
- `test_openai_content_has_data_uri(tmp_path)` — [`L208`](../../../../../raw/code/graphify/tests/test_image_vision.py#L208)
- `test_partition_splits_raster_from_text(tmp_path)` — [`L89`](../../../../../raw/code/graphify/tests/test_image_vision.py#L89)
- `test_path_backend_skips_byte_read_and_size_cap(tmp_path, monkeypatch)` — [`L131`](../../../../../raw/code/graphify/tests/test_image_vision.py#L131)
- `test_pdf_is_not_treated_as_vision_image(tmp_path)` — [`L60`](../../../../../raw/code/graphify/tests/test_image_vision.py#L60)
- `test_pdf_routed_through_pypdf_not_readtext(tmp_path, monkeypatch)` — [`L47`](../../../../../raw/code/graphify/tests/test_image_vision.py#L47)
- `test_read_files_skips_out_of_root_symlink(tmp_path)` — [`L73`](../../../../../raw/code/graphify/tests/test_image_vision.py#L73)

## Module values
- `_NODE_JSON` — [`L26`](../../../../../raw/code/graphify/tests/test_image_vision.py#L26)
- `_PNG_BYTES` — [`L25`](../../../../../raw/code/graphify/tests/test_image_vision.py#L25)

