---
title: 'Module: tests/fixtures/factories.py'
type: catalog
provenance: extracted
module: tests/fixtures/factories.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.fixtures.factories`/
symbols:
  AnalysisResultFactory.create_simple_analysis_result: AnalysisResultFactory#create_simple_analysis_result().
  create_test_analysis_result: create_test_analysis_result().
  create_test_elements: create_test_elements().
  AnalysisResultFactory.create_empty_analysis_result: AnalysisResultFactory#create_empty_analysis_result().
  AnalysisResultFactory.create_analysis_result_with_metadata: AnalysisResultFactory#create_analysis_result_with_metadata().
  QueryResultFactory.create_simple_query_result: QueryResultFactory#create_simple_query_result().
  QueryResultFactory.create_empty_query_result: QueryResultFactory#create_empty_query_result().
  QueryResultFactory.create_error_query_result: QueryResultFactory#create_error_query_result().
  PerformanceStatsFactory.create_empty_performance_stats: PerformanceStatsFactory#create_empty_performance_stats().
  CodeElementFactory: CodeElementFactory#
  AnalysisResultFactory: AnalysisResultFactory#
  AnalysisResultFactory.create_analysis_result: AnalysisResultFactory#create_analysis_result().
  QueryResultFactory: QueryResultFactory#
  QueryResultFactory.create_query_result: QueryResultFactory#create_query_result().
  CodeElementFactory.create_class_element: CodeElementFactory#create_class_element().
  CodeElementFactory.create_method_element: CodeElementFactory#create_method_element().
  CodeElementFactory.create_function_element: CodeElementFactory#create_function_element().
  PerformanceStatsFactory: PerformanceStatsFactory#
  PerformanceStatsFactory.create_performance_stats: PerformanceStatsFactory#create_performance_stats().
  CodeElementFactory.create_property_element: CodeElementFactory#create_property_element().
  CodeElementFactory.create_variable_element: CodeElementFactory#create_variable_element().
  CodeElementFactory.create_interface_element: CodeElementFactory#create_interface_element().
  CodeElementFactory.create_enum_element: CodeElementFactory#create_enum_element().
  CodeElementFactory.create_namespace_element: CodeElementFactory#create_namespace_element().
  FileContentFactory: FileContentFactory#
  FileContentFactory.create_python_file_content: FileContentFactory#create_python_file_content().
  FileContentFactory.create_java_file_content: FileContentFactory#create_java_file_content().
  FileContentFactory.create_javascript_file_content: FileContentFactory#create_javascript_file_content().
---
# Module: [`tests/fixtures/factories.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/factories.py)

