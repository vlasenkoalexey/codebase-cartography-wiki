---
title: 'Module: tests/unit/languages/test_rust_impl_receiver.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_rust_impl_receiver.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_rust_impl_receiver`/
symbols:
  _functions: _functions().
  test_impl_method_gets_receiver_type: test_impl_method_gets_receiver_type().
  test_associated_function_owned_but_not_method: test_associated_function_owned_but_not_method().
  test_verbose_self_receiver_is_method: test_verbose_self_receiver_is_method().
  test_impl_method_shared_ref: test_impl_method_shared_ref().
  test_trait_impl_method_receiver_type: test_trait_impl_method_receiver_type().
  test_free_function_unowned: test_free_function_unowned().
  test_receiver_survives_api_serialization: test_receiver_survives_api_serialization().
  RUST_SRC: RUST_SRC.
---
# Module: [`tests/unit/languages/test_rust_impl_receiver.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_impl_receiver.py)

## Functions
- `_functions()` — [`L46`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_impl_receiver.py#L46)
- `test_associated_function_owned_but_not_method()` — [`L69`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_impl_receiver.py#L69) — fn new() has no self — owned by Counter but not a method.
- `test_free_function_unowned()` — [`L95`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_impl_receiver.py#L95)
- `test_impl_method_gets_receiver_type()` — [`L54`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_impl_receiver.py#L54)
- `test_impl_method_shared_ref()` — [`L63`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_impl_receiver.py#L63)
- `test_receiver_survives_api_serialization()` — [`L101`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_impl_receiver.py#L101) — End-to-end Theme-A: the serializer allowlist (landed with the Go
- `test_trait_impl_method_receiver_type()` — [`L77`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_impl_receiver.py#L77)
- `test_verbose_self_receiver_is_method()` — [`L83`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_impl_receiver.py#L83) — ``self: Box<Self>`` / ``self: Pin<&mut Self>`` parse as plain

## Module values
- `RUST_SRC` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_impl_receiver.py#L22)

