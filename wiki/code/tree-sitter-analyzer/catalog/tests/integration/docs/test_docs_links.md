---
title: 'Module: tests/integration/docs/test_docs_links.py'
type: catalog
provenance: extracted
module: tests/integration/docs/test_docs_links.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.docs.test_docs_links`/
symbols:
  TestDocumentationLinksValidity.test_all_docs_links_are_valid: TestDocumentationLinksValidity#test_all_docs_links_are_valid().
  DOCS_DIR: DOCS_DIR.
  PROJECT_ROOT: PROJECT_ROOT.
  TestRequiredDocsFiles.test_required_docs_exist: TestRequiredDocsFiles#test_required_docs_exist().
  get_readme_content: get_readme_content().
  README_PATH: README_PATH.
  TestDocumentationLinksValidity.test_docs_directory_exists: TestDocumentationLinksValidity#test_docs_directory_exists().
  TestRequiredDocsFiles.test_docs_assets_directory_exists: TestRequiredDocsFiles#test_docs_assets_directory_exists().
  TestChangelogLink.test_changelog_exists: TestChangelogLink#test_changelog_exists().
  TestChangelogLink.test_readme_links_to_changelog: TestChangelogLink#test_readme_links_to_changelog().
  extract_docs_links: extract_docs_links().
  TestRequiredDocsFiles.REQUIRED_DOCS: TestRequiredDocsFiles#REQUIRED_DOCS.
  TestDocumentationLinksValidity: TestDocumentationLinksValidity#
  TestRequiredDocsFiles: TestRequiredDocsFiles#
  TestChangelogLink: TestChangelogLink#
---
# Module: [`tests/integration/docs/test_docs_links.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/docs/test_docs_links.py)

## Classes
### `TestChangelogLink`
- def: [`tests/integration/docs/test_docs_links.py:99`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/docs/test_docs_links.py#L99)
- doc: Tests for CHANGELOG.md link.
- signature: `class TestChangelogLink:`
- members:
  - `test_changelog_exists(self)` — [`L102`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/docs/test_docs_links.py#L102) — CHANGELOG.md should exist in project root.
  - `test_readme_links_to_changelog(self)` — [`L107`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/docs/test_docs_links.py#L107) — README should link to CHANGELOG.md.
- uses (calls/refs, reference-scoped): (2 test-only callers)

### `TestDocumentationLinksValidity`
- def: [`tests/integration/docs/test_docs_links.py:36`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/docs/test_docs_links.py#L36)
- doc: Tests for documentation links validity.
- signature: `class TestDocumentationLinksValidity:`
- members:
  - `test_all_docs_links_are_valid(self)` — [`L42`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/docs/test_docs_links.py#L42) — All links to docs/ directory should reference existing files.
  - `test_docs_directory_exists(self)` — [`L62`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/docs/test_docs_links.py#L62) — docs/ directory should exist.
- uses (calls/refs, reference-scoped): (4 test-only callers)

### `TestRequiredDocsFiles`
- def: [`tests/integration/docs/test_docs_links.py:68`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/docs/test_docs_links.py#L68)
- doc: Tests for required documentation files existence.
- signature: `class TestRequiredDocsFiles:`
- members:
  - `test_docs_assets_directory_exists(self)` — [`L93`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/docs/test_docs_links.py#L93) — docs/assets/ directory should exist for GIF and images.
  - `test_required_docs_exist(self)` — [`L81`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/docs/test_docs_links.py#L81) — All required documentation files should exist.
  - `REQUIRED_DOCS` — [`L71`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/docs/test_docs_links.py#L71)
- uses (calls/refs, reference-scoped): (2 test-only callers)

## Functions
- `extract_docs_links(content: str)` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/docs/test_docs_links.py#L21) — Extract all links to docs/ directory with line numbers.
- `get_readme_content()` — [`L16`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/docs/test_docs_links.py#L16) — Read README content.

## Module values
- `DOCS_DIR` — [`L13`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/docs/test_docs_links.py#L13)
- `PROJECT_ROOT` — [`L11`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/docs/test_docs_links.py#L11)
- `README_PATH` — [`L12`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/docs/test_docs_links.py#L12)

