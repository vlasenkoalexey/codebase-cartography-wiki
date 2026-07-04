---
title: 'Module: tests/unit/utils/test_utils_init.py'
type: catalog
provenance: extracted
module: tests/unit/utils/test_utils_init.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.utils.test_utils_init`/Test
symbols:
  TestFunctionTypes.test_logging_functions_callable: FunctionTypes#test_logging_functions_callable().
  TestModuleExports.test_logging_function_exports: ModuleExports#test_logging_function_exports().
  TestModuleExports.test_logging_utility_exports: ModuleExports#test_logging_utility_exports().
  TestModuleExports.test_tree_sitter_compat_exports: ModuleExports#test_tree_sitter_compat_exports().
  TestModuleExports.test_logging_class_exports: ModuleExports#test_logging_class_exports().
  TestImportability.test_direct_import_from_utils: Importability#test_direct_import_from_utils().
  TestModuleExports.test_logger_instance_exports: ModuleExports#test_logger_instance_exports().
  TestFunctionTypes.test_tree_sitter_compat_callables: FunctionTypes#test_tree_sitter_compat_callables().
  TestClassTypes.test_tree_sitter_query_compat_is_class: ClassTypes#test_tree_sitter_query_compat_is_class().
  TestClassTypes.test_quiet_mode_is_class: ClassTypes#test_quiet_mode_is_class().
  TestClassTypes.test_logging_context_is_class: ClassTypes#test_logging_context_is_class().
  TestClassTypes.test_safe_stream_handler_is_class: ClassTypes#test_safe_stream_handler_is_class().
  TestLoggerInstances.test_logger_is_logger_instance: LoggerInstances#test_logger_is_logger_instance().
  TestLoggerInstances.test_perf_logger_is_logger_instance: LoggerInstances#test_perf_logger_is_logger_instance().
  TestLoggerInstances.test_logger_has_name: LoggerInstances#test_logger_has_name().
  TestLoggerInstances.test_perf_logger_has_name: LoggerInstances#test_perf_logger_has_name().
  TestModuleAttributes.test_module_has_all_attribute: ModuleAttributes#test_module_has_all_attribute().
  TestModuleAttributes.test_all_attribute_completeness: ModuleAttributes#test_all_attribute_completeness().
  TestNoExtraExports.test_all_public_items_in_all: NoExtraExports#test_all_public_items_in_all().
  TestFunctionalityAvailability.test_log_info_works: FunctionalityAvailability#test_log_info_works().
  TestFunctionalityAvailability.test_log_error_works: FunctionalityAvailability#test_log_error_works().
  TestFunctionalityAvailability.test_log_warning_works: FunctionalityAvailability#test_log_warning_works().
  TestFunctionalityAvailability.test_log_debug_works: FunctionalityAvailability#test_log_debug_works().
  TestFunctionalityAvailability.test_safe_print_works: FunctionalityAvailability#test_safe_print_works().
  TestClassInstantiation.test_quiet_mode_instantiation: ClassInstantiation#test_quiet_mode_instantiation().
  TestClassInstantiation.test_logging_context_instantiation: ClassInstantiation#test_logging_context_instantiation().
  TestClassInstantiation.test_tree_sitter_query_compat_instantiation: ClassInstantiation#test_tree_sitter_query_compat_instantiation().
  TestModuleExports: ModuleExports#
  TestImportability: Importability#
  TestImportability.test_all_exports_importable: Importability#test_all_exports_importable().
  TestFunctionTypes: FunctionTypes#
  TestClassTypes: ClassTypes#
  TestLoggerInstances: LoggerInstances#
  TestModuleAttributes: ModuleAttributes#
  TestImportSources: ImportSources#
  TestImportSources.test_logging_imports_from_logging_module: ImportSources#test_logging_imports_from_logging_module().
  TestImportSources.test_compat_imports_from_compat_module: ImportSources#test_compat_imports_from_compat_module().
  TestModuleDocstring: ModuleDocstring#
  TestModuleDocstring.test_module_has_docstring: ModuleDocstring#test_module_has_docstring().
  TestModuleDocstring.test_docstring_describes_purpose: ModuleDocstring#test_docstring_describes_purpose().
  TestNoExtraExports: NoExtraExports#
  TestImportPerformance: ImportPerformance#
  TestImportPerformance.test_import_does_not_raise: ImportPerformance#test_import_does_not_raise().
  TestImportPerformance.test_reimport_is_safe: ImportPerformance#test_reimport_is_safe().
  TestFunctionalityAvailability: FunctionalityAvailability#
  TestClassInstantiation: ClassInstantiation#
---
# Module: [`tests/unit/utils/test_utils_init.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_init.py)

