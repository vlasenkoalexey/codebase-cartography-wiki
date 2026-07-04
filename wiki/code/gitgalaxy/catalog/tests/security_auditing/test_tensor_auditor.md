---
title: 'Module: tests/security_auditing/test_tensor_auditor.py'
type: catalog
provenance: extracted
module: tests/security_auditing/test_tensor_auditor.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `tests.security_auditing.test_tensor_auditor`/
symbols:
  scanner: scanner().
  test_tensor_scanner_safetensors_success: test_tensor_scanner_safetensors_success().
  test_tensor_scanner_gguf_success: test_tensor_scanner_gguf_success().
  test_tensor_scanner_gguf_bad_magic: test_tensor_scanner_gguf_bad_magic().
  test_tensor_scanner_safetensors_massive_header: test_tensor_scanner_safetensors_massive_header().
  test_tensor_scanner_param_formatting: test_tensor_scanner_param_formatting().
---
# Module: [`tests/security_auditing/test_tensor_auditor.py`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_tensor_auditor.py)

## Functions
- `scanner()` — [`L10`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_tensor_auditor.py#L10) — Initializes the Tensor Scanner.
- `test_tensor_scanner_gguf_bad_magic(scanner, tmp_path)` — [`L82`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_tensor_auditor.py#L82) — Proves the scanner safely rejects corrupted files missing the magic bytes.
- `test_tensor_scanner_gguf_success(scanner, tmp_path)` — [`L61`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_tensor_auditor.py#L61) — Proves the scanner validates the GGUF magic bytes and successfully extracts
- `test_tensor_scanner_param_formatting(scanner)` — [`L123`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_tensor_auditor.py#L123) — Proves the engine accurately translates raw parameters into human scales.
- `test_tensor_scanner_safetensors_massive_header(scanner, tmp_path)` — [`L98`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_tensor_auditor.py#L98) — Proves that a maliciously crafted safetensors file claiming to have an
- `test_tensor_scanner_safetensors_success(scanner, tmp_path)` — [`L18`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_tensor_auditor.py#L18) — Proves the scanner correctly unpacks the uint64 header, reads the JSON,

