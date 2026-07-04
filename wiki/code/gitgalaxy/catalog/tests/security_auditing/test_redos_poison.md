---
title: 'Module: tests/security_auditing/test_redos_poison.py'
type: catalog
provenance: extracted
module: tests/security_auditing/test_redos_poison.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `tests.security_auditing.test_redos_poison`/
symbols:
  TestProductionRegexSecurity.test_production_regex_redos_immunity: TestProductionRegexSecurity#test_production_regex_redos_immunity().
  _fuzz_chunk: _fuzz_chunk().
  EVIL_STRINGS: EVIL_STRINGS.
  TestProductionRegexSecurity: TestProductionRegexSecurity#
---
# Module: [`tests/security_auditing/test_redos_poison.py`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_redos_poison.py)

## Classes
### `TestProductionRegexSecurity`
- def: [`tests/security_auditing/test_redos_poison.py:49`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_redos_poison.py#L49)
- signature: `class TestProductionRegexSecurity:`
- members:
  - `test_production_regex_redos_immunity(self)` — [`L50`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_redos_poison.py#L50) — Extracts every single regex from the production standards and blasts them — documented in [gitgalaxy-standards-language_standards](../../../concepts/gitgalaxy-standards-language_standards.md)
- uses (calls/refs, reference-scoped): [`LANGUAGE_DEFINITIONS`](../../gitgalaxy/standards/language_standards.md#LANGUAGE_DEFINITIONS)  (1 test-only)

## Functions
- `_fuzz_chunk(tasks_chunk, status_queue)` — [`L33`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_redos_poison.py#L33) — Worker process. Evaluates a massive chunk of regexes instantly.

## Module values
- `EVIL_STRINGS` — [`L14`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_redos_poison.py#L14)

