---
title: 'Module: python/ts_executor.py'
type: catalog
provenance: extracted
module: python/ts_executor.py
status: fresh
symbol_base: scip-python python claude-context 0.0.0 `python.ts_executor`/
symbols:
  result: result.
  result2: result2.
  TypeScriptExecutor.call_method: TypeScriptExecutor#call_method().
  result1: result1.
  executor: executor.
  call_ts_method: call_ts_method().
  f: f.
  TypeScriptExecutor: TypeScriptExecutor#
  e: e.
  TypeScriptExecutor.working_dir: TypeScriptExecutor#working_dir.
  TypeScriptExecutor._create_wrapper_script: TypeScriptExecutor#_create_wrapper_script().
  test_ts_content: test_ts_content.
  TypeScriptExecutor.__init__: TypeScriptExecutor#__init__().
---
# Module: [`python/ts_executor.py`](../../../../../raw/code/claude-context/python/ts_executor.py)

## Classes
### `TypeScriptExecutor`
- def: [`python/ts_executor.py:15`](../../../../../raw/code/claude-context/python/ts_executor.py#L15)
- doc: TypeScript method executor
- signature: `class TypeScriptExecutor:`
- members:
  - `__init__(self, working_dir: Optional[str] = None)` — [`L18`](../../../../../raw/code/claude-context/python/ts_executor.py#L18) — Initialize TypeScript executor
  - `_create_wrapper_script(self, ts_file_path: str, method_name: str, args: List[Any], kwargs: Dict[str, Any])` — [`L128`](../../../../../raw/code/claude-context/python/ts_executor.py#L128) — Create wrapper script
  - `call_method(self, ts_file_path: str, method_name: str, *args, **kwargs)` — [`L26`](../../../../../raw/code/claude-context/python/ts_executor.py#L26) — Call TypeScript method
  - `working_dir` — [`L24`](../../../../../raw/code/claude-context/python/ts_executor.py#L24)
- used by: [`result`](ts_executor.md#result), [`result2`](ts_executor.md#result2), [`result1`](ts_executor.md#result1), [`executor`](ts_executor.md#executor), [`call_ts_method`](ts_executor.md#call_ts_method)  (1 test-only)

## Functions
- `call_ts_method(ts_file: str, method_name: str, *args, working_dir: Optional[str] = None, **kwargs)` — [`L201`](../../../../../raw/code/claude-context/python/ts_executor.py#L201) — Convenience function: Call TypeScript method

## Module values
- `e` — [`L302`](../../../../../raw/code/claude-context/python/ts_executor.py#L302)
- `executor` — [`L261`](../../../../../raw/code/claude-context/python/ts_executor.py#L261)
- `f` — [`L256`](../../../../../raw/code/claude-context/python/ts_executor.py#L256)
- `result` — [`L267`](../../../../../raw/code/claude-context/python/ts_executor.py#L267)
- `result1` — [`L272`](../../../../../raw/code/claude-context/python/ts_executor.py#L272)
- `result2` — [`L275`](../../../../../raw/code/claude-context/python/ts_executor.py#L275)
- `test_ts_content` — [`L224`](../../../../../raw/code/claude-context/python/ts_executor.py#L224)

