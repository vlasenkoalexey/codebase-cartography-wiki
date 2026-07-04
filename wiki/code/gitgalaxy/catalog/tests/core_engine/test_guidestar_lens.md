---
title: 'Module: tests/core_engine/test_guidestar_lens.py'
type: catalog
provenance: extracted
module: tests/core_engine/test_guidestar_lens.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `tests.core_engine.test_guidestar_lens`/
symbols:
  guidestar: guidestar().
  MOCK_GUIDESTAR_CONFIG: MOCK_GUIDESTAR_CONFIG.
  test_guidestar_manifest_and_ai_detection: test_guidestar_manifest_and_ai_detection().
  test_guidestar_gitattributes_authority: test_guidestar_gitattributes_authority().
  test_guidestar_gitignore_evasion_tactics: test_guidestar_gitignore_evasion_tactics().
  test_guidestar_sector_bias: test_guidestar_sector_bias().
---
# Module: [`tests/core_engine/test_guidestar_lens.py`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_guidestar_lens.py)

## Functions
- `guidestar(tmp_path)` — [`L23`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_guidestar_lens.py#L23) — Initializes the GuideStar Lens with a mocked configuration.
- `test_guidestar_gitattributes_authority(guidestar, tmp_path)` — [`L81`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_guidestar_lens.py#L81) — Proves that .gitattributes pattern rules override normal logic with
- `test_guidestar_gitignore_evasion_tactics(guidestar, tmp_path)` — [`L104`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_guidestar_lens.py#L104) — Proves that force-including a compiled binary in .gitignore triggers
- `test_guidestar_manifest_and_ai_detection(guidestar, tmp_path)` — [`L42`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_guidestar_lens.py#L42) — Proves that package.json is parsed for entry points, and that AI
- `test_guidestar_sector_bias(guidestar, tmp_path)` — [`L126`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_guidestar_lens.py#L126) — Proves that files located in structurally important directories get a

## Module values
- `MOCK_GUIDESTAR_CONFIG` — [`L11`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_guidestar_lens.py#L11)

