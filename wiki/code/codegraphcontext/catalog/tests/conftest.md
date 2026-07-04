---
title: 'Module: tests/conftest.py'
type: catalog
provenance: extracted
module: tests/conftest.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `tests.conftest`/
symbols:
  SAMPLE_PROJECTS_DIR: SAMPLE_PROJECTS_DIR.
  FIXTURES_DIR: FIXTURES_DIR.
  sample_projects_path: sample_projects_path().
  TEST_ROOT: TEST_ROOT.
  pytest_addoption: pytest_addoption().
  update_goldens: update_goldens().
  python_sample_project: python_sample_project().
  javascript_sample_project: javascript_sample_project().
  temp_test_dir: temp_test_dir().
---
# Module: [`tests/conftest.py`](../../../../../raw/code/codegraphcontext/tests/conftest.py)

## Functions
- `javascript_sample_project(sample_projects_path)` — [`L41`](../../../../../raw/code/codegraphcontext/tests/conftest.py#L41) — Returns path to the JavaScript sample project.
- `pytest_addoption(parser)` — [`L8`](../../../../../raw/code/codegraphcontext/tests/conftest.py#L8)
- `python_sample_project(sample_projects_path)` — [`L33`](../../../../../raw/code/codegraphcontext/tests/conftest.py#L33) — Returns path to the Python sample project.
- `sample_projects_path()` — [`L26`](../../../../../raw/code/codegraphcontext/tests/conftest.py#L26) — Returns the path to the directory containing all sample projects.
- `temp_test_dir()` — [`L49`](../../../../../raw/code/codegraphcontext/tests/conftest.py#L49) — Creates a temporary directory for file operations, cleaned up after test.
- `update_goldens(request)` — [`L17`](../../../../../raw/code/codegraphcontext/tests/conftest.py#L17)

## Module values
- `FIXTURES_DIR` — [`L22`](../../../../../raw/code/codegraphcontext/tests/conftest.py#L22)
- `SAMPLE_PROJECTS_DIR` — [`L23`](../../../../../raw/code/codegraphcontext/tests/conftest.py#L23)
- `TEST_ROOT` — [`L21`](../../../../../raw/code/codegraphcontext/tests/conftest.py#L21)