## Classes
### `AnalysisResultFactory`
- def: [`tests/fixtures/factories.py:271`](../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/factories.py#L271)
- doc: 分析结果工厂类。
- signature: `class AnalysisResultFactory:`
- members:
  - `create_analysis_result(file_path: Path | None = None, language: str = "python", elements: list[dict[str, Any]] | None = None, metadata: dict[str, Any] | None = None, **kwargs: Any)` — [`L278`](../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/factories.py#L278) — 创建分析结果。
  - `create_analysis_result_with_metadata(file_path: Path | None = None, analysis_time: float | None = None, element_count: int | None = None, **kwargs: Any)` — [`L369`](../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/factories.py#L369) — 创建带有元数据的分析结果。
  - `create_empty_analysis_result(file_path: Path | None = None, **kwargs: Any)` — [`L352`](../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/factories.py#L352) — 创建空的分析结果。
  - `create_simple_analysis_result(num_classes: int = 1, num_methods: int = 2, num_functions: int = 1, **kwargs: Any)` — [`L306`](../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/factories.py#L306) — 创建简单的分析结果。
- uses (calls/refs, reference-scoped): (4 test-only callers)
- used by: (1 test-only callers)

### `CodeElementFactory`
- def: [`tests/fixtures/factories.py:13`](../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/factories.py#L13)
- doc: 代码元素工厂类。
- signature: `class CodeElementFactory:`
- members:
  - `create_class_element(name: str = "TestClass", line_start: int = 1, line_end: int = 10, is_private: bool = False, **kwargs: Any)` — [`L20`](../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/factories.py#L20) — 创建类元素。
  - `create_enum_element(name: str = "TestEnum", line_start: int = 1, line_end: int = 6, is_private: bool = False, values: list[str] | None = None, **kwargs: Any)` — [`L209`](../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/factories.py#L209) — 创建枚举元素。
  - `create_function_element(name: str = "test_function", line_start: int = 1, line_end: int = 5, is_private: bool = False, parameters: list[str] | None = None, return_type: str | None = None, **kwargs: Any)` — [`L81`](../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/factories.py#L81) — 创建函数元素。
  - `create_interface_element(name: str = "TestInterface", line_start: int = 1, line_end: int = 8, is_private: bool = False, **kwargs: Any)` — [`L180`](../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/factories.py#L180) — 创建接口元素。
  - `create_method_element(name: str = "test_method", line_start: int = 5, line_end: int = 8, is_private: bool = False, parameters: list[str] | None = None, **kwargs: Any)` — [`L49`](../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/factories.py#L49) — 创建方法元素。
  - `create_namespace_element(name: str = "TestNamespace", line_start: int = 1, line_end: int = 20, is_private: bool = False, **kwargs: Any)` — [`L241`](../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/factories.py#L241) — 创建命名空间元素。
  - `create_property_element(name: str = "test_property", line_start: int = 3, line_end: int = 3, is_private: bool = False, property_type: str | None = None, **kwargs: Any)` — [`L116`](../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/factories.py#L116) — 创建属性元素。
  - `create_variable_element(name: str = "test_variable", line_start: int = 2, line_end: int = 2, is_private: bool = False, variable_type: str | None = None, **kwargs: Any)` — [`L148`](../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/factories.py#L148) — 创建变量元素。
- used by: (2 test-only callers)

### `FileContentFactory`
- def: [`tests/fixtures/factories.py:551`](../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/factories.py#L551)
- doc: 文件内容工厂类。
- signature: `class FileContentFactory:`
- members:
  - `create_java_file_content(num_classes: int = 1, **kwargs: Any)` — [`L590`](../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/factories.py#L590) — 创建Java文件内容。
  - `create_javascript_file_content(num_functions: int = 2, **kwargs: Any)` — [`L613`](../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/factories.py#L613) — 创建JavaScript文件内容。
  - `create_python_file_content(num_classes: int = 1, num_functions: int = 2, **kwargs: Any)` — [`L558`](../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/factories.py#L558) — 创建Python文件内容。

### `PerformanceStatsFactory`
- def: [`tests/fixtures/factories.py:490`](../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/factories.py#L490)
- doc: 性能统计工厂类。
- signature: `class PerformanceStatsFactory:`
- members:
  - `create_empty_performance_stats(operation_name: str = "test_operation", **kwargs: Any)` — [`L528`](../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/factories.py#L528) — 创建空的性能统计。
  - `create_performance_stats(operation_name: str = "test_operation", execution_time: float = 0.5, memory_usage: int = 1024, cache_hits: int = 5, cache_misses: int = 2, **kwargs: Any)` — [`L497`](../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/factories.py#L497) — 创建性能统计。

### `QueryResultFactory`
- def: [`tests/fixtures/factories.py:398`](../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/factories.py#L398)
- doc: 查询结果工厂类。
- signature: `class QueryResultFactory:`
- members:
  - `create_empty_query_result(query_name: str = "test_query", **kwargs: Any)` — [`L452`](../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/factories.py#L452) — 创建空的查询结果。
  - `create_error_query_result(query_name: str = "test_query", error_message: str = "Query failed", **kwargs: Any)` — [`L469`](../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/factories.py#L469) — 创建错误查询结果。
  - `create_query_result(query_name: str = "test_query", matches: list[dict[str, Any]] | None = None, success: bool = True, error_message: str | None = None, **kwargs: Any)` — [`L405`](../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/factories.py#L405) — 创建查询结果。
  - `create_simple_query_result(num_matches: int = 3, **kwargs: Any)` — [`L433`](../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/factories.py#L433) — 创建简单的查询结果。

## Functions
- `create_test_analysis_result(file_path: Path | None = None, num_elements: int = 5)` — [`L654`](../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/factories.py#L654) — 创建测试分析结果。
- `create_test_elements(count: int = 5)` — [`L635`](../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/factories.py#L635) — 创建测试元素列表。

