---
title: 'Module: tests/extraction/test_class_extraction_strict.py'
type: catalog
provenance: extracted
module: tests/extraction/test_class_extraction_strict.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `tests.extraction.test_class_extraction_strict`/
symbols:
  CLASS_EXTRACTION_CASES: CLASS_EXTRACTION_CASES.
  TestClassExtraction.test_positive_class_extraction: TestClassExtraction#test_positive_class_extraction().
  TestClassExtraction.test_negative_class_extraction: TestClassExtraction#test_negative_class_extraction().
  TestClassExtraction.test_pathological_class_extraction: TestClassExtraction#test_pathological_class_extraction().
  TestClassExtraction: TestClassExtraction#
---
# Module: [`tests/extraction/test_class_extraction_strict.py`](../../../../../../raw/code/gitgalaxy/tests/extraction/test_class_extraction_strict.py)

## Classes
### `TestClassExtraction`
- def: [`tests/extraction/test_class_extraction_strict.py:284`](../../../../../../raw/code/gitgalaxy/tests/extraction/test_class_extraction_strict.py#L284)
- signature: `class TestClassExtraction:`
- members:
  - `test_negative_class_extraction(self, lang_id)` — [`L319`](../../../../../../raw/code/gitgalaxy/tests/extraction/test_class_extraction_strict.py#L319) — Proves that structural lookalikes (instantiations, function calls) — documented in [gitgalaxy-standards-language_standards](../../../concepts/gitgalaxy-standards-language_standards.md)
  - `test_pathological_class_extraction(self, lang_id)` — [`L339`](../../../../../../raw/code/gitgalaxy/tests/extraction/test_class_extraction_strict.py#L339) — Adversarial Engineering: Proves the regex can survive "Frankenstein" — documented in [gitgalaxy-standards-language_standards](../../../concepts/gitgalaxy-standards-language_standards.md)
  - `test_positive_class_extraction(self, lang_id)` — [`L286`](../../../../../../raw/code/gitgalaxy/tests/extraction/test_class_extraction_strict.py#L286) — Proves that valid class/entity signatures are caught, and the regex — documented in [gitgalaxy-standards-language_standards](../../../concepts/gitgalaxy-standards-language_standards.md)
- uses (calls/refs, reference-scoped): [`LANGUAGE_DEFINITIONS`](../../gitgalaxy/standards/language_standards.md#LANGUAGE_DEFINITIONS)  (1 test-only)

## Module values
- `CLASS_EXTRACTION_CASES` — [`L16`](../../../../../../raw/code/gitgalaxy/tests/extraction/test_class_extraction_strict.py#L16)

