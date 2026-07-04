---
title: 'Module: tests/compatibility/test_cross_version_compatibility.py'
type: catalog
provenance: extracted
module: tests/compatibility/test_cross_version_compatibility.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.compatibility.test_cross_version_compatibility`/Test
symbols:
  TestAPIVersionCompatibility.test_analysis_request_v1_compatibility: APIVersionCompatibility#test_analysis_request_v1_compatibility().
  TestForwardCompatibility.test_new_parameters_accepted: ForwardCompatibility#test_new_parameters_accepted().
  TestPluginInterfaceCompatibility.test_python_plugin_interface: PluginInterfaceCompatibility#test_python_plugin_interface().
  TestPluginInterfaceCompatibility.test_java_plugin_interface: PluginInterfaceCompatibility#test_java_plugin_interface().
  TestPluginInterfaceCompatibility.test_javascript_plugin_interface: PluginInterfaceCompatibility#test_javascript_plugin_interface().
  TestBackwardCompatibility.test_old_analysis_request_creation: BackwardCompatibility#test_old_analysis_request_creation().
  TestBackwardCompatibility.test_old_query_execution: BackwardCompatibility#test_old_query_execution().
  TestBackwardCompatibility.test_old_format_types: BackwardCompatibility#test_old_format_types().
  TestForwardCompatibility.test_new_format_types_accepted: ForwardCompatibility#test_new_format_types_accepted().
  TestQueryFileCompatibility.test_query_loader_loads_files: QueryFileCompatibility#test_query_loader_loads_files().
  TestPluginInterfaceCompatibility.test_plugin_base_interface: PluginInterfaceCompatibility#test_plugin_base_interface().
  TestAPIVersionCompatibility.test_query_executor_v1_compatibility: APIVersionCompatibility#test_query_executor_v1_compatibility().
  TestAPIVersionCompatibility.test_query_loader_v1_compatibility: APIVersionCompatibility#test_query_loader_v1_compatibility().
  TestConfigFileCompatibility: ConfigFileCompatibility#
  TestConfigFileCompatibility.test_config_file_syntax_valid: ConfigFileCompatibility#test_config_file_syntax_valid().
  TestConfigFileCompatibility.test_config_file_missing_fields: ConfigFileCompatibility#test_config_file_missing_fields().
  TestConfigFileCompatibility.test_config_file_extra_fields: ConfigFileCompatibility#test_config_file_extra_fields().
  TestConfigFileCompatibility.test_config_file_invalid_json: ConfigFileCompatibility#test_config_file_invalid_json().
  TestConfigFileCompatibility.test_config_file_empty_queries: ConfigFileCompatibility#test_config_file_empty_queries().
  TestConfigFileCompatibility.test_config_file_multiple_languages: ConfigFileCompatibility#test_config_file_multiple_languages().
  TestQueryFileCompatibility: QueryFileCompatibility#
  TestQueryFileCompatibility.test_query_file_valid_syntax: QueryFileCompatibility#test_query_file_valid_syntax().
  TestQueryFileCompatibility.test_query_file_missing_captures: QueryFileCompatibility#test_query_file_missing_captures().
  TestQueryFileCompatibility.test_query_file_multiple_queries: QueryFileCompatibility#test_query_file_multiple_queries().
  TestQueryFileCompatibility.test_query_file_invalid_syntax: QueryFileCompatibility#test_query_file_invalid_syntax().
  TestPluginInterfaceCompatibility: PluginInterfaceCompatibility#
  TestDataFormatCompatibility: DataFormatCompatibility#
  TestDataFormatCompatibility.test_json_format_compatibility: DataFormatCompatibility#test_json_format_compatibility().
  TestDataFormatCompatibility.test_json_format_with_nested_structures: DataFormatCompatibility#test_json_format_with_nested_structures().
  TestDataFormatCompatibility.test_json_format_with_arrays: DataFormatCompatibility#test_json_format_with_arrays().
  TestDataFormatCompatibility.test_toon_format_compatibility: DataFormatCompatibility#test_toon_format_compatibility().
  TestDataFormatCompatibility.test_csv_format_compatibility: DataFormatCompatibility#test_csv_format_compatibility().
  TestAPIVersionCompatibility: APIVersionCompatibility#
  TestAPIVersionCompatibility.test_module_imports: APIVersionCompatibility#test_module_imports().
  TestBackwardCompatibility: BackwardCompatibility#
  TestForwardCompatibility: ForwardCompatibility#
---
# Module: [`tests/compatibility/test_cross_version_compatibility.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/compatibility/test_cross_version_compatibility.py)

