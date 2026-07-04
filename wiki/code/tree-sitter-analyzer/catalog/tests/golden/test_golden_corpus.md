---
title: 'Module: tests/golden/test_golden_corpus.py'
type: catalog
provenance: extracted
module: tests/golden/test_golden_corpus.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.golden.test_golden_corpus`/
symbols:
  TestGoldenCorpus.test_golden_corpus: TestGoldenCorpus#test_golden_corpus().
  TestGoldenCorpus.count_nodes: TestGoldenCorpus#count_nodes().
  TestGoldenCorpus._get_corpus_path: TestGoldenCorpus#_get_corpus_path().
  TestGoldenCorpus._extract_node_types_from_file: TestGoldenCorpus#_extract_node_types_from_file().
  TestGoldenCorpus.LANGUAGE_EXTENSIONS: TestGoldenCorpus#LANGUAGE_EXTENSIONS.
  TestGoldenCorpus._get_expected_path: TestGoldenCorpus#_get_expected_path().
  TestGoldenCorpus._load_expected_json: TestGoldenCorpus#_load_expected_json().
  TestGoldenCorpus._format_diff_critical_only: TestGoldenCorpus#_format_diff_critical_only().
  pytestmark: pytestmark.
  TestGoldenCorpus: TestGoldenCorpus#
  TestGoldenCorpus.golden_dir: TestGoldenCorpus#golden_dir().
---
# Module: [`tests/golden/test_golden_corpus.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/test_golden_corpus.py)

## Classes
### `TestGoldenCorpus`
- def: [`tests/golden/test_golden_corpus.py:44`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/test_golden_corpus.py#L44)
- doc: Golden corpus tests for all supported languages
- signature: `class TestGoldenCorpus:`
- members:
  - `_extract_node_types_from_file(self, corpus_path: Path, language: str)` — [`L115`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/test_golden_corpus.py#L115) — Extract node type counts from corpus file using tree-sitter directly.
  - `_format_diff_critical_only(self, expected: dict[str, int], actual: dict[str, int], language: str, mismatches: list[tuple[str, int, int]])` — [`L201`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/test_golden_corpus.py#L201) — Format a clear diff between expected and actual node counts for critical types only.
  - `_get_corpus_path(self, golden_dir: Path, language: str)` — [`L76`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/test_golden_corpus.py#L76) — Get the corpus file path for a language
  - `_get_expected_path(self, golden_dir: Path, language: str)` — [`L81`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/test_golden_corpus.py#L81) — Get the expected.json file path for a language
  - `_load_expected_json(self, expected_path: Path)` — [`L85`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/test_golden_corpus.py#L85) — Load and validate expected.json file.
  - `count_nodes(node: tree_sitter.Node)` — [`L190`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/test_golden_corpus.py#L190)
  - `golden_dir(self)` — [`L72`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/test_golden_corpus.py#L72) — Get the golden directory path
  - `test_golden_corpus(self, language: str, golden_dir: Path)` — [`L282`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/test_golden_corpus.py#L282) — Test golden corpus for a specific language.
  - `LANGUAGE_EXTENSIONS` — [`L48`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/test_golden_corpus.py#L48)
- uses (calls/refs, reference-scoped): [`analyze_file`](../../tree_sitter_analyzer/api.md#analyze_file)

## Module values
- `pytestmark` — [`L41`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/test_golden_corpus.py#L41)