## Classes
### `TestClassInstantiation`
- def: [`tests/unit/utils/test_utils_init.py:327`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_init.py#L327)
- doc: Test that exported classes can be instantiated.
- signature: `class TestClassInstantiation:`
- members:
  - `test_logging_context_instantiation(self)` — [`L336`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_init.py#L336) — Test LoggingContext can be instantiated.
  - `test_quiet_mode_instantiation(self)` — [`L330`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_init.py#L330) — Test QuietMode can be instantiated.
  - `test_tree_sitter_query_compat_instantiation(self)` — [`L342`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_init.py#L342) — Test TreeSitterQueryCompat can be instantiated.
- uses (calls/refs, reference-scoped): [`TreeSitterQueryCompat`](../../../tree_sitter_analyzer/utils/tree_sitter_compat.md#TreeSitterQueryCompat), [`LoggingContext`](../../../tree_sitter_analyzer/utils/logging.md#LoggingContext), [`QuietMode`](../../../tree_sitter_analyzer/utils/logging.md#QuietMode)

### `TestClassTypes`
- def: [`tests/unit/utils/test_utils_init.py:119`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_init.py#L119)
- doc: Test that exported classes are proper classes.
- signature: `class TestClassTypes:`
- members:
  - `test_logging_context_is_class(self)` — [`L130`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_init.py#L130) — Test LoggingContext is a class.
  - `test_quiet_mode_is_class(self)` — [`L126`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_init.py#L126) — Test QuietMode is a class.
  - `test_safe_stream_handler_is_class(self)` — [`L134`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_init.py#L134) — Test SafeStreamHandler is a class.
  - `test_tree_sitter_query_compat_is_class(self)` — [`L122`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_init.py#L122) — Test TreeSitterQueryCompat is a class.
- uses (calls/refs, reference-scoped): [`TreeSitterQueryCompat`](../../../tree_sitter_analyzer/utils/tree_sitter_compat.md#TreeSitterQueryCompat), [`LoggingContext`](../../../tree_sitter_analyzer/utils/logging.md#LoggingContext), [`SafeStreamHandler`](../../../tree_sitter_analyzer/utils/logging.md#SafeStreamHandler), [`QuietMode`](../../../tree_sitter_analyzer/utils/logging.md#QuietMode)

### `TestFunctionTypes`
- def: [`tests/unit/utils/test_utils_init.py:96`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_init.py#L96)
- doc: Test that exported functions are callable.
- signature: `class TestFunctionTypes:`
- members:
  - `test_logging_functions_callable(self)` — [`L104`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_init.py#L104) — Test logging functions are callable.
  - `test_tree_sitter_compat_callables(self)` — [`L99`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_init.py#L99) — Test tree-sitter compatibility functions are callable.
- uses (calls/refs, reference-scoped): [`log_debug`](../../../tree_sitter_analyzer/utils/logging.md#log_debug), [`log_error`](../../../tree_sitter_analyzer/utils/logging.md#log_error), [`setup_logger`](../../../tree_sitter_analyzer/utils/logging.md#setup_logger), [`log_warning`](../../../tree_sitter_analyzer/utils/logging.md#log_warning), [`get_node_text_safe`](../../../tree_sitter_analyzer/utils/tree_sitter_compat.md#get_node_text_safe), [`log_info`](../../../tree_sitter_analyzer/utils/logging.md#log_info), [`safe_print`](../../../tree_sitter_analyzer/utils/logging.md#safe_print), [`log_performance`](../../../tree_sitter_analyzer/utils/logging.md#log_performance), [`create_performance_logger`](../../../tree_sitter_analyzer/utils/logging.md#create_performance_logger), [`log_api_info`](../../../tree_sitter_analyzer/utils/tree_sitter_compat.md#log_api_info), [`setup_performance_logger`](../../../tree_sitter_analyzer/utils/logging.md#setup_performance_logger), [`suppress_output`](../../../tree_sitter_analyzer/utils/logging.md#suppress_output), [`setup_safe_logging_shutdown`](../../../tree_sitter_analyzer/utils/logging.md#setup_safe_logging_shutdown)

### `TestFunctionalityAvailability`
- def: [`tests/unit/utils/test_utils_init.py:298`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_init.py#L298)
- doc: Test that exported functionality works.
- signature: `class TestFunctionalityAvailability:`
- members:
  - `test_log_debug_works(self)` — [`L316`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_init.py#L316) — Test that log_debug can be called.
  - `test_log_error_works(self)` — [`L306`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_init.py#L306) — Test that log_error can be called.
  - `test_log_info_works(self)` — [`L301`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_init.py#L301) — Test that log_info can be called.
  - `test_log_warning_works(self)` — [`L311`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_init.py#L311) — Test that log_warning can be called.
  - `test_safe_print_works(self)` — [`L321`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_init.py#L321) — Test that safe_print can be called.
- uses (calls/refs, reference-scoped): [`log_debug`](../../../tree_sitter_analyzer/utils/logging.md#log_debug), [`log_error`](../../../tree_sitter_analyzer/utils/logging.md#log_error), [`log_warning`](../../../tree_sitter_analyzer/utils/logging.md#log_warning), [`log_info`](../../../tree_sitter_analyzer/utils/logging.md#log_info), [`safe_print`](../../../tree_sitter_analyzer/utils/logging.md#safe_print)

### `TestImportPerformance`
- def: [`tests/unit/utils/test_utils_init.py:275`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_init.py#L275)
- doc: Test that imports don't have side effects.
- signature: `class TestImportPerformance:`
- members:
  - `test_import_does_not_raise(self)` — [`L278`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_init.py#L278) — Test that importing the module doesn't raise exceptions.
  - `test_reimport_is_safe(self)` — [`L285`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_init.py#L285) — Test that reimporting the module is safe.

### `TestImportSources`
- def: [`tests/unit/utils/test_utils_init.py:206`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_init.py#L206)
- doc: Test that imports come from correct sources.
- signature: `class TestImportSources:`
- members:
  - `test_compat_imports_from_compat_module(self)` — [`L217`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_init.py#L217) — Test compat functions come from tree_sitter_compat module.
  - `test_logging_imports_from_logging_module(self)` — [`L209`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_init.py#L209) — Test logging functions come from logging module.

### `TestImportability`
- def: [`tests/unit/utils/test_utils_init.py:70`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_init.py#L70)
- doc: Test that all exports can be imported.
- signature: `class TestImportability:`
- members:
  - `test_all_exports_importable(self)` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_init.py#L73) — Test that all items in __all__ can be imported.
  - `test_direct_import_from_utils(self)` — [`L84`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_init.py#L84) — Test direct import from utils works.
- uses (calls/refs, reference-scoped): [`logger`](../../../tree_sitter_analyzer/utils/logging.md#logger), [`TreeSitterQueryCompat`](../../../tree_sitter_analyzer/utils/tree_sitter_compat.md#TreeSitterQueryCompat), [`log_info`](../../../tree_sitter_analyzer/utils/logging.md#log_info)

### `TestLoggerInstances`
- def: [`tests/unit/utils/test_utils_init.py:139`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_init.py#L139)
- doc: Test logger instance properties.
- signature: `class TestLoggerInstances:`
- members:
  - `test_logger_has_name(self)` — [`L154`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_init.py#L154) — Test logger has a name.
  - `test_logger_is_logger_instance(self)` — [`L142`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_init.py#L142) — Test logger is a Logger instance.
  - `test_perf_logger_has_name(self)` — [`L159`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_init.py#L159) — Test perf_logger has a name.
  - `test_perf_logger_is_logger_instance(self)` — [`L148`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_init.py#L148) — Test perf_logger is a Logger instance.
- uses (calls/refs, reference-scoped): [`logger`](../../../tree_sitter_analyzer/utils/logging.md#logger), [`perf_logger`](../../../tree_sitter_analyzer/utils/logging.md#perf_logger)

### `TestModuleAttributes`
- def: [`tests/unit/utils/test_utils_init.py:165`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_init.py#L165)
- doc: Test module-level attributes.
- signature: `class TestModuleAttributes:`
- members:
  - `test_all_attribute_completeness(self)` — [`L176`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_init.py#L176) — Test __all__ contains expected items.
  - `test_module_has_all_attribute(self)` — [`L168`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_init.py#L168) — Test module has __all__ attribute.
- uses (calls/refs, reference-scoped): [`__all__`](../../../tree_sitter_analyzer/utils/__init__.md#__all__)

### `TestModuleDocstring`
- def: [`tests/unit/utils/test_utils_init.py:226`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_init.py#L226)
- doc: Test module documentation.
- signature: `class TestModuleDocstring:`
- members:
  - `test_docstring_describes_purpose(self)` — [`L236`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_init.py#L236) — Test docstring describes module purpose.
  - `test_module_has_docstring(self)` — [`L229`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_init.py#L229) — Test module has a docstring.

### `TestModuleExports`
- def: [`tests/unit/utils/test_utils_init.py:30`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_init.py#L30)
- doc: Test that all expected exports are available.
- signature: `class TestModuleExports:`
- members:
  - `test_logger_instance_exports(self)` — [`L62`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_init.py#L62) — Test logger instance exports are available.
  - `test_logging_class_exports(self)` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_init.py#L48) — Test logging class exports are available.
  - `test_logging_function_exports(self)` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_init.py#L39) — Test logging function exports are available.
  - `test_logging_utility_exports(self)` — [`L54`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_init.py#L54) — Test logging utility exports are available.
  - `test_tree_sitter_compat_exports(self)` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_init.py#L33) — Test tree-sitter compatibility exports are available.
- uses (calls/refs, reference-scoped): [`log_debug`](../../../tree_sitter_analyzer/utils/logging.md#log_debug), [`log_error`](../../../tree_sitter_analyzer/utils/logging.md#log_error), [`setup_logger`](../../../tree_sitter_analyzer/utils/logging.md#setup_logger), [`log_warning`](../../../tree_sitter_analyzer/utils/logging.md#log_warning), [`logger`](../../../tree_sitter_analyzer/utils/logging.md#logger), [`get_node_text_safe`](../../../tree_sitter_analyzer/utils/tree_sitter_compat.md#get_node_text_safe), [`TreeSitterQueryCompat`](../../../tree_sitter_analyzer/utils/tree_sitter_compat.md#TreeSitterQueryCompat), [`log_info`](../../../tree_sitter_analyzer/utils/logging.md#log_info), [`safe_print`](../../../tree_sitter_analyzer/utils/logging.md#safe_print), [`LoggingContext`](../../../tree_sitter_analyzer/utils/logging.md#LoggingContext), [`SafeStreamHandler`](../../../tree_sitter_analyzer/utils/logging.md#SafeStreamHandler), [`log_performance`](../../../tree_sitter_analyzer/utils/logging.md#log_performance), [`perf_logger`](../../../tree_sitter_analyzer/utils/logging.md#perf_logger), [`QuietMode`](../../../tree_sitter_analyzer/utils/logging.md#QuietMode), [`create_performance_logger`](../../../tree_sitter_analyzer/utils/logging.md#create_performance_logger), [`log_api_info`](../../../tree_sitter_analyzer/utils/tree_sitter_compat.md#log_api_info), [`setup_performance_logger`](../../../tree_sitter_analyzer/utils/logging.md#setup_performance_logger), [`suppress_output`](../../../tree_sitter_analyzer/utils/logging.md#suppress_output), [`setup_safe_logging_shutdown`](../../../tree_sitter_analyzer/utils/logging.md#setup_safe_logging_shutdown)

### `TestNoExtraExports`
- def: [`tests/unit/utils/test_utils_init.py:244`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_init.py#L244)
- doc: Test that no unexpected items are exported.
- signature: `class TestNoExtraExports:`
- members:
  - `test_all_public_items_in_all(self)` — [`L247`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_utils_init.py#L247) — Test that public items (not starting with _) are in __all__.
- uses (calls/refs, reference-scoped): [`__all__`](../../../tree_sitter_analyzer/utils/__init__.md#__all__)

