---
title: 'Module: tests/unit/core/test_output.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_output.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_output`/
symbols:
  TestOutputManagerModes.test_quiet_mode: TestOutputManagerModes#test_quiet_mode().
  TestOutputManagerInit.test_output_manager_initialization: TestOutputManagerInit#test_output_manager_initialization().
  TestOutputManagerCallableFormatter.test_data_with_callable_formatter: TestOutputManagerCallableFormatter#test_data_with_callable_formatter().
  TestOutputManagerCallableFormatter.test_data_with_non_callable_formatter: TestOutputManagerCallableFormatter#test_data_with_non_callable_formatter().
  TestOutputManagerModes.test_json_output_mode: TestOutputManagerModes#test_json_output_mode().
  TestOutputFormatValidator.test_single_format_parameter_valid: TestOutputFormatValidator#test_single_format_parameter_valid().
  TestOutputFormatValidator.test_no_format_parameter_valid: TestOutputFormatValidator#test_no_format_parameter_valid().
  TestOutputFormatValidator.test_multiple_format_parameters_raises_error: TestOutputFormatValidator#test_multiple_format_parameters_raises_error().
  TestOutputFormatValidator.test_error_message_contains_token_guidance: TestOutputFormatValidator#test_error_message_contains_token_guidance().
  TestOutputFormatValidator.test_get_active_format: TestOutputFormatValidator#test_get_active_format().
  TestOutputFormatValidator.test_get_default_validator: TestOutputFormatValidator#test_get_default_validator().
  TestOutputFormatValidator.test_false_values_ignored: TestOutputFormatValidator#test_false_values_ignored().
  TestOutputFormatValidator.test_language_detection: TestOutputFormatValidator#test_language_detection().
  TestOutputManagerQueryResultSingular.test_query_result_quiet_mode: TestOutputManagerQueryResultSingular#test_query_result_quiet_mode().
  TestOutputManagerToonDataHandling.test_data_toon_format_with_toon_content: TestOutputManagerToonDataHandling#test_data_toon_format_with_toon_content().
  TestOutputManagerToonDataHandling.test_data_json_format_with_toon_content: TestOutputManagerToonDataHandling#test_data_json_format_with_toon_content().
  TestOutputManagerCallableFormatter.test_data_unregistered_format_falls_back: TestOutputManagerCallableFormatter#test_data_unregistered_format_falls_back().
  TestGetOutputManager.test_get_output_manager_returns_instance: TestGetOutputManager#test_get_output_manager_returns_instance().
  output_manager: output_manager().
  TestModuleLevelFunctions.test_output_info_function: TestModuleLevelFunctions#test_output_info_function().
  TestModuleLevelFunctions.test_output_warning_function: TestModuleLevelFunctions#test_output_warning_function().
  TestModuleLevelFunctions.test_output_error_function: TestModuleLevelFunctions#test_output_error_function().
  TestModuleLevelFunctions.test_output_success_function: TestModuleLevelFunctions#test_output_success_function().
  TestModuleLevelFunctions.test_output_json_function: TestModuleLevelFunctions#test_output_json_function().
  TestModuleLevelFunctions.test_output_data_function: TestModuleLevelFunctions#test_output_data_function().
  TestModuleLevelFunctions.test_output_list_function: TestModuleLevelFunctions#test_output_list_function().
  TestModuleLevelFunctions.test_output_section_function: TestModuleLevelFunctions#test_output_section_function().
  TestSpecializedOutputFunctions.test_output_statistics: TestSpecializedOutputFunctions#test_output_statistics().
  TestSpecializedOutputFunctions.test_output_languages: TestSpecializedOutputFunctions#test_output_languages().
  TestSpecializedOutputFunctions.test_output_queries: TestSpecializedOutputFunctions#test_output_queries().
  TestSpecializedOutputFunctions.test_output_extensions: TestSpecializedOutputFunctions#test_output_extensions().
  TestGetOutputManager.test_output_query_results_module_function: TestGetOutputManager#test_output_query_results_module_function().
  TestOutputManagerInit: TestOutputManagerInit#
  TestOutputManagerBasicOutput: TestOutputManagerBasicOutput#
  TestOutputManagerBasicOutput.test_output_info: TestOutputManagerBasicOutput#test_output_info().
  TestOutputManagerBasicOutput.test_output_warning: TestOutputManagerBasicOutput#test_output_warning().
  TestOutputManagerBasicOutput.test_output_error: TestOutputManagerBasicOutput#test_output_error().
  TestOutputManagerBasicOutput.test_output_success: TestOutputManagerBasicOutput#test_output_success().
  TestOutputManagerBasicOutput.test_output_json: TestOutputManagerBasicOutput#test_output_json().
  TestOutputManagerBasicOutput.test_output_section: TestOutputManagerBasicOutput#test_output_section().
  TestOutputManagerDataOutput: TestOutputManagerDataOutput#
  TestOutputManagerDataOutput.test_output_data_dict: TestOutputManagerDataOutput#test_output_data_dict().
  TestOutputManagerDataOutput.test_output_data_list: TestOutputManagerDataOutput#test_output_data_list().
  TestOutputManagerDataOutput.test_output_data_string: TestOutputManagerDataOutput#test_output_data_string().
  TestOutputManagerQueryResults: TestOutputManagerQueryResults#
  TestOutputManagerQueryResults.test_output_query_results: TestOutputManagerQueryResults#test_output_query_results().
  TestOutputManagerModes: TestOutputManagerModes#
  TestModuleLevelFunctions: TestModuleLevelFunctions#
  TestSpecializedOutputFunctions: TestSpecializedOutputFunctions#
  TestOutputManagerEdgeCases: TestOutputManagerEdgeCases#
  TestOutputManagerEdgeCases.test_output_manager_with_none_data: TestOutputManagerEdgeCases#test_output_manager_with_none_data().
  TestOutputManagerEdgeCases.test_output_empty_collections: TestOutputManagerEdgeCases#test_output_empty_collections().
  TestOutputManagerEdgeCases.test_output_complex_nested_data: TestOutputManagerEdgeCases#test_output_complex_nested_data().
  TestOutputFormatValidator: TestOutputFormatValidator#
  TestOutputManagerQueryResultSingular: TestOutputManagerQueryResultSingular#
  TestOutputManagerQueryResultSingular.test_query_result_prints_details: TestOutputManagerQueryResultSingular#test_query_result_prints_details().
  TestOutputManagerQueryResultSingular.test_query_result_no_content: TestOutputManagerQueryResultSingular#test_query_result_no_content().
  TestOutputManagerListWithTitle: TestOutputManagerListWithTitle#
  TestOutputManagerListWithTitle.test_output_list_with_title: TestOutputManagerListWithTitle#test_output_list_with_title().
  TestOutputManagerAliasMethods: TestOutputManagerAliasMethods#
  TestOutputManagerAliasMethods.test_output_languages_delegates: TestOutputManagerAliasMethods#test_output_languages_delegates().
  TestOutputManagerAliasMethods.test_output_queries_delegates: TestOutputManagerAliasMethods#test_output_queries_delegates().
  TestOutputManagerToonDataHandling: TestOutputManagerToonDataHandling#
  TestOutputManagerCallableFormatter: TestOutputManagerCallableFormatter#
  TestGetOutputManager: TestGetOutputManager#
