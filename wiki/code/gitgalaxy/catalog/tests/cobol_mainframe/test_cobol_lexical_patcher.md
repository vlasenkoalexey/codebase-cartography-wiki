---
title: 'Module: tests/cobol_mainframe/test_cobol_lexical_patcher.py'
type: catalog
provenance: extracted
module: tests/cobol_mainframe/test_cobol_lexical_patcher.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `tests.cobol_mainframe.test_cobol_lexical_patcher`/test_
symbols:
  test_detect_cobol_dialect: detect_cobol_dialect().
  test_patch_cobol85_modernization: patch_cobol85_modernization().
  test_patch_cobol74_strict_mode: patch_cobol74_strict_mode().
  test_fast_exit_clean_file: fast_exit_clean_file().
---
# Module: [`tests/cobol_mainframe/test_cobol_lexical_patcher.py`](../../../../../../raw/code/gitgalaxy/tests/cobol_mainframe/test_cobol_lexical_patcher.py)

## Functions
- `test_detect_cobol_dialect()` — [`L9`](../../../../../../raw/code/gitgalaxy/tests/cobol_mainframe/test_cobol_lexical_patcher.py#L9) — Proves the sensor correctly dates the compiler era by scanning for
- `test_fast_exit_clean_file(tmp_path)` — [`L84`](../../../../../../raw/code/gitgalaxy/tests/cobol_mainframe/test_cobol_lexical_patcher.py#L84) — Proves that files without the lexical trap are instantly skipped,
- `test_patch_cobol74_strict_mode(tmp_path)` — [`L58`](../../../../../../raw/code/gitgalaxy/tests/cobol_mainframe/test_cobol_lexical_patcher.py#L58) — Proves that in a legacy environment, the engine normalizes the casing and
- `test_patch_cobol85_modernization(tmp_path)` — [`L35`](../../../../../../raw/code/gitgalaxy/tests/cobol_mainframe/test_cobol_lexical_patcher.py#L35) — Proves that in a modern environment, the dangerous NEXT SENTENCE trap

