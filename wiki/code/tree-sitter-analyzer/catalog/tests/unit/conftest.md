---
title: 'Module: tests/unit/conftest.py'
type: catalog
provenance: extracted
module: tests/unit/conftest.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.conftest`/
symbols:
  _write: _write().
  flask_project: flask_project().
  fastapi_project: fastapi_project().
  express_project: express_project().
  spring_project: spring_project().
  go_nethttp_project: go_nethttp_project().
  go_gin_project: go_gin_project().
  go_echo_project: go_echo_project().
  go_fiber_project: go_fiber_project().
  go_multi_framework_project: go_multi_framework_project().
  multi_framework_project: multi_framework_project().
---
# Module: [`tests/unit/conftest.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/conftest.py)

## Functions
- `_write(root: Path, rel: str, content: str)` — [`L10`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/conftest.py#L10)
- `express_project(tmp_path: Path)` — [`L68`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/conftest.py#L68)
- `fastapi_project(tmp_path: Path)` — [`L43`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/conftest.py#L43)
- `flask_project(tmp_path: Path)` — [`L18`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/conftest.py#L18)
- `go_echo_project(tmp_path: Path)` — [`L153`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/conftest.py#L153)
- `go_fiber_project(tmp_path: Path)` — [`L174`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/conftest.py#L174)
- `go_gin_project(tmp_path: Path)` — [`L131`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/conftest.py#L131)
- `go_multi_framework_project(tmp_path: Path)` — [`L195`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/conftest.py#L195)
- `go_nethttp_project(tmp_path: Path)` — [`L109`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/conftest.py#L109)
- `multi_framework_project(flask_project: Path, fastapi_project: Path, express_project: Path)` — [`L228`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/conftest.py#L228) — flask_project is base; merge fastapi + express in.
- `spring_project(tmp_path: Path)` — [`L84`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/conftest.py#L84)

