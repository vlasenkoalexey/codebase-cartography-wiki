---
title: 'Module: tests/unit/test_doc_sync.py'
type: catalog
provenance: extracted
module: tests/unit/test_doc_sync.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_doc_sync`/Test
symbols:
  TestValidateFileRefs.test_missing_file_reported: ValidateFileRefs#test_missing_file_reported().
  TestExtractFileRefs.test_backtick_py_file: ExtractFileRefs#test_backtick_py_file().
  TestValidateFileRefs.test_multiple_some_stale: ValidateFileRefs#test_multiple_some_stale().
  TestExtractFileRefs.test_backtick_md_file: ExtractFileRefs#test_backtick_md_file().
  TestExtractFileRefs.test_markdown_link_target: ExtractFileRefs#test_markdown_link_target().
  TestExtractFileRefs.test_multiple_refs_on_same_line: ExtractFileRefs#test_multiple_refs_on_same_line().
  TestExtractFileRefs.test_line_numbers_are_accurate: ExtractFileRefs#test_line_numbers_are_accurate().
  TestExtractFileRefs.test_shell_script_ref: ExtractFileRefs#test_shell_script_ref().
  TestValidateFileRefs.test_existing_file_no_stale: ValidateFileRefs#test_existing_file_no_stale().
  TestExtractFileRefs.test_skips_glob_patterns: ExtractFileRefs#test_skips_glob_patterns().
  TestExtractFileRefs.test_skips_http_links: ExtractFileRefs#test_skips_http_links().
  TestExtractFileRefs.test_skips_anchor_links: ExtractFileRefs#test_skips_anchor_links().
  TestExtractFileRefs.test_skips_plain_words: ExtractFileRefs#test_skips_plain_words().
  TestExtractFileRefs.test_skips_code_blocks: ExtractFileRefs#test_skips_code_blocks().
  TestExtractFileRefs.test_path_without_extension_skipped: ExtractFileRefs#test_path_without_extension_skipped().
  TestExtractFileRefs.test_path_with_slash_and_no_ext_skipped: ExtractFileRefs#test_path_with_slash_and_no_ext_skipped().
  TestValidateFileRefs.test_empty_refs_returns_empty: ValidateFileRefs#test_empty_refs_returns_empty().
  TestRunDocSync.test_finds_stale_ref_in_doc: RunDocSync#test_finds_stale_ref_in_doc().
  TestRunDocSync.test_all_clean_returns_zero_stale: RunDocSync#test_all_clean_returns_zero_stale().
  TestRunDocSync.test_summary_fields_present: RunDocSync#test_summary_fields_present().
  TestRunDocSync.test_default_pattern_scans_docs_folder: RunDocSync#test_default_pattern_scans_docs_folder().
  TestRunDocSync.test_no_docs_folder_returns_success: RunDocSync#test_no_docs_folder_returns_success().
  TestRunDocSync.test_stale_ref_includes_doc_file_and_line: RunDocSync#test_stale_ref_includes_doc_file_and_line().
  TestExtractFileRefs: ExtractFileRefs#
  TestValidateFileRefs: ValidateFileRefs#
  TestRunDocSync: RunDocSync#
---
# Module: [`tests/unit/test_doc_sync.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_doc_sync.py)

## Classes
### `TestExtractFileRefs`
- def: [`tests/unit/test_doc_sync.py:17`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_doc_sync.py#L17)
- signature: `class TestExtractFileRefs:`
- members:
  - `test_backtick_md_file(self)` — [`L26`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_doc_sync.py#L26)
  - `test_backtick_py_file(self)` — [`L18`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_doc_sync.py#L18)
  - `test_line_numbers_are_accurate(self)` — [`L65`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_doc_sync.py#L65)
  - `test_markdown_link_target(self)` — [`L32`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_doc_sync.py#L32)
  - `test_multiple_refs_on_same_line(self)` — [`L58`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_doc_sync.py#L58)
  - `test_path_with_slash_and_no_ext_skipped(self)` — [`L93`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_doc_sync.py#L93)
  - `test_path_without_extension_skipped(self)` — [`L88`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_doc_sync.py#L88)
  - `test_shell_script_ref(self)` — [`L71`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_doc_sync.py#L71)
  - `test_skips_anchor_links(self)` — [`L48`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_doc_sync.py#L48)
  - `test_skips_code_blocks(self)` — [`L77`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_doc_sync.py#L77)
  - `test_skips_glob_patterns(self)` — [`L38`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_doc_sync.py#L38)
  - `test_skips_http_links(self)` — [`L43`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_doc_sync.py#L43)
  - `test_skips_plain_words(self)` — [`L53`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_doc_sync.py#L53)
- uses (calls/refs, reference-scoped): [`extract_file_refs`](../../tree_sitter_analyzer/doc_sync.md#extract_file_refs), [`path`](../../tree_sitter_analyzer/doc_sync.md#DocRef.path), [`line`](../../tree_sitter_analyzer/doc_sync.md#DocRef.line), [`doc_file`](../../tree_sitter_analyzer/doc_sync.md#DocRef.doc_file)

### `TestRunDocSync`
- def: [`tests/unit/test_doc_sync.py:139`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_doc_sync.py#L139)
- signature: `class TestRunDocSync:`
- members:
  - `test_all_clean_returns_zero_stale(self, tmp_path)` — [`L155`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_doc_sync.py#L155)
  - `test_default_pattern_scans_docs_folder(self, tmp_path)` — [`L181`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_doc_sync.py#L181)
  - `test_finds_stale_ref_in_doc(self, tmp_path)` — [`L140`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_doc_sync.py#L140)
  - `test_no_docs_folder_returns_success(self, tmp_path)` — [`L189`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_doc_sync.py#L189)
  - `test_stale_ref_includes_doc_file_and_line(self, tmp_path)` — [`L194`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_doc_sync.py#L194)
  - `test_summary_fields_present(self, tmp_path)` — [`L169`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_doc_sync.py#L169)
- uses (calls/refs, reference-scoped): [`run_doc_sync`](../../tree_sitter_analyzer/doc_sync.md#run_doc_sync)

### `TestValidateFileRefs`
- def: [`tests/unit/test_doc_sync.py:104`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_doc_sync.py#L104)
- signature: `class TestValidateFileRefs:`
- members:
  - `test_empty_refs_returns_empty(self, tmp_path)` — [`L130`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_doc_sync.py#L130)
  - `test_existing_file_no_stale(self, tmp_path)` — [`L105`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_doc_sync.py#L105)
  - `test_missing_file_reported(self, tmp_path)` — [`L112`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_doc_sync.py#L112)
  - `test_multiple_some_stale(self, tmp_path)` — [`L120`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_doc_sync.py#L120)
- uses (calls/refs, reference-scoped): [`validate_file_refs`](../../tree_sitter_analyzer/doc_sync.md#validate_file_refs), [`path`](../../tree_sitter_analyzer/doc_sync.md#DocRef.path), [`DocRef`](../../tree_sitter_analyzer/doc_sync.md#DocRef), [`ref`](../../tree_sitter_analyzer/doc_sync.md#StaleRef.ref), [`line`](../../tree_sitter_analyzer/doc_sync.md#DocRef.line), [`reason`](../../tree_sitter_analyzer/doc_sync.md#StaleRef.reason)

