---
title: 'Module: tests/unit/test_pipx_runner_support.py'
type: catalog
provenance: extracted
module: tests/unit/test_pipx_runner_support.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `tests.unit.test_pipx_runner_support`/
symbols:
  _run_generate_mcp_json: _run_generate_mcp_json().
  _get_server_block: _get_server_block().
  TestTC05_ReadmeDocumentation.README_PATH: TestTC05_ReadmeDocumentation#README_PATH.
  TestTC02_PipxAvailable.test_pipx_used_when_cgc_absent: TestTC02_PipxAvailable#test_pipx_used_when_cgc_absent().
  TestTC01_CgcAvailable.test_cgc_path_available_uses_cgc_command: TestTC01_CgcAvailable#test_cgc_path_available_uses_cgc_command().
  TestTC01_CgcAvailable.test_cgc_available_does_not_use_pipx: TestTC01_CgcAvailable#test_cgc_available_does_not_use_pipx().
  TestTC02_PipxAvailable.test_pipx_args_contain_codegraphcontext_package: TestTC02_PipxAvailable#test_pipx_args_contain_codegraphcontext_package().
  TestTC03_PythonFallback.test_python_fallback_when_both_absent: TestTC03_PythonFallback#test_python_fallback_when_both_absent().
  TestTC03_PythonFallback.test_fallback_args_include_mcp_start: TestTC03_PythonFallback#test_fallback_args_include_mcp_start().
  TestTC06_McpJsonFileOutput.test_mcp_json_written_with_pipx_command: TestTC06_McpJsonFileOutput#test_mcp_json_written_with_pipx_command().
  TestTC07_PipxIsolatedEnvArgs.test_pipx_run_keyword_present_for_isolated_env: TestTC07_PipxIsolatedEnvArgs#test_pipx_run_keyword_present_for_isolated_env().
  TestTC08_PipxNotUsingPythonModule.test_pipx_args_do_not_contain_module_flag: TestTC08_PipxNotUsingPythonModule#test_pipx_args_do_not_contain_module_flag().
  TestTC09_PipxBinaryAsCommand.test_pipx_binary_path_used_as_command: TestTC09_PipxBinaryAsCommand#test_pipx_binary_path_used_as_command().
  DUMMY_CREDS: DUMMY_CREDS.
  TestTC04_KuzuSetupBlock._run_kuzu_block: TestTC04_KuzuSetupBlock#_run_kuzu_block().
  TestTC04_KuzuSetupBlock.test_kuzu_block_pipx_detected: TestTC04_KuzuSetupBlock#test_kuzu_block_pipx_detected().
  TestTC04_KuzuSetupBlock.test_kuzu_block_cgc_takes_priority_over_pipx: TestTC04_KuzuSetupBlock#test_kuzu_block_cgc_takes_priority_over_pipx().
  TestTC04_KuzuSetupBlock.test_kuzu_block_python_fallback: TestTC04_KuzuSetupBlock#test_kuzu_block_python_fallback().
  TestTC05_ReadmeDocumentation.test_readme_exists: TestTC05_ReadmeDocumentation#test_readme_exists().
  TestTC05_ReadmeDocumentation.test_readme_contains_pipx_command: TestTC05_ReadmeDocumentation#test_readme_contains_pipx_command().
  TestTC05_ReadmeDocumentation.test_readme_contains_pipx_run_codegraphcontext: TestTC05_ReadmeDocumentation#test_readme_contains_pipx_run_codegraphcontext().
  TestTC05_ReadmeDocumentation.test_readme_pipx_config_has_mcp_start: TestTC05_ReadmeDocumentation#test_readme_pipx_config_has_mcp_start().
  TestTC06_McpJsonFileOutput.test_mcp_json_structure_valid: TestTC06_McpJsonFileOutput#test_mcp_json_structure_valid().
  TestTC02_PipxAvailable.which_side: TestTC02_PipxAvailable#which_side().
  TestTC01_CgcAvailable: TestTC01_CgcAvailable#
  TestTC02_PipxAvailable: TestTC02_PipxAvailable#
  TestTC03_PythonFallback: TestTC03_PythonFallback#
  TestTC04_KuzuSetupBlock: TestTC04_KuzuSetupBlock#
  TestTC05_ReadmeDocumentation: TestTC05_ReadmeDocumentation#
  TestTC06_McpJsonFileOutput: TestTC06_McpJsonFileOutput#
  TestTC07_PipxIsolatedEnvArgs: TestTC07_PipxIsolatedEnvArgs#
  TestTC08_PipxNotUsingPythonModule: TestTC08_PipxNotUsingPythonModule#
  TestTC09_PipxBinaryAsCommand: TestTC09_PipxBinaryAsCommand#
