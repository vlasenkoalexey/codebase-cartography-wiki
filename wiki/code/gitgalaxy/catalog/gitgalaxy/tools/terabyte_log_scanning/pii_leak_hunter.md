---
title: 'Module: gitgalaxy/tools/terabyte_log_scanning/pii_leak_hunter.py'
type: catalog
provenance: extracted
module: gitgalaxy/tools/terabyte_log_scanning/pii_leak_hunter.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `gitgalaxy.tools.terabyte_log_scanning.pii_leak_hunter`/
symbols:
  main: main().
  mask_pii: mask_pii().
  PII_PATTERNS: PII_PATTERNS.
  draw_ascii_histogram: draw_ascii_histogram().
---
# Module: [`gitgalaxy/tools/terabyte_log_scanning/pii_leak_hunter.py`](../../../../../../../raw/code/gitgalaxy/gitgalaxy/tools/terabyte_log_scanning/pii_leak_hunter.py)

## Functions
- `draw_ascii_histogram(time_buckets: dict, keyword: str)` — [`L54`](../../../../../../../raw/code/gitgalaxy/gitgalaxy/tools/terabyte_log_scanning/pii_leak_hunter.py#L54) — Draws a dynamically scaled ASCII histogram to visualize exposure frequency over time.
- `main()` — [`L81`](../../../../../../../raw/code/gitgalaxy/gitgalaxy/tools/terabyte_log_scanning/pii_leak_hunter.py#L81) — documented in [gitgalaxy-licensing](../../../../concepts/gitgalaxy-licensing.md)
- `mask_pii(text: str)` — [`L27`](../../../../../../../raw/code/gitgalaxy/gitgalaxy/tools/terabyte_log_scanning/pii_leak_hunter.py#L27) — Masks out the middle of sensitive data so the evidence log is safe for retention.

## Module values
- `PII_PATTERNS` — [`L19`](../../../../../../../raw/code/gitgalaxy/gitgalaxy/tools/terabyte_log_scanning/pii_leak_hunter.py#L19)

