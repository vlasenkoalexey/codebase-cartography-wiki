---
title: 'Module: tests/unit/tools/test_scip_pipeline_calls.py'
type: catalog
provenance: extracted
module: tests/unit/tools/test_scip_pipeline_calls.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `tests.unit.tools.test_scip_pipeline_calls`/
symbols:
  test_scip_pipeline_runs_build_function_call_groups: test_scip_pipeline_runs_build_function_call_groups().
  _FakeScipIndexParser.parse: _FakeScipIndexParser#parse().
  _FakeScipIndexParser: _FakeScipIndexParser#
  _FakeScipIndexParser.files_data: _FakeScipIndexParser#files_data.
  _FakeScipIndexer: _FakeScipIndexer#
  _FakeParser: _FakeParser#
  _FakeScipIndexer.run: _FakeScipIndexer#run().
  _FakeParser.parse: _FakeParser#parse().
---
# Module: [`tests/unit/tools/test_scip_pipeline_calls.py`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_scip_pipeline_calls.py)

## Classes
### `_FakeParser`
- def: [`tests/unit/tools/test_scip_pipeline_calls.py:28`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_scip_pipeline_calls.py#L28)
- signature: `class _FakeParser:`
- members:
  - `parse(self, path: Path, _is_dependency: bool, index_source: bool = False)` — [`L29`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_scip_pipeline_calls.py#L29)
- used by: (1 test-only callers)

### `_FakeScipIndexParser`
- def: [`tests/unit/tools/test_scip_pipeline_calls.py:21`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_scip_pipeline_calls.py#L21)
- signature: `class _FakeScipIndexParser:`
- members:
  - `parse(self, _index_scip_path: Path, _project_path: Path)` — [`L24`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_scip_pipeline_calls.py#L24)
  - `files_data` — [`L22`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_scip_pipeline_calls.py#L22)
- used by: (1 test-only callers)

### `_FakeScipIndexer`
- def: [`tests/unit/tools/test_scip_pipeline_calls.py:14`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_scip_pipeline_calls.py#L14)
- signature: `class _FakeScipIndexer:`
- members:
  - `run(self, _project_path: Path, _lang: str, output_dir: Path)` — [`L15`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_scip_pipeline_calls.py#L15)
- used by: (1 test-only callers)

## Functions
- `test_scip_pipeline_runs_build_function_call_groups(tmp_path: Path)` — [`L52`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_scip_pipeline_calls.py#L52)

