---
title: 'Module: tests/test_ingest.py'
type: catalog
provenance: extracted
module: tests/test_ingest.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_ingest`/test_
symbols:
  test_file_created: file_created().
  test_filename_format: filename_format().
  test_frontmatter_question: frontmatter_question().
  test_frontmatter_type: frontmatter_type().
  test_source_nodes_included: source_nodes_included().
  test_source_nodes_capped_at_10: source_nodes_capped_at_10().
  test_memory_dir_created: memory_dir_created().
  test_answer_in_body: answer_in_body().
  test_outcome_in_frontmatter_and_body: outcome_in_frontmatter_and_body().
  test_correction_in_frontmatter_and_body: correction_in_frontmatter_and_body().
  test_no_outcome_means_no_outcome_section: no_outcome_means_no_outcome_section().
  test_invalid_outcome_rejected: invalid_outcome_rejected().
---
# Module: [`tests/test_ingest.py`](../../../../../raw/code/graphify/tests/test_ingest.py)

## Functions
- `test_answer_in_body(tmp_path)` — [`L63`](../../../../../raw/code/graphify/tests/test_ingest.py#L63)
- `test_correction_in_frontmatter_and_body(tmp_path)` — [`L80`](../../../../../raw/code/graphify/tests/test_ingest.py#L80)
- `test_file_created(tmp_path)` — [`L9`](../../../../../raw/code/graphify/tests/test_ingest.py#L9)
- `test_filename_format(tmp_path)` — [`L14`](../../../../../raw/code/graphify/tests/test_ingest.py#L14)
- `test_frontmatter_question(tmp_path)` — [`L21`](../../../../../raw/code/graphify/tests/test_ingest.py#L21)
- `test_frontmatter_type(tmp_path)` — [`L30`](../../../../../raw/code/graphify/tests/test_ingest.py#L30)
- `test_invalid_outcome_rejected(tmp_path)` — [`L98`](../../../../../raw/code/graphify/tests/test_ingest.py#L98)
- `test_memory_dir_created(tmp_path)` — [`L56`](../../../../../raw/code/graphify/tests/test_ingest.py#L56)
- `test_no_outcome_means_no_outcome_section(tmp_path)` — [`L90`](../../../../../raw/code/graphify/tests/test_ingest.py#L90) — Backward compatible: a result without an outcome looks exactly as before.
- `test_outcome_in_frontmatter_and_body(tmp_path)` — [`L70`](../../../../../raw/code/graphify/tests/test_ingest.py#L70) — An outcome signal is written to both frontmatter (for `reflect`) and an
- `test_source_nodes_capped_at_10(tmp_path)` — [`L46`](../../../../../raw/code/graphify/tests/test_ingest.py#L46)
- `test_source_nodes_included(tmp_path)` — [`L37`](../../../../../raw/code/graphify/tests/test_ingest.py#L37)

