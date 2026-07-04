---
title: 'Module: tests/unit/cli/test_analyze_complexity_file_path.py'
type: catalog
provenance: extracted
module: tests/unit/cli/test_analyze_complexity_file_path.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `tests.unit.cli.test_analyze_complexity_file_path`/
symbols:
  TestIsFilePathDetection._is_file_path: TestIsFilePathDetection#_is_file_path().
  runner: runner.
  cli_env: cli_env().
  _FakeCodeFinder.calls: _FakeCodeFinder#calls.
  _FakeCodeFinder.get_cyclomatic_complexity: _FakeCodeFinder#get_cyclomatic_complexity().
  _FakeCodeFinder.find_most_complex_functions: _FakeCodeFinder#find_most_complex_functions().
  _FakeCodeFinder.find_most_complex_functions_in_file: _FakeCodeFinder#find_most_complex_functions_in_file().
  TestIsFilePathDetection.test_path_with_slash: TestIsFilePathDetection#test_path_with_slash().
  TestIsFilePathDetection.test_path_with_backslash: TestIsFilePathDetection#test_path_with_backslash().
  TestIsFilePathDetection.test_deep_path: TestIsFilePathDetection#test_deep_path().
  TestIsFilePathDetection.test_bare_python_file: TestIsFilePathDetection#test_bare_python_file().
  TestIsFilePathDetection.test_bare_js_file: TestIsFilePathDetection#test_bare_js_file().
  TestIsFilePathDetection.test_bare_go_file: TestIsFilePathDetection#test_bare_go_file().
  TestIsFilePathDetection.test_bare_ts_file: TestIsFilePathDetection#test_bare_ts_file().
  TestIsFilePathDetection.test_bare_rust_file: TestIsFilePathDetection#test_bare_rust_file().
  TestIsFilePathDetection.test_simple_function_name: TestIsFilePathDetection#test_simple_function_name().
  TestIsFilePathDetection.test_class_method_name: TestIsFilePathDetection#test_class_method_name().
  TestIsFilePathDetection.test_snake_case_function: TestIsFilePathDetection#test_snake_case_function().
  TestIsFilePathDetection.test_camel_case_function: TestIsFilePathDetection#test_camel_case_function().
  TestComplexityCommandRouting.test_no_args_calls_global: TestComplexityCommandRouting#test_no_args_calls_global().
  TestComplexityCommandRouting.test_function_name_calls_get_complexity: TestComplexityCommandRouting#test_function_name_calls_get_complexity().
  TestComplexityCommandRouting.test_file_path_with_slash_calls_file_method: TestComplexityCommandRouting#test_file_path_with_slash_calls_file_method().
  TestComplexityCommandRouting.test_bare_filename_calls_file_method: TestComplexityCommandRouting#test_bare_filename_calls_file_method().
  TestComplexityCommandRouting.test_file_option_without_positional_calls_file_method: TestComplexityCommandRouting#test_file_option_without_positional_calls_file_method().
  TestComplexityCommandRouting.test_function_name_with_file_option_calls_get_complexity: TestComplexityCommandRouting#test_function_name_with_file_option_calls_get_complexity().
  TestComplexityCommandOutput.test_file_path_shows_table_with_file_title: TestComplexityCommandOutput#test_file_path_shows_table_with_file_title().
  TestComplexityCommandOutput.test_global_shows_threshold_info: TestComplexityCommandOutput#test_global_shows_threshold_info().
  TestComplexityCommandOutput.test_function_name_shows_single_result: TestComplexityCommandOutput#test_function_name_shows_single_result().
  TestComplexityCommandOutput.test_empty_file_results_shows_message: TestComplexityCommandOutput#test_empty_file_results_shows_message().
  _FakeDBManager: _FakeDBManager#
  _FakeGraphBuilder: _FakeGraphBuilder#
  _FakeCodeFinder: _FakeCodeFinder#
  _FakeDBManager.get_driver: _FakeDBManager#get_driver().
  _FakeDBManager.close_driver: _FakeDBManager#close_driver().
  _FakeCodeFinder.__init__: _FakeCodeFinder#__init__().
  TestIsFilePathDetection: TestIsFilePathDetection#
  TestComplexityCommandRouting: TestComplexityCommandRouting#
  TestComplexityCommandOutput: TestComplexityCommandOutput#
---
# Module: [`tests/unit/cli/test_analyze_complexity_file_path.py`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_analyze_complexity_file_path.py)

