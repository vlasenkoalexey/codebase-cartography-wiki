---
title: 'Module: tests/unit/test_exceptions_core.py'
type: catalog
provenance: extracted
module: tests/unit/test_exceptions_core.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_exceptions_core`/Test
symbols:
  TestExceptionHierarchy.test_all_inherit_from_base: ExceptionHierarchy#test_all_inherit_from_base().
  TestTreeSitterAnalyzerError.test_message_and_error_code: TreeSitterAnalyzerError#test_message_and_error_code().
  TestTreeSitterAnalyzerError.test_custom_error_code: TreeSitterAnalyzerError#test_custom_error_code().
  TestTreeSitterAnalyzerError.test_default_context_is_empty: TreeSitterAnalyzerError#test_default_context_is_empty().
  TestTreeSitterAnalyzerError.test_custom_context: TreeSitterAnalyzerError#test_custom_context().
  TestTreeSitterAnalyzerError.test_to_dict: TreeSitterAnalyzerError#test_to_dict().
  TestAnalysisError.test_with_file_path_and_language: AnalysisError#test_with_file_path_and_language().
  TestAnalysisError.test_without_optional_fields: AnalysisError#test_without_optional_fields().
  TestParseError.test_with_source_info: ParseError#test_with_source_info().
  TestLanguageNotSupportedError.test_message_includes_language: LanguageNotSupportedError#test_message_includes_language().
  TestPluginError.test_with_plugin_and_operation: PluginError#test_with_plugin_and_operation().
  TestQueryError.test_with_query_details: QueryError#test_with_query_details().
  TestFileHandlingError.test_with_file_and_operation: FileHandlingError#test_with_file_and_operation().
  TestConfigurationError.test_with_config_key_and_value: ConfigurationError#test_with_config_key_and_value().
  TestConfigurationError.test_none_value_not_stored: ConfigurationError#test_none_value_not_stored().
  TestValidationError.test_with_validation_type: ValidationError#test_with_validation_type().
  TestMCPError.test_with_tool_and_resource: MCPError#test_with_tool_and_resource().
  TestExceptionHierarchy.test_all_catchable_as_base: ExceptionHierarchy#test_all_catchable_as_base().
  TestExceptionHierarchy.test_to_dict_includes_concrete_class_name: ExceptionHierarchy#test_to_dict_includes_concrete_class_name().
  TestTreeSitterAnalyzerError.test_is_catchable_as_exception: TreeSitterAnalyzerError#test_is_catchable_as_exception().
  TestLanguageNotSupportedError.test_message_includes_supported_list: LanguageNotSupportedError#test_message_includes_supported_list().
  TestLanguageNotSupportedError.test_without_supported_list: LanguageNotSupportedError#test_without_supported_list().
  TestTreeSitterAnalyzerError: TreeSitterAnalyzerError#
  TestAnalysisError: AnalysisError#
  TestParseError: ParseError#
  TestLanguageNotSupportedError: LanguageNotSupportedError#
  TestPluginError: PluginError#
  TestQueryError: QueryError#
  TestFileHandlingError: FileHandlingError#
  TestConfigurationError: ConfigurationError#
  TestValidationError: ValidationError#
  TestMCPError: MCPError#
  TestExceptionHierarchy: ExceptionHierarchy#
---
# Module: [`tests/unit/test_exceptions_core.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_core.py)

