---
title: 'Module: tests/extraction/test_function_extraction_strict.py'
type: catalog
provenance: extracted
module: tests/extraction/test_function_extraction_strict.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `tests.extraction.test_function_extraction_strict`/
symbols:
  EXTRACTION_CASES: EXTRACTION_CASES.
  TestFunctionExtraction.test_positive_function_extraction: TestFunctionExtraction#test_positive_function_extraction().
  TestFunctionExtraction.test_negative_function_extraction: TestFunctionExtraction#test_negative_function_extraction().
  TestFunctionExtraction.test_pathological_function_extraction: TestFunctionExtraction#test_pathological_function_extraction().
  TestFunctionExtraction: TestFunctionExtraction#
---
# Module: [`tests/extraction/test_function_extraction_strict.py`](../../../../../../raw/code/gitgalaxy/tests/extraction/test_function_extraction_strict.py)

## Classes
### `TestFunctionExtraction`
- def: [`tests/extraction/test_function_extraction_strict.py:457`](../../../../../../raw/code/gitgalaxy/tests/extraction/test_function_extraction_strict.py#L457)
- signature: `class TestFunctionExtraction:`
- members:
  - `test_negative_function_extraction(self, lang_id)` — [`L497`](../../../../../../raw/code/gitgalaxy/tests/extraction/test_function_extraction_strict.py#L497) — Proves that structural lookalikes (classes, if-statements, macros, invocations, interfaces) — documented in [gitgalaxy-standards-language_standards](../../../concepts/gitgalaxy-standards-language_standards.md)
  - `test_pathological_function_extraction(self, lang_id)` — [`L517`](../../../../../../raw/code/gitgalaxy/tests/extraction/test_function_extraction_strict.py#L517) — Adversarial Engineering: Proves the regex can survive "Frankenstein" — documented in [gitgalaxy-standards-language_standards](../../../concepts/gitgalaxy-standards-language_standards.md)
  - `test_positive_function_extraction(self, lang_id)` — [`L459`](../../../../../../raw/code/gitgalaxy/tests/extraction/test_function_extraction_strict.py#L459) — Proves that valid function signatures are caught, and the regex — documented in [gitgalaxy-standards-language_standards](../../../concepts/gitgalaxy-standards-language_standards.md)
- uses (calls/refs, reference-scoped): [`LANGUAGE_DEFINITIONS`](../../gitgalaxy/standards/language_standards.md#LANGUAGE_DEFINITIONS)  (1 test-only)

## Module values
- `EXTRACTION_CASES` — [`L27`](../../../../../../raw/code/gitgalaxy/tests/extraction/test_function_extraction_strict.py#L27)