---
# Module: [`tests/unit/test_pipx_runner_support.py`](../../../../../../raw/code/codegraphcontext/tests/unit/test_pipx_runner_support.py)

## Classes
### `TestTC01_CgcAvailable`
- def: [`tests/unit/test_pipx_runner_support.py:54`](../../../../../../raw/code/codegraphcontext/tests/unit/test_pipx_runner_support.py#L54)
- signature: `class TestTC01_CgcAvailable:`
- members:
  - `test_cgc_available_does_not_use_pipx(self)` — [`L66`](../../../../../../raw/code/codegraphcontext/tests/unit/test_pipx_runner_support.py#L66)
  - `test_cgc_path_available_uses_cgc_command(self)` — [`L56`](../../../../../../raw/code/codegraphcontext/tests/unit/test_pipx_runner_support.py#L56)
- uses (calls/refs, reference-scoped): (2 test-only callers)

### `TestTC02_PipxAvailable`
- def: [`tests/unit/test_pipx_runner_support.py:83`](../../../../../../raw/code/codegraphcontext/tests/unit/test_pipx_runner_support.py#L83)
- signature: `class TestTC02_PipxAvailable:`
- members:
  - `test_pipx_args_contain_codegraphcontext_package(self)` — [`L100`](../../../../../../raw/code/codegraphcontext/tests/unit/test_pipx_runner_support.py#L100)
  - `test_pipx_used_when_cgc_absent(self)` — [`L85`](../../../../../../raw/code/codegraphcontext/tests/unit/test_pipx_runner_support.py#L85)
  - `which_side(name)` — [`L86`](../../../../../../raw/code/codegraphcontext/tests/unit/test_pipx_runner_support.py#L86)
- uses (calls/refs, reference-scoped): (2 test-only callers)

### `TestTC03_PythonFallback`
- def: [`tests/unit/test_pipx_runner_support.py:117`](../../../../../../raw/code/codegraphcontext/tests/unit/test_pipx_runner_support.py#L117)
- signature: `class TestTC03_PythonFallback:`
- members:
  - `test_fallback_args_include_mcp_start(self)` — [`L140`](../../../../../../raw/code/codegraphcontext/tests/unit/test_pipx_runner_support.py#L140)
  - `test_python_fallback_when_both_absent(self)` — [`L119`](../../../../../../raw/code/codegraphcontext/tests/unit/test_pipx_runner_support.py#L119)
- uses (calls/refs, reference-scoped): (2 test-only callers)

### `TestTC04_KuzuSetupBlock`
- def: [`tests/unit/test_pipx_runner_support.py:168`](../../../../../../raw/code/codegraphcontext/tests/unit/test_pipx_runner_support.py#L168)
- signature: `class TestTC04_KuzuSetupBlock:`
- members:
  - `test_kuzu_block_cgc_takes_priority_over_pipx(self)` — [`L187`](../../../../../../raw/code/codegraphcontext/tests/unit/test_pipx_runner_support.py#L187)
  - `test_kuzu_block_pipx_detected(self)` — [`L182`](../../../../../../raw/code/codegraphcontext/tests/unit/test_pipx_runner_support.py#L182)
  - `test_kuzu_block_python_fallback(self)` — [`L192`](../../../../../../raw/code/codegraphcontext/tests/unit/test_pipx_runner_support.py#L192)
- protocol/private: `_run_kuzu_block`[`L170`](../../../../../../raw/code/codegraphcontext/tests/unit/test_pipx_runner_support.py#L170)

### `TestTC05_ReadmeDocumentation`
- def: [`tests/unit/test_pipx_runner_support.py:204`](../../../../../../raw/code/codegraphcontext/tests/unit/test_pipx_runner_support.py#L204)
- signature: `class TestTC05_ReadmeDocumentation:`
- members:
  - `test_readme_contains_pipx_command(self)` — [`L221`](../../../../../../raw/code/codegraphcontext/tests/unit/test_pipx_runner_support.py#L221)
  - `test_readme_contains_pipx_run_codegraphcontext(self)` — [`L228`](../../../../../../raw/code/codegraphcontext/tests/unit/test_pipx_runner_support.py#L228)
  - `test_readme_exists(self)` — [`L217`](../../../../../../raw/code/codegraphcontext/tests/unit/test_pipx_runner_support.py#L217)
  - `test_readme_pipx_config_has_mcp_start(self)` — [`L235`](../../../../../../raw/code/codegraphcontext/tests/unit/test_pipx_runner_support.py#L235)
  - `README_PATH` — [`L207`](../../../../../../raw/code/codegraphcontext/tests/unit/test_pipx_runner_support.py#L207)

### `TestTC06_McpJsonFileOutput`
- def: [`tests/unit/test_pipx_runner_support.py:253`](../../../../../../raw/code/codegraphcontext/tests/unit/test_pipx_runner_support.py#L253)
- signature: `class TestTC06_McpJsonFileOutput:`
- members:
  - `test_mcp_json_structure_valid(self)` — [`L266`](../../../../../../raw/code/codegraphcontext/tests/unit/test_pipx_runner_support.py#L266)
  - `test_mcp_json_written_with_pipx_command(self)` — [`L255`](../../../../../../raw/code/codegraphcontext/tests/unit/test_pipx_runner_support.py#L255)
- uses (calls/refs, reference-scoped): (2 test-only callers)

### `TestTC07_PipxIsolatedEnvArgs`
- def: [`tests/unit/test_pipx_runner_support.py:284`](../../../../../../raw/code/codegraphcontext/tests/unit/test_pipx_runner_support.py#L284)
- signature: `class TestTC07_PipxIsolatedEnvArgs:`
- members:
  - `test_pipx_run_keyword_present_for_isolated_env(self)` — [`L286`](../../../../../../raw/code/codegraphcontext/tests/unit/test_pipx_runner_support.py#L286) — TC-07: 'run' keyword must be first arg so pipx uses isolated env.
- uses (calls/refs, reference-scoped): (2 test-only callers)

### `TestTC08_PipxNotUsingPythonModule`
- def: [`tests/unit/test_pipx_runner_support.py:304`](../../../../../../raw/code/codegraphcontext/tests/unit/test_pipx_runner_support.py#L304)
- signature: `class TestTC08_PipxNotUsingPythonModule:`
- members:
  - `test_pipx_args_do_not_contain_module_flag(self)` — [`L306`](../../../../../../raw/code/codegraphcontext/tests/unit/test_pipx_runner_support.py#L306) — TC-08: '-m' flag must NOT be in pipx args — it bypasses isolated env.
- uses (calls/refs, reference-scoped): (2 test-only callers)

### `TestTC09_PipxBinaryAsCommand`
- def: [`tests/unit/test_pipx_runner_support.py:324`](../../../../../../raw/code/codegraphcontext/tests/unit/test_pipx_runner_support.py#L324)
- signature: `class TestTC09_PipxBinaryAsCommand:`
- members:
  - `test_pipx_binary_path_used_as_command(self)` — [`L326`](../../../../../../raw/code/codegraphcontext/tests/unit/test_pipx_runner_support.py#L326) — TC-09: exact pipx binary path must be the command.
- uses (calls/refs, reference-scoped): (2 test-only callers)

## Functions
- `_get_server_block(mcp_config: dict)` — [`L26`](../../../../../../raw/code/codegraphcontext/tests/unit/test_pipx_runner_support.py#L26)
- `_run_generate_mcp_json(which_side_effect)` — [`L30`](../../../../../../raw/code/codegraphcontext/tests/unit/test_pipx_runner_support.py#L30) — Helper: run _generate_mcp_json() with mocked shutil.which.

## Module values
- `DUMMY_CREDS` — [`L19`](../../../../../../raw/code/codegraphcontext/tests/unit/test_pipx_runner_support.py#L19)

