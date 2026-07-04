---
title: 'Module: tests/core_engine/test_prism.py'
type: catalog
provenance: extracted
module: tests/core_engine/test_prism.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `tests.core_engine.test_prism`/
symbols:
  prism_engine: prism_engine().
  test_prism_regex_matrix_calibration_edge_cases: test_prism_regex_matrix_calibration_edge_cases().
  MOCK_COMMENT_DEFS: MOCK_COMMENT_DEFS.
  MOCK_LANG_DEFS: MOCK_LANG_DEFS.
  test_prism_prose_bypass: test_prism_prose_bypass().
  test_prism_metadata_guard: test_prism_metadata_guard().
  test_prism_string_shield_protection: test_prism_string_shield_protection().
  test_prism_nested_block_peeling: test_prism_nested_block_peeling().
  test_prism_positional_anchors: test_prism_positional_anchors().
  test_prism_python_docstring_extraction: test_prism_python_docstring_extraction().
  test_prism_format_and_xml_bypass: test_prism_format_and_xml_bypass().
  test_prism_php_string_extraction: test_prism_php_string_extraction().
  test_prism_embedded_partitioning_and_escaping: test_prism_embedded_partitioning_and_escaping().
---
# Module: [`tests/core_engine/test_prism.py`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_prism.py)

## Functions
- `prism_engine()` — [`L35`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_prism.py#L35) — Initializes the Prism with a controlled, deterministic regex matrix.
- `test_prism_embedded_partitioning_and_escaping(prism_engine)` — [`L211`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_prism.py#L211) — Proves the Embedded Triggers accurately isolate languages.
- `test_prism_format_and_xml_bypass(prism_engine)` — [`L167`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_prism.py#L167) — Proves unknown and unparsable languages skip the scanner entirely.
- `test_prism_metadata_guard(prism_engine)` — [`L67`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_prism.py#L67) — Proves that Shebangs bypass the comment stripper and stay in the logic stream.
- `test_prism_nested_block_peeling(prism_engine)` — [`L102`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_prism.py#L102) — Proves the iterative peel loop correctly extracts recursive block comments.
- `test_prism_php_string_extraction(prism_engine)` — [`L194`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_prism.py#L194) — Proves PHP Heredoc and large strings are stripped to the documentation stream.
- `test_prism_positional_anchors(prism_engine)` — [`L126`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_prism.py#L126) — Proves legacy column-anchored and inline comments are handled correctly.
- `test_prism_prose_bypass(prism_engine)` — [`L56`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_prism.py#L56) — Proves that Markdown and XML are routed entirely to the Documentation stream.
- `test_prism_python_docstring_extraction(prism_engine)` — [`L149`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_prism.py#L149) — Proves multi-line string literals acting as docstrings are extracted.
- `test_prism_regex_matrix_calibration_edge_cases()` — [`L243`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_prism.py#L243) — Proves all complex and fallback regex families compile correctly.
- `test_prism_string_shield_protection(prism_engine)` — [`L81`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_prism.py#L81) — Proves that string literals containing comment delimiters do not trigger the stripper.

## Module values
- `MOCK_COMMENT_DEFS` — [`L14`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_prism.py#L14)
- `MOCK_LANG_DEFS` — [`L23`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_prism.py#L23)