## Classes
### `TestAPIVersionCompatibility`
- def: [`tests/compatibility/test_cross_version_compatibility.py:399`](../../../../../../raw/code/tree-sitter-analyzer/tests/compatibility/test_cross_version_compatibility.py#L399)
- doc: API版本兼容性测试
- signature: `class TestAPIVersionCompatibility:`
- members:
  - `test_analysis_request_v1_compatibility(self)` — [`L403`](../../../../../../raw/code/tree-sitter-analyzer/tests/compatibility/test_cross_version_compatibility.py#L403) — 测试AnalysisRequest v1兼容性
  - `test_module_imports(self)` — [`L451`](../../../../../../raw/code/tree-sitter-analyzer/tests/compatibility/test_cross_version_compatibility.py#L451) — 测试模块导入兼容性
  - `test_query_executor_v1_compatibility(self)` — [`L426`](../../../../../../raw/code/tree-sitter-analyzer/tests/compatibility/test_cross_version_compatibility.py#L426) — 测试QueryExecutor v1兼容性
  - `test_query_loader_v1_compatibility(self)` — [`L441`](../../../../../../raw/code/tree-sitter-analyzer/tests/compatibility/test_cross_version_compatibility.py#L441) — 测试QueryLoader v1兼容性
- uses (calls/refs, reference-scoped): [`AnalysisRequest`](../../tree_sitter_analyzer/core/request.md#AnalysisRequest), [`file_path`](../../tree_sitter_analyzer/core/request.md#AnalysisRequest.file_path), [`QueryExecutor`](../../tree_sitter_analyzer/core/query.md#QueryExecutor), [`language`](../../tree_sitter_analyzer/core/request.md#AnalysisRequest.language), [`include_complexity`](../../tree_sitter_analyzer/core/request.md#AnalysisRequest.include_complexity), [`include_details`](../../tree_sitter_analyzer/core/request.md#AnalysisRequest.include_details), [`format_type`](../../tree_sitter_analyzer/core/request.md#AnalysisRequest.format_type), [`get_query_loader`](../../tree_sitter_analyzer/query_loader.md#get_query_loader), [`include_queries`](../../tree_sitter_analyzer/core/request.md#AnalysisRequest.include_queries), [`include_elements`](../../tree_sitter_analyzer/core/request.md#AnalysisRequest.include_elements)

### `TestBackwardCompatibility`
- def: [`tests/compatibility/test_cross_version_compatibility.py:465`](../../../../../../raw/code/tree-sitter-analyzer/tests/compatibility/test_cross_version_compatibility.py#L465)
- doc: 向后兼容性测试
- signature: `class TestBackwardCompatibility:`
- members:
  - `test_old_analysis_request_creation(self)` — [`L469`](../../../../../../raw/code/tree-sitter-analyzer/tests/compatibility/test_cross_version_compatibility.py#L469) — 测试旧的AnalysisRequest创建方式
  - `test_old_format_types(self)` — [`L504`](../../../../../../raw/code/tree-sitter-analyzer/tests/compatibility/test_cross_version_compatibility.py#L504) — 测试旧的格式类型仍然有效
  - `test_old_query_execution(self)` — [`L487`](../../../../../../raw/code/tree-sitter-analyzer/tests/compatibility/test_cross_version_compatibility.py#L487) — 测试旧的查询执行方式
- uses (calls/refs, reference-scoped): [`AnalysisRequest`](../../tree_sitter_analyzer/core/request.md#AnalysisRequest), [`file_path`](../../tree_sitter_analyzer/core/request.md#AnalysisRequest.file_path), [`QueryExecutor`](../../tree_sitter_analyzer/core/query.md#QueryExecutor), [`language`](../../tree_sitter_analyzer/core/request.md#AnalysisRequest.language), [`format_type`](../../tree_sitter_analyzer/core/request.md#AnalysisRequest.format_type), [`get_available_queries`](../../tree_sitter_analyzer/core/query.md#QueryExecutor.get_available_queries), [`get_query_description`](../../tree_sitter_analyzer/core/query.md#QueryExecutor.get_query_description)

### `TestConfigFileCompatibility`
- def: [`tests/compatibility/test_cross_version_compatibility.py:15`](../../../../../../raw/code/tree-sitter-analyzer/tests/compatibility/test_cross_version_compatibility.py#L15)
- doc: 配置文件兼容性测试
- signature: `class TestConfigFileCompatibility:`
- members:
  - `test_config_file_empty_queries(self, tmp_path)` — [`L87`](../../../../../../raw/code/tree-sitter-analyzer/tests/compatibility/test_cross_version_compatibility.py#L87) — 测试配置文件空查询列表
  - `test_config_file_extra_fields(self, tmp_path)` — [`L53`](../../../../../../raw/code/tree-sitter-analyzer/tests/compatibility/test_cross_version_compatibility.py#L53) — 测试配置文件额外字段
  - `test_config_file_invalid_json(self, tmp_path)` — [`L76`](../../../../../../raw/code/tree-sitter-analyzer/tests/compatibility/test_cross_version_compatibility.py#L76) — 测试配置文件无效JSON
  - `test_config_file_missing_fields(self, tmp_path)` — [`L39`](../../../../../../raw/code/tree-sitter-analyzer/tests/compatibility/test_cross_version_compatibility.py#L39) — 测试配置文件缺失字段
  - `test_config_file_multiple_languages(self, tmp_path)` — [`L99`](../../../../../../raw/code/tree-sitter-analyzer/tests/compatibility/test_cross_version_compatibility.py#L99) — 测试多语言配置文件
  - `test_config_file_syntax_valid(self, tmp_path)` — [`L19`](../../../../../../raw/code/tree-sitter-analyzer/tests/compatibility/test_cross_version_compatibility.py#L19) — 测试配置文件语法有效性

### `TestDataFormatCompatibility`
- def: [`tests/compatibility/test_cross_version_compatibility.py:275`](../../../../../../raw/code/tree-sitter-analyzer/tests/compatibility/test_cross_version_compatibility.py#L275)
- doc: 数据格式兼容性测试
- signature: `class TestDataFormatCompatibility:`
- members:
  - `test_csv_format_compatibility(self, tmp_path)` — [`L379`](../../../../../../raw/code/tree-sitter-analyzer/tests/compatibility/test_cross_version_compatibility.py#L379) — 测试CSV格式兼容性
  - `test_json_format_compatibility(self, tmp_path)` — [`L279`](../../../../../../raw/code/tree-sitter-analyzer/tests/compatibility/test_cross_version_compatibility.py#L279) — 测试JSON格式兼容性
  - `test_json_format_with_arrays(self, tmp_path)` — [`L335`](../../../../../../raw/code/tree-sitter-analyzer/tests/compatibility/test_cross_version_compatibility.py#L335) — 测试JSON数组格式兼容性
  - `test_json_format_with_nested_structures(self, tmp_path)` — [`L304`](../../../../../../raw/code/tree-sitter-analyzer/tests/compatibility/test_cross_version_compatibility.py#L304) — 测试嵌套JSON结构兼容性
  - `test_toon_format_compatibility(self, tmp_path)` — [`L355`](../../../../../../raw/code/tree-sitter-analyzer/tests/compatibility/test_cross_version_compatibility.py#L355) — 测试Toon格式兼容性

### `TestForwardCompatibility`
- def: [`tests/compatibility/test_cross_version_compatibility.py:517`](../../../../../../raw/code/tree-sitter-analyzer/tests/compatibility/test_cross_version_compatibility.py#L517)
- doc: 向前兼容性测试
- signature: `class TestForwardCompatibility:`
- members:
  - `test_new_format_types_accepted(self)` — [`L538`](../../../../../../raw/code/tree-sitter-analyzer/tests/compatibility/test_cross_version_compatibility.py#L538) — 测试新格式类型被接受
  - `test_new_parameters_accepted(self)` — [`L521`](../../../../../../raw/code/tree-sitter-analyzer/tests/compatibility/test_cross_version_compatibility.py#L521) — 测试新参数被接受
- uses (calls/refs, reference-scoped): [`AnalysisRequest`](../../tree_sitter_analyzer/core/request.md#AnalysisRequest), [`file_path`](../../tree_sitter_analyzer/core/request.md#AnalysisRequest.file_path), [`language`](../../tree_sitter_analyzer/core/request.md#AnalysisRequest.language), [`include_complexity`](../../tree_sitter_analyzer/core/request.md#AnalysisRequest.include_complexity), [`include_details`](../../tree_sitter_analyzer/core/request.md#AnalysisRequest.include_details), [`format_type`](../../tree_sitter_analyzer/core/request.md#AnalysisRequest.format_type), [`include_queries`](../../tree_sitter_analyzer/core/request.md#AnalysisRequest.include_queries), [`include_elements`](../../tree_sitter_analyzer/core/request.md#AnalysisRequest.include_elements)

### `TestPluginInterfaceCompatibility`
- def: [`tests/compatibility/test_cross_version_compatibility.py:206`](../../../../../../raw/code/tree-sitter-analyzer/tests/compatibility/test_cross_version_compatibility.py#L206)
- doc: 插件接口兼容性测试
- signature: `class TestPluginInterfaceCompatibility:`
- members:
  - `test_java_plugin_interface(self)` — [`L238`](../../../../../../raw/code/tree-sitter-analyzer/tests/compatibility/test_cross_version_compatibility.py#L238) — 测试Java插件接口
  - `test_javascript_plugin_interface(self)` — [`L257`](../../../../../../raw/code/tree-sitter-analyzer/tests/compatibility/test_cross_version_compatibility.py#L257) — 测试JavaScript插件接口
  - `test_plugin_base_interface(self)` — [`L210`](../../../../../../raw/code/tree-sitter-analyzer/tests/compatibility/test_cross_version_compatibility.py#L210) — 测试插件基类接口
  - `test_python_plugin_interface(self)` — [`L219`](../../../../../../raw/code/tree-sitter-analyzer/tests/compatibility/test_cross_version_compatibility.py#L219) — 测试Python插件接口
- uses (calls/refs, reference-scoped): [`LanguagePlugin`](../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin), [`PythonPlugin`](../../tree_sitter_analyzer/languages/python_plugin/plugin.md#PythonPlugin), [`JavaPlugin`](../../tree_sitter_analyzer/languages/java_plugin.md#JavaPlugin), [`JavaScriptPlugin`](../../tree_sitter_analyzer/languages/javascript_plugin/plugin.md#JavaScriptPlugin), [`get_queries`](../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin.get_queries), [`get_language_name`](../../tree_sitter_analyzer/languages/javascript_plugin/plugin.md#JavaScriptPlugin.get_language_name), [`get_language_name`](../../tree_sitter_analyzer/languages/python_plugin/plugin.md#PythonPlugin.get_language_name), [`get_language_name`](../../tree_sitter_analyzer/languages/java_plugin.md#JavaPlugin.get_language_name)

### `TestQueryFileCompatibility`
- def: [`tests/compatibility/test_cross_version_compatibility.py:123`](../../../../../../raw/code/tree-sitter-analyzer/tests/compatibility/test_cross_version_compatibility.py#L123)
- doc: 查询文件兼容性测试
- signature: `class TestQueryFileCompatibility:`
- members:
  - `test_query_file_invalid_syntax(self, tmp_path)` — [`L185`](../../../../../../raw/code/tree-sitter-analyzer/tests/compatibility/test_cross_version_compatibility.py#L185) — 测试查询文件无效语法
  - `test_query_file_missing_captures(self, tmp_path)` — [`L147`](../../../../../../raw/code/tree-sitter-analyzer/tests/compatibility/test_cross_version_compatibility.py#L147) — 测试查询文件缺失captures
  - `test_query_file_multiple_queries(self, tmp_path)` — [`L162`](../../../../../../raw/code/tree-sitter-analyzer/tests/compatibility/test_cross_version_compatibility.py#L162) — 测试查询文件多个查询
  - `test_query_file_valid_syntax(self, tmp_path)` — [`L127`](../../../../../../raw/code/tree-sitter-analyzer/tests/compatibility/test_cross_version_compatibility.py#L127) — 测试查询文件语法有效性
  - `test_query_loader_loads_files(self)` — [`L194`](../../../../../../raw/code/tree-sitter-analyzer/tests/compatibility/test_cross_version_compatibility.py#L194) — 测试查询加载器加载文件
- uses (calls/refs, reference-scoped): [`get_query_loader`](../../tree_sitter_analyzer/query_loader.md#get_query_loader), [`get_all_queries_for_language`](../../tree_sitter_analyzer/query_loader.md#QueryLoader.get_all_queries_for_language)

