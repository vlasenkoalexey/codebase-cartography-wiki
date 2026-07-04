---
title: 'Module: gitgalaxy/metrics/tensor_scanner.py'
type: catalog
provenance: extracted
module: gitgalaxy/metrics/tensor_scanner.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `gitgalaxy.metrics.tensor_scanner`/TensorScanner#
symbols:
  TensorScanner.audit_model: audit_model().
  TensorScanner: ''
  TensorScanner._parse_safetensors: _parse_safetensors().
  TensorScanner.logger: logger.
  TensorScanner._parse_gguf: _parse_gguf().
  TensorScanner._format_params: _format_params().
  TensorScanner.__init__: __init__().
---
# Module: [`gitgalaxy/metrics/tensor_scanner.py`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/tensor_scanner.py)

## Classes
### `TensorScanner`
- def: [`gitgalaxy/metrics/tensor_scanner.py:13`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/tensor_scanner.py#L13)
- doc: Surgically inspects massive AI model binaries (.safetensors, .gguf)
- signature: `class TensorScanner:`
- members:
  - `_format_params(self, count: int)` — [`L143`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/tensor_scanner.py#L143) — Converts raw integer parameters into human-readable B/M format.
  - `_parse_gguf(self, file_path: str)` — [`L98`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/tensor_scanner.py#L98) — GGUF format:
  - `_parse_safetensors(self, file_path: str)` — [`L46`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/tensor_scanner.py#L46) — Safetensors format:
  - `audit_model(self, file_path: str)` — [`L23`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/tensor_scanner.py#L23) — Routes the binary to the correct header parser.
  - `logger` — [`L21`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/tensor_scanner.py#L21)
- protocol/private: `__init__`[`L20`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/tensor_scanner.py#L20)
- used by: [`used_tokens`](../galaxyscope.md#Orchestrator.used_tokens)  (1 test-only)

