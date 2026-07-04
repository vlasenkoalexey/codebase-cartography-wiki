---
title: 'Module: tests/integration/formatters/test_toon_public_contract.py'
type: catalog
provenance: extracted
module: tests/integration/formatters/test_toon_public_contract.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.formatters.test_toon_public_contract`/TestToonEncoderPublicContract#
symbols:
  TestToonEncoderPublicContract.test_contract_simple_dict_structure: test_contract_simple_dict_structure().
  TestToonEncoderPublicContract.test_contract_homogeneous_array_uses_array_table: test_contract_homogeneous_array_uses_array_table().
  TestToonEncoderPublicContract.test_contract_mixed_array_uses_inline_json: test_contract_mixed_array_uses_inline_json().
  TestToonEncoderPublicContract.test_contract_nested_structure_preserves_hierarchy: test_contract_nested_structure_preserves_hierarchy().
  TestToonEncoderPublicContract.test_contract_empty_containers_handled: test_contract_empty_containers_handled().
  TestToonEncoderPublicContract.test_contract_unicode_content_preserved: test_contract_unicode_content_preserved().
  TestToonEncoderPublicContract.test_contract_large_array_does_not_timeout: test_contract_large_array_does_not_timeout().
  TestToonEncoderPublicContract.test_contract_circular_reference_no_crash: test_contract_circular_reference_no_crash().
  TestToonEncoderPublicContract.test_contract_priority_fields_order_respected: test_contract_priority_fields_order_respected().
  TestToonEncoderPublicContract.test_contract_docstring_truncation_with_ellipsis: test_contract_docstring_truncation_with_ellipsis().
  TestToonEncoderPublicContract: ''
---
# Module: [`tests/integration/formatters/test_toon_public_contract.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_toon_public_contract.py)

## Classes
### `TestToonEncoderPublicContract`
- def: [`tests/integration/formatters/test_toon_public_contract.py:14`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_toon_public_contract.py#L14)
- doc: 对外契约测试：外部用户依赖的核心行为
- signature: `class TestToonEncoderPublicContract:`
- members:
  - `test_contract_circular_reference_no_crash(self)` — [`L120`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_toon_public_contract.py#L120) — 契约：循环引用不导致堆栈溢出
  - `test_contract_docstring_truncation_with_ellipsis(self)` — [`L178`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_toon_public_contract.py#L178) — 契约：超长 docstring 被截断并添加 ... 标记
  - `test_contract_empty_containers_handled(self)` — [`L77`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_toon_public_contract.py#L77) — 契约：空容器不导致崩溃
  - `test_contract_homogeneous_array_uses_array_table(self)` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_toon_public_contract.py#L28) — 契约：同构数组使用 Array Table 格式（紧凑表示）
  - `test_contract_large_array_does_not_timeout(self)` — [`L101`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_toon_public_contract.py#L101) — 契约：大数组处理不超时（性能契约）
  - `test_contract_mixed_array_uses_inline_json(self)` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_toon_public_contract.py#L45) — 契约：非同构数组使用内联 JSON 格式
  - `test_contract_nested_structure_preserves_hierarchy(self)` — [`L60`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_toon_public_contract.py#L60) — 契约：嵌套结构保持层级关系
  - `test_contract_priority_fields_order_respected(self)` — [`L139`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_toon_public_contract.py#L139) — 契约：高优先级字段优先保留（当字段数超限时）
  - `test_contract_simple_dict_structure(self)` — [`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_toon_public_contract.py#L17) — 契约：简单 dict 编码为 key: value 格式
  - `test_contract_unicode_content_preserved(self)` — [`L90`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_toon_public_contract.py#L90) — 契约：Unicode 内容正确保留
- uses (calls/refs, reference-scoped): [`ToonEncoder`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder), [`encode`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder.encode)