---
# Module: [`tests/unit/core/test_output.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_output.py)

## Classes
### `TestGetOutputManager`
- def: [`tests/unit/core/test_output.py:679`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_output.py#L679)
- doc: Test module-level get_output_manager
- signature: `class TestGetOutputManager:`
- members:
  - `test_get_output_manager_returns_instance(self)` — [`L682`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_output.py#L682)
  - `test_output_query_results_module_function(self, monkeypatch)` — [`L688`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_output.py#L688)
- uses (calls/refs, reference-scoped): [`OutputManager`](../../../tree_sitter_analyzer/output_manager.md#OutputManager), [`get_output_manager`](../../../tree_sitter_analyzer/output_manager.md#get_output_manager), [`output_query_results`](../../../tree_sitter_analyzer/output_manager.md#output_query_results)

### `TestModuleLevelFunctions`
- def: [`tests/unit/core/test_output.py:233`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_output.py#L233)
- doc: 模块级别便捷函数测试
- signature: `class TestModuleLevelFunctions:`
- members:
  - `test_output_data_function(self, monkeypatch)` — [`L283`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_output.py#L283) — Test module-level output_data function
  - `test_output_error_function(self, monkeypatch)` — [`L254`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_output.py#L254) — Test module-level output_error function
  - `test_output_info_function(self, monkeypatch)` — [`L236`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_output.py#L236) — Test module-level output_info function — goes to stderr (Q2).
  - `test_output_json_function(self, monkeypatch)` — [`L272`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_output.py#L272) — Test module-level output_json function
  - `test_output_list_function(self, monkeypatch)` — [`L291`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_output.py#L291) — Test module-level output_list function
  - `test_output_section_function(self, monkeypatch)` — [`L299`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_output.py#L299) — Test module-level output_section function
  - `test_output_success_function(self, monkeypatch)` — [`L262`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_output.py#L262) — Test module-level output_success function — goes to stderr (Q2).
  - `test_output_warning_function(self, monkeypatch)` — [`L246`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_output.py#L246) — Test module-level output_warning function
- uses (calls/refs, reference-scoped): [`output_data`](../../../tree_sitter_analyzer/output_manager.md#output_data), [`output_error`](../../../tree_sitter_analyzer/output_manager.md#output_error), [`output_info`](../../../tree_sitter_analyzer/output_manager.md#output_info), [`output_json`](../../../tree_sitter_analyzer/output_manager.md#output_json), [`output_list`](../../../tree_sitter_analyzer/output_manager.md#output_list), [`output_section`](../../../tree_sitter_analyzer/output_manager.md#output_section), [`output_success`](../../../tree_sitter_analyzer/output_manager.md#output_success), [`output_warning`](../../../tree_sitter_analyzer/output_manager.md#output_warning)

### `TestOutputFormatValidator`
- def: [`tests/unit/core/test_output.py:419`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_output.py#L419)
- doc: OutputFormatValidator 测试
- signature: `class TestOutputFormatValidator:`
- members:
  - `test_error_message_contains_token_guidance(self)` — [`L469`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_output.py#L469) — Test that error messages include token efficiency guidance.
  - `test_false_values_ignored(self)` — [`L512`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_output.py#L512) — Test that False values are ignored (not treated as specified).
  - `test_get_active_format(self)` — [`L486`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_output.py#L486) — Test getting the active format from arguments.
  - `test_get_default_validator(self)` — [`L503`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_output.py#L503) — Test getting the default validator instance.
  - `test_language_detection(self)` — [`L535`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_output.py#L535) — Test language detection mechanism.
  - `test_multiple_format_parameters_raises_error(self)` — [`L439`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_output.py#L439) — Test that multiple format parameters raise ValueError.
  - `test_no_format_parameter_valid(self)` — [`L433`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_output.py#L433) — Test that no format parameter is valid (normal mode).
  - `test_single_format_parameter_valid(self)` — [`L422`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_output.py#L422) — Test that single format parameter is valid.
- uses (calls/refs, reference-scoped): [`OutputFormatValidator`](../../../tree_sitter_analyzer/mcp/tools/output_format_validator.md#OutputFormatValidator), [`validate_output_format_exclusion`](../../../tree_sitter_analyzer/mcp/tools/output_format_validator.md#OutputFormatValidator.validate_output_format_exclusion), [`get_active_format`](../../../tree_sitter_analyzer/mcp/tools/output_format_validator.md#OutputFormatValidator.get_active_format), [`get_default_validator`](../../../tree_sitter_analyzer/mcp/tools/output_format_validator.md#get_default_validator), [`_detect_language`](../../../tree_sitter_analyzer/mcp/tools/output_format_validator.md#OutputFormatValidator._detect_language)

### `TestOutputManagerAliasMethods`
- def: [`tests/unit/core/test_output.py:605`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_output.py#L605)
- doc: Test alias/delegate methods that forward to other methods
- signature: `class TestOutputManagerAliasMethods:`
- members:
  - `test_output_languages_delegates(self, monkeypatch, output_manager)` — [`L608`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_output.py#L608)
  - `test_output_queries_delegates(self, monkeypatch, output_manager)` — [`L616`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_output.py#L616)

### `TestOutputManagerBasicOutput`
- def: [`tests/unit/core/test_output.py:61`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_output.py#L61)
- doc: OutputManager 基本输出测试
- signature: `class TestOutputManagerBasicOutput:`
- members:
  - `test_output_error(self, monkeypatch, output_manager)` — [`L88`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_output.py#L88) — Test error output
  - `test_output_info(self, monkeypatch, output_manager)` — [`L64`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_output.py#L64) — Test info output goes to stderr.
  - `test_output_json(self, monkeypatch, output_manager)` — [`L109`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_output.py#L109) — Test JSON output
  - `test_output_section(self, monkeypatch, output_manager)` — [`L122`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_output.py#L122) — Test section output
  - `test_output_success(self, monkeypatch, output_manager)` — [`L96`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_output.py#L96) — Test success output goes to stderr.
  - `test_output_warning(self, monkeypatch, output_manager)` — [`L80`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_output.py#L80) — Test warning output

### `TestOutputManagerCallableFormatter`
- def: [`tests/unit/core/test_output.py:648`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_output.py#L648)
- doc: Test callable formatter and fallback paths
- signature: `class TestOutputManagerCallableFormatter:`
- members:
  - `test_data_unregistered_format_falls_back(self, monkeypatch)` — [`L670`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_output.py#L670)
  - `test_data_with_callable_formatter(self, monkeypatch)` — [`L651`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_output.py#L651)
  - `test_data_with_non_callable_formatter(self, monkeypatch)` — [`L660`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_output.py#L660)
- uses (calls/refs, reference-scoped): [`OutputManager`](../../../tree_sitter_analyzer/output_manager.md#OutputManager), [`data`](../../../tree_sitter_analyzer/output_manager.md#OutputManager.data), [`_formatter_registry`](../../../tree_sitter_analyzer/output_manager.md#OutputManager._formatter_registry)

### `TestOutputManagerDataOutput`
- def: [`tests/unit/core/test_output.py:131`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_output.py#L131)
- doc: OutputManager 数据输出测试
- signature: `class TestOutputManagerDataOutput:`
- members:
  - `test_output_data_dict(self, monkeypatch, output_manager)` — [`L134`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_output.py#L134) — Test data output with dictionary
  - `test_output_data_list(self, monkeypatch, output_manager)` — [`L147`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_output.py#L147) — Test data output with list
  - `test_output_data_string(self, monkeypatch, output_manager)` — [`L159`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_output.py#L159) — Test data output with string

### `TestOutputManagerEdgeCases`
- def: [`tests/unit/core/test_output.py:370`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_output.py#L370)
- doc: 边缘情况测试
- signature: `class TestOutputManagerEdgeCases:`
- members:
  - `test_output_complex_nested_data(self, monkeypatch, output_manager)` — [`L391`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_output.py#L391) — Test output with complex nested data structures
  - `test_output_empty_collections(self, monkeypatch, output_manager)` — [`L379`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_output.py#L379) — Test output with empty collections
  - `test_output_manager_with_none_data(self, output_manager)` — [`L373`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_output.py#L373) — Test output manager handles None data gracefully

### `TestOutputManagerInit`
- def: [`tests/unit/core/test_output.py:45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_output.py#L45)
- doc: OutputManager 初始化测试
- signature: `class TestOutputManagerInit:`
- members:
  - `test_output_manager_initialization(self)` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_output.py#L48) — Test OutputManager initializes correctly
- uses (calls/refs, reference-scoped): [`OutputManager`](../../../tree_sitter_analyzer/output_manager.md#OutputManager), [`quiet`](../../../tree_sitter_analyzer/output_manager.md#OutputManager.quiet), [`json_output`](../../../tree_sitter_analyzer/output_manager.md#OutputManager.json_output)

### `TestOutputManagerListWithTitle`
- def: [`tests/unit/core/test_output.py:592`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_output.py#L592)
- doc: Test output_list with title parameter
- signature: `class TestOutputManagerListWithTitle:`
- members:
  - `test_output_list_with_title(self, monkeypatch, output_manager)` — [`L595`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_output.py#L595)

### `TestOutputManagerModes`
- def: [`tests/unit/core/test_output.py:198`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_output.py#L198)
- doc: OutputManager 模式测试
- signature: `class TestOutputManagerModes:`
- members:
  - `test_json_output_mode(self, monkeypatch)` — [`L216`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_output.py#L216) — Test JSON output mode
  - `test_quiet_mode(self, monkeypatch)` — [`L201`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_output.py#L201) — Test quiet mode suppresses output
- uses (calls/refs, reference-scoped): [`OutputManager`](../../../tree_sitter_analyzer/output_manager.md#OutputManager), [`output_data`](../../../tree_sitter_analyzer/output_manager.md#OutputManager.output_data), [`output_info`](../../../tree_sitter_analyzer/output_manager.md#OutputManager.output_info), [`output_success`](../../../tree_sitter_analyzer/output_manager.md#OutputManager.output_success), [`output_warning`](../../../tree_sitter_analyzer/output_manager.md#OutputManager.output_warning)

### `TestOutputManagerQueryResultSingular`
- def: [`tests/unit/core/test_output.py:549`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_output.py#L549)
- doc: Test the singular query_result method (not output_query_results)
- signature: `class TestOutputManagerQueryResultSingular:`
- members:
  - `test_query_result_no_content(self, monkeypatch, output_manager)` — [`L569`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_output.py#L569)
  - `test_query_result_prints_details(self, monkeypatch, output_manager)` — [`L552`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_output.py#L552)
  - `test_query_result_quiet_mode(self, monkeypatch)` — [`L584`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_output.py#L584)
- uses (calls/refs, reference-scoped): [`OutputManager`](../../../tree_sitter_analyzer/output_manager.md#OutputManager), [`query_result`](../../../tree_sitter_analyzer/output_manager.md#OutputManager.query_result)

### `TestOutputManagerQueryResults`
- def: [`tests/unit/core/test_output.py:168`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_output.py#L168)
- doc: OutputManager 查询结果输出测试
- signature: `class TestOutputManagerQueryResults:`
- members:
  - `test_output_query_results(self, monkeypatch, output_manager)` — [`L171`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_output.py#L171) — Test query results output

### `TestOutputManagerToonDataHandling`
- def: [`tests/unit/core/test_output.py:625`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_output.py#L625)
- doc: Test TOON-formatted data handling in data() method
- signature: `class TestOutputManagerToonDataHandling:`
- members:
  - `test_data_json_format_with_toon_content(self, monkeypatch)` — [`L637`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_output.py#L637)
  - `test_data_toon_format_with_toon_content(self, monkeypatch)` — [`L628`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_output.py#L628)
- uses (calls/refs, reference-scoped): [`OutputManager`](../../../tree_sitter_analyzer/output_manager.md#OutputManager), [`data`](../../../tree_sitter_analyzer/output_manager.md#OutputManager.data)

### `TestSpecializedOutputFunctions`
- def: [`tests/unit/core/test_output.py:308`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_output.py#L308)
- doc: 专用输出函数测试
- signature: `class TestSpecializedOutputFunctions:`
- members:
  - `test_output_extensions(self, monkeypatch)` — [`L350`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_output.py#L350) — Test extensions output
  - `test_output_languages(self, monkeypatch)` — [`L323`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_output.py#L323) — Test languages output
  - `test_output_queries(self, monkeypatch)` — [`L334`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_output.py#L334) — Test queries output
  - `test_output_statistics(self, monkeypatch)` — [`L311`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_output.py#L311) — Test statistics output
- uses (calls/refs, reference-scoped): [`output_extensions`](../../../tree_sitter_analyzer/output_manager.md#output_extensions), [`output_languages`](../../../tree_sitter_analyzer/output_manager.md#output_languages), [`output_queries`](../../../tree_sitter_analyzer/output_manager.md#output_queries), [`output_statistics`](../../../tree_sitter_analyzer/output_manager.md#output_statistics)

## Functions
- `output_manager()` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_output.py#L35) — Fixture for OutputManager instance

