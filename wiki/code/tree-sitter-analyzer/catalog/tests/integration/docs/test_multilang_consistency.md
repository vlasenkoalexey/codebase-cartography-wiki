---
title: 'Module: tests/integration/docs/test_multilang_consistency.py'
type: catalog
provenance: extracted
module: tests/integration/docs/test_multilang_consistency.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.docs.test_multilang_consistency`/
symbols:
  TestMultiLanguageConsistency.test_section_emojis_match: TestMultiLanguageConsistency#test_section_emojis_match().
  README_PATH: README_PATH.
  README_JA_PATH: README_JA_PATH.
  README_ZH_PATH: README_ZH_PATH.
  TestMultiLanguageConsistency.test_japanese_readme_section_count: TestMultiLanguageConsistency#test_japanese_readme_section_count().
  TestMultiLanguageConsistency.test_chinese_readme_section_count: TestMultiLanguageConsistency#test_chinese_readme_section_count().
  TestMultiLanguageConsistency.test_language_switcher_present: TestMultiLanguageConsistency#test_language_switcher_present().
  TestMultiLanguageConsistency.test_all_readmes_under_500_lines: TestMultiLanguageConsistency#test_all_readmes_under_500_lines().
  get_section_headers: get_section_headers().
  PROJECT_ROOT: PROJECT_ROOT.
  TestMultiLanguageConsistency.test_japanese_readme_exists: TestMultiLanguageConsistency#test_japanese_readme_exists().
  TestMultiLanguageConsistency.test_chinese_readme_exists: TestMultiLanguageConsistency#test_chinese_readme_exists().
  TestMultiLanguageConsistency: TestMultiLanguageConsistency#
---
# Module: [`tests/integration/docs/test_multilang_consistency.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/docs/test_multilang_consistency.py)

## Classes
### `TestMultiLanguageConsistency`
- def: [`tests/integration/docs/test_multilang_consistency.py:44`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/docs/test_multilang_consistency.py#L44)
- doc: Tests for multi-language README structure consistency.
- signature: `class TestMultiLanguageConsistency:`
- members:
  - `test_all_readmes_under_500_lines(self)` — [`L117`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/docs/test_multilang_consistency.py#L117) — All README versions should be under 500 lines.
  - `test_chinese_readme_exists(self)` — [`L54`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/docs/test_multilang_consistency.py#L54) — README_zh.md should exist.
  - `test_chinese_readme_section_count(self)` — [`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/docs/test_multilang_consistency.py#L68) — README_zh.md should have same number of sections as README.md.
  - `test_japanese_readme_exists(self)` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/docs/test_multilang_consistency.py#L50) — README_ja.md should exist.
  - `test_japanese_readme_section_count(self)` — [`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/docs/test_multilang_consistency.py#L58) — README_ja.md should have same number of sections as README.md.
  - `test_language_switcher_present(self)` — [`L97`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/docs/test_multilang_consistency.py#L97) — All READMEs should have language switcher links.
  - `test_section_emojis_match(self)` — [`L78`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/docs/test_multilang_consistency.py#L78) — Section emojis should match across all README versions.
- uses (calls/refs, reference-scoped): (4 test-only callers)

## Functions
- `get_section_headers(readme_path: Path)` — [`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/docs/test_multilang_consistency.py#L17) — Extract section headers from README.

## Module values
- `PROJECT_ROOT` — [`L11`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/docs/test_multilang_consistency.py#L11)
- `README_JA_PATH` — [`L13`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/docs/test_multilang_consistency.py#L13)
- `README_PATH` — [`L12`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/docs/test_multilang_consistency.py#L12)
- `README_ZH_PATH` — [`L14`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/docs/test_multilang_consistency.py#L14)