## Classes
### `TestComplexityCommandOutput`
- def: [`tests/unit/cli/test_analyze_complexity_file_path.py:162`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_analyze_complexity_file_path.py#L162)
- doc: Verify that the CLI output contains expected content.
- signature: `class TestComplexityCommandOutput:`
- members:
  - `test_empty_file_results_shows_message(self, cli_env)` — [`L181`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_analyze_complexity_file_path.py#L181) — When no functions found in file, show appropriate message.
  - `test_file_path_shows_table_with_file_title(self, cli_env)` — [`L165`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_analyze_complexity_file_path.py#L165)
  - `test_function_name_shows_single_result(self, cli_env)` — [`L176`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_analyze_complexity_file_path.py#L176)
  - `test_global_shows_threshold_info(self, cli_env)` — [`L171`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_analyze_complexity_file_path.py#L171)
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `TestComplexityCommandRouting`
- def: [`tests/unit/cli/test_analyze_complexity_file_path.py:119`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_analyze_complexity_file_path.py#L119)
- doc: Verify that the CLI routes to the correct CodeFinder method
- signature: `class TestComplexityCommandRouting:`
- members:
  - `test_bare_filename_calls_file_method(self, cli_env)` — [`L141`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_analyze_complexity_file_path.py#L141) — cgc analyze complexity main.py → find_most_complex_functions_in_file
  - `test_file_option_without_positional_calls_file_method(self, cli_env)` — [`L147`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_analyze_complexity_file_path.py#L147) — cgc analyze complexity --file src/main.py → find_most_complex_functions_in_file
  - `test_file_path_with_slash_calls_file_method(self, cli_env)` — [`L135`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_analyze_complexity_file_path.py#L135) — cgc analyze complexity src/main.py → find_most_complex_functions_in_file
  - `test_function_name_calls_get_complexity(self, cli_env)` — [`L129`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_analyze_complexity_file_path.py#L129) — cgc analyze complexity my_function → get_cyclomatic_complexity
  - `test_function_name_with_file_option_calls_get_complexity(self, cli_env)` — [`L153`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_analyze_complexity_file_path.py#L153) — cgc analyze complexity my_func -f main.py → get_cyclomatic_complexity
  - `test_no_args_calls_global(self, cli_env)` — [`L123`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_analyze_complexity_file_path.py#L123) — cgc analyze complexity → find_most_complex_functions
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `TestIsFilePathDetection`
- def: [`tests/unit/cli/test_analyze_complexity_file_path.py:62`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_analyze_complexity_file_path.py#L62)
- doc: Verify that the file-path heuristic correctly distinguishes
- signature: `class TestIsFilePathDetection:`
- members:
  - `_is_file_path(self, value: str)` — [`L66`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_analyze_complexity_file_path.py#L66) — Mirror the logic in analyze_complexity.
  - `test_bare_go_file(self)` — [`L94`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_analyze_complexity_file_path.py#L94)
  - `test_bare_js_file(self)` — [`L91`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_analyze_complexity_file_path.py#L91)
  - `test_bare_python_file(self)` — [`L88`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_analyze_complexity_file_path.py#L88)
  - `test_bare_rust_file(self)` — [`L100`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_analyze_complexity_file_path.py#L100)
  - `test_bare_ts_file(self)` — [`L97`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_analyze_complexity_file_path.py#L97)
  - `test_camel_case_function(self)` — [`L113`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_analyze_complexity_file_path.py#L113)
  - `test_class_method_name(self)` — [`L107`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_analyze_complexity_file_path.py#L107)
  - `test_deep_path(self)` — [`L84`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_analyze_complexity_file_path.py#L84)
  - `test_path_with_backslash(self)` — [`L81`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_analyze_complexity_file_path.py#L81)
  - `test_path_with_slash(self)` — [`L78`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_analyze_complexity_file_path.py#L78)
  - `test_simple_function_name(self)` — [`L104`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_analyze_complexity_file_path.py#L104)
  - `test_snake_case_function(self)` — [`L110`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_analyze_complexity_file_path.py#L110)

### `_FakeCodeFinder`
- def: [`tests/unit/cli/test_analyze_complexity_file_path.py:28`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_analyze_complexity_file_path.py#L28)
- doc: Tracks which methods are called so we can assert routing.
- signature: `class _FakeCodeFinder:`
- members:
  - `find_most_complex_functions(self, *args, **kwargs)` — [`L38`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_analyze_complexity_file_path.py#L38)
  - `find_most_complex_functions_in_file(self, *args, **kwargs)` — [`L42`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_analyze_complexity_file_path.py#L42)
  - `get_cyclomatic_complexity(self, *args, **kwargs)` — [`L34`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_analyze_complexity_file_path.py#L34)
  - `calls` — [`L32`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_analyze_complexity_file_path.py#L32)
- protocol/private: `__init__`[`L31`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_analyze_complexity_file_path.py#L31)
- used by: (1 test-only callers)

### `_FakeDBManager`
- def: [`tests/unit/cli/test_analyze_complexity_file_path.py:16`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_analyze_complexity_file_path.py#L16)
- signature: `class _FakeDBManager:`
- members:
  - `close_driver(self)` — [`L20`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_analyze_complexity_file_path.py#L20)
  - `get_driver(self)` — [`L17`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_analyze_complexity_file_path.py#L17)
- used by: (1 test-only callers)

### `_FakeGraphBuilder`
- def: [`tests/unit/cli/test_analyze_complexity_file_path.py:24`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_analyze_complexity_file_path.py#L24)
- signature: `class _FakeGraphBuilder:`
- used by: (1 test-only callers)

## Functions
- `cli_env(monkeypatch, tmp_path)` — [`L48`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_analyze_complexity_file_path.py#L48) — Set up minimal CLI stubs for complexity command testing.

## Module values
- `runner` — [`L14`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_analyze_complexity_file_path.py#L14)