## Classes
### `TestAnalysisError`
- def: [`tests/unit/test_exceptions_core.py:54`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_core.py#L54)
- doc: Tests for AnalysisError.
- signature: `class TestAnalysisError:`
- members:
  - `test_with_file_path_and_language(self)` — [`L57`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_core.py#L57)
  - `test_without_optional_fields(self)` — [`L62`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_core.py#L62)
- uses (calls/refs, reference-scoped): [`context`](../../tree_sitter_analyzer/_exceptions_core.md#TreeSitterAnalyzerError.context), [`AnalysisError`](../../tree_sitter_analyzer/_exceptions_core.md#AnalysisError)

### `TestConfigurationError`
- def: [`tests/unit/test_exceptions_core.py:129`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_core.py#L129)
- doc: Tests for ConfigurationError.
- signature: `class TestConfigurationError:`
- members:
  - `test_none_value_not_stored(self)` — [`L137`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_core.py#L137)
  - `test_with_config_key_and_value(self)` — [`L132`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_core.py#L132)
- uses (calls/refs, reference-scoped): [`context`](../../tree_sitter_analyzer/_exceptions_core.md#TreeSitterAnalyzerError.context), [`ConfigurationError`](../../tree_sitter_analyzer/_exceptions_core.md#ConfigurationError)

### `TestExceptionHierarchy`
- def: [`tests/unit/test_exceptions_core.py:164`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_core.py#L164)
- doc: Tests for exception inheritance.
- signature: `class TestExceptionHierarchy:`
- members:
  - `test_all_catchable_as_base(self)` — [`L181`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_core.py#L181)
  - `test_all_inherit_from_base(self)` — [`L167`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_core.py#L167)
  - `test_to_dict_includes_concrete_class_name(self)` — [`L185`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_core.py#L185)
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerError`](../../tree_sitter_analyzer/_exceptions_core.md#TreeSitterAnalyzerError), [`MCPError`](../../tree_sitter_analyzer/_exceptions_core.md#MCPError), [`AnalysisError`](../../tree_sitter_analyzer/_exceptions_core.md#AnalysisError), [`ValidationError`](../../tree_sitter_analyzer/_exceptions_core.md#ValidationError), [`QueryError`](../../tree_sitter_analyzer/_exceptions_core.md#QueryError), [`FileHandlingError`](../../tree_sitter_analyzer/_exceptions_core.md#FileHandlingError), [`ParseError`](../../tree_sitter_analyzer/_exceptions_core.md#ParseError), [`LanguageNotSupportedError`](../../tree_sitter_analyzer/_exceptions_core.md#LanguageNotSupportedError), [`to_dict`](../../tree_sitter_analyzer/_exceptions_core.md#TreeSitterAnalyzerError.to_dict), [`ConfigurationError`](../../tree_sitter_analyzer/_exceptions_core.md#ConfigurationError), [`PluginError`](../../tree_sitter_analyzer/_exceptions_core.md#PluginError)

### `TestFileHandlingError`
- def: [`tests/unit/test_exceptions_core.py:120`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_core.py#L120)
- doc: Tests for FileHandlingError.
- signature: `class TestFileHandlingError:`
- members:
  - `test_with_file_and_operation(self)` — [`L123`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_core.py#L123)
- uses (calls/refs, reference-scoped): [`context`](../../tree_sitter_analyzer/_exceptions_core.md#TreeSitterAnalyzerError.context), [`FileHandlingError`](../../tree_sitter_analyzer/_exceptions_core.md#FileHandlingError)

### `TestLanguageNotSupportedError`
- def: [`tests/unit/test_exceptions_core.py:77`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_core.py#L77)
- doc: Tests for LanguageNotSupportedError.
- signature: `class TestLanguageNotSupportedError:`
- members:
  - `test_message_includes_language(self)` — [`L80`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_core.py#L80)
  - `test_message_includes_supported_list(self)` — [`L85`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_core.py#L85)
  - `test_without_supported_list(self)` — [`L92`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_core.py#L92)
- uses (calls/refs, reference-scoped): [`context`](../../tree_sitter_analyzer/_exceptions_core.md#TreeSitterAnalyzerError.context), [`LanguageNotSupportedError`](../../tree_sitter_analyzer/_exceptions_core.md#LanguageNotSupportedError)

### `TestMCPError`
- def: [`tests/unit/test_exceptions_core.py:153`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_core.py#L153)
- doc: Tests for MCPError.
- signature: `class TestMCPError:`
- members:
  - `test_with_tool_and_resource(self)` — [`L156`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_core.py#L156)
- uses (calls/refs, reference-scoped): [`context`](../../tree_sitter_analyzer/_exceptions_core.md#TreeSitterAnalyzerError.context), [`MCPError`](../../tree_sitter_analyzer/_exceptions_core.md#MCPError)

### `TestParseError`
- def: [`tests/unit/test_exceptions_core.py:68`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_core.py#L68)
- doc: Tests for ParseError.
- signature: `class TestParseError:`
- members:
  - `test_with_source_info(self)` — [`L71`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_core.py#L71)
- uses (calls/refs, reference-scoped): [`context`](../../tree_sitter_analyzer/_exceptions_core.md#TreeSitterAnalyzerError.context), [`ParseError`](../../tree_sitter_analyzer/_exceptions_core.md#ParseError)

### `TestPluginError`
- def: [`tests/unit/test_exceptions_core.py:97`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_core.py#L97)
- doc: Tests for PluginError.
- signature: `class TestPluginError:`
- members:
  - `test_with_plugin_and_operation(self)` — [`L100`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_core.py#L100)
- uses (calls/refs, reference-scoped): [`context`](../../tree_sitter_analyzer/_exceptions_core.md#TreeSitterAnalyzerError.context), [`PluginError`](../../tree_sitter_analyzer/_exceptions_core.md#PluginError)

### `TestQueryError`
- def: [`tests/unit/test_exceptions_core.py:106`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_core.py#L106)
- doc: Tests for QueryError.
- signature: `class TestQueryError:`
- members:
  - `test_with_query_details(self)` — [`L109`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_core.py#L109)
- uses (calls/refs, reference-scoped): [`context`](../../tree_sitter_analyzer/_exceptions_core.md#TreeSitterAnalyzerError.context), [`QueryError`](../../tree_sitter_analyzer/_exceptions_core.md#QueryError)

### `TestTreeSitterAnalyzerError`
- def: [`tests/unit/test_exceptions_core.py:19`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_core.py#L19)
- doc: Tests for the base exception class.
- signature: `class TestTreeSitterAnalyzerError:`
- members:
  - `test_custom_context(self)` — [`L36`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_core.py#L36)
  - `test_custom_error_code(self)` — [`L28`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_core.py#L28)
  - `test_default_context_is_empty(self)` — [`L32`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_core.py#L32)
  - `test_is_catchable_as_exception(self)` — [`L48`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_core.py#L48)
  - `test_message_and_error_code(self)` — [`L22`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_core.py#L22)
  - `test_to_dict(self)` — [`L40`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_core.py#L40)
- uses (calls/refs, reference-scoped): [`context`](../../tree_sitter_analyzer/_exceptions_core.md#TreeSitterAnalyzerError.context), [`TreeSitterAnalyzerError`](../../tree_sitter_analyzer/_exceptions_core.md#TreeSitterAnalyzerError), [`message`](../../tree_sitter_analyzer/_exceptions_core.md#TreeSitterAnalyzerError.message), [`to_dict`](../../tree_sitter_analyzer/_exceptions_core.md#TreeSitterAnalyzerError.to_dict), [`error_code`](../../tree_sitter_analyzer/_exceptions_core.md#TreeSitterAnalyzerError.error_code)

### `TestValidationError`
- def: [`tests/unit/test_exceptions_core.py:142`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_core.py#L142)
- doc: Tests for ValidationError.
- signature: `class TestValidationError:`
- members:
  - `test_with_validation_type(self)` — [`L145`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_core.py#L145)
- uses (calls/refs, reference-scoped): [`context`](../../tree_sitter_analyzer/_exceptions_core.md#TreeSitterAnalyzerError.context), [`ValidationError`](../../tree_sitter_analyzer/_exceptions_core.md#ValidationError)

