---
title: 'Module: tests/extraction/test_dependency_extraction_strict.py'
type: catalog
provenance: extracted
module: tests/extraction/test_dependency_extraction_strict.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `tests.extraction.test_dependency_extraction_strict`/
symbols:
  DEPENDENCY_EXTRACTION_CASES: DEPENDENCY_EXTRACTION_CASES.
  TestDependencyExtraction.test_positive_dependency_extraction: TestDependencyExtraction#test_positive_dependency_extraction().
  TestDependencyExtraction.test_negative_dependency_extraction: TestDependencyExtraction#test_negative_dependency_extraction().
  TestDependencyExtraction.test_pathological_dependency_extraction: TestDependencyExtraction#test_pathological_dependency_extraction().
  TestDependencyExtraction: TestDependencyExtraction#
---
# Module: [`tests/extraction/test_dependency_extraction_strict.py`](../../../../../../raw/code/gitgalaxy/tests/extraction/test_dependency_extraction_strict.py)

## Classes
### `TestDependencyExtraction`
- def: [`tests/extraction/test_dependency_extraction_strict.py:375`](../../../../../../raw/code/gitgalaxy/tests/extraction/test_dependency_extraction_strict.py#L375)
- signature: `class TestDependencyExtraction:`
- members:
  - `test_negative_dependency_extraction(self, lang_id)` — [`L413`](../../../../../../raw/code/gitgalaxy/tests/extraction/test_dependency_extraction_strict.py#L413) — Proves that structural lookalikes (variable assignments, comments) — documented in [gitgalaxy-standards-language_standards](../../../concepts/gitgalaxy-standards-language_standards.md)
  - `test_pathological_dependency_extraction(self, lang_id)` — [`L433`](../../../../../../raw/code/gitgalaxy/tests/extraction/test_dependency_extraction_strict.py#L433) — Adversarial Engineering: Proves the regex can survive "Frankenstein" — documented in [gitgalaxy-standards-language_standards](../../../concepts/gitgalaxy-standards-language_standards.md)
  - `test_positive_dependency_extraction(self, lang_id)` — [`L377`](../../../../../../raw/code/gitgalaxy/tests/extraction/test_dependency_extraction_strict.py#L377) — Proves that valid import signatures are caught, and the regex — documented in [gitgalaxy-standards-language_standards](../../../concepts/gitgalaxy-standards-language_standards.md)
- uses (calls/refs, reference-scoped): [`LANGUAGE_DEFINITIONS`](../../gitgalaxy/standards/language_standards.md#LANGUAGE_DEFINITIONS)  (1 test-only)

## Module values
- `DEPENDENCY_EXTRACTION_CASES` — [`L16`](../../../../../../raw/code/gitgalaxy/tests/extraction/test_dependency_extraction_strict.py#L16)

