---
title: 'Module: tests/unit/utils/test_logging.py'
type: catalog
provenance: extracted
module: tests/unit/utils/test_logging.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.utils.test_logging`/Test
symbols:
  TestIntegration.test_complete_logging_workflow: Integration#test_complete_logging_workflow().
  TestIntegration.test_quiet_mode_integration: Integration#test_quiet_mode_integration().
  TestIntegration.test_logging_context_integration: Integration#test_logging_context_integration().
  TestSafeStreamHandler.test_emit_stream_no_write: SafeStreamHandler#test_emit_stream_no_write().
  TestLoggingContext.test_init_with_level: LoggingContext#test_init_with_level().
  TestSuppressOutput.test_func: SuppressOutput#test_func().
  TestSafeStreamHandler.test_emit_normal: SafeStreamHandler#test_emit_normal().
  TestSafeStreamHandler.test_emit_closed_stream: SafeStreamHandler#test_emit_closed_stream().
  TestSafeStreamHandler.test_emit_pytest_stream: SafeStreamHandler#test_emit_pytest_stream().
  TestSafeStreamHandler.test_emit_non_writable_stream: SafeStreamHandler#test_emit_non_writable_stream().
  TestSafeStreamHandler.test_emit_value_error: SafeStreamHandler#test_emit_value_error().
  TestSafeStreamHandler.test_emit_os_error: SafeStreamHandler#test_emit_os_error().
  TestQuietMode.test_init_enabled: QuietMode#test_init_enabled().
  TestQuietMode.test_init_disabled: QuietMode#test_init_disabled().
  TestQuietMode.test_enter_sets_level: QuietMode#test_enter_sets_level().
  TestQuietMode.test_exit_restores_level: QuietMode#test_exit_restores_level().
  TestQuietMode.test_no_level_change_when_disabled: QuietMode#test_no_level_change_when_disabled().
  TestQuietMode.test_multiple_nested_contexts: QuietMode#test_multiple_nested_contexts().
  TestLoggingContext.test_init_enabled: LoggingContext#test_init_enabled().
  TestLoggingContext.test_init_disabled: LoggingContext#test_init_disabled().
  TestLoggingContext.test_enter_sets_level: LoggingContext#test_enter_sets_level().
  TestLoggingContext.test_exit_restores_level: LoggingContext#test_exit_restores_level().
  TestLoggingContext.test_notset_level_restores_info: LoggingContext#test_notset_level_restores_info().
  TestLogInfo.test_log_info_normal: LogInfo#test_log_info_normal().
  TestLogInfo.test_log_info_with_args: LogInfo#test_log_info_with_args().
  TestLogInfo.test_log_info_with_kwargs: LogInfo#test_log_info_with_kwargs().
  TestLogInfo.test_log_info_exception_handling: LogInfo#test_log_info_exception_handling().
  TestLogWarning.test_log_warning_normal: LogWarning#test_log_warning_normal().
  TestLogWarning.test_log_warning_exception_handling: LogWarning#test_log_warning_exception_handling().
  TestLogError.test_log_error_normal: LogError#test_log_error_normal().
  TestLogError.test_log_error_exception_handling: LogError#test_log_error_exception_handling().
  TestLogDebug.test_log_debug_normal: LogDebug#test_log_debug_normal().
  TestLogDebug.test_log_debug_exception_handling: LogDebug#test_log_debug_exception_handling().
  TestLogPerformance.test_log_performance_basic: LogPerformance#test_log_performance_basic().
  TestLogPerformance.test_log_performance_with_execution_time: LogPerformance#test_log_performance_with_execution_time().
  TestLogPerformance.test_log_performance_with_details: LogPerformance#test_log_performance_with_details().
  TestLogPerformance.test_log_performance_with_all_params: LogPerformance#test_log_performance_with_all_params().
  TestLogPerformance.test_log_performance_exception_handling: LogPerformance#test_log_performance_exception_handling().
  TestSetupLogger.test_setup_logger_default: SetupLogger#test_setup_logger_default().
  TestSetupLogger.test_setup_logger_debug_level: SetupLogger#test_setup_logger_debug_level().
  TestSetupLogger.test_setup_logger_info_level: SetupLogger#test_setup_logger_info_level().
  TestSetupLogger.test_setup_logger_warning_level: SetupLogger#test_setup_logger_warning_level().
  TestSetupLogger.test_setup_logger_error_level: SetupLogger#test_setup_logger_error_level().
  TestSetupLogger.test_setup_logger_invalid_level: SetupLogger#test_setup_logger_invalid_level().
  TestSetupLogger.test_setup_logger_env_debug: SetupLogger#test_setup_logger_env_debug().
  TestSetupLogger.test_setup_logger_env_info: SetupLogger#test_setup_logger_env_info().
  TestSetupLogger.test_setup_logger_test_logger: SetupLogger#test_setup_logger_test_logger().
  TestSetupLogger.test_setup_logger_file_logging_enabled: SetupLogger#test_setup_logger_file_logging_enabled().
  TestSetupLogger.test_setup_logger_file_logging_custom_dir: SetupLogger#test_setup_logger_file_logging_custom_dir().
  TestSetupLogger.test_setup_logger_file_log_level: SetupLogger#test_setup_logger_file_log_level().
  TestSafeStreamHandler.test_init_default_stream: SafeStreamHandler#test_init_default_stream().
  TestSafeStreamHandler.test_init_custom_stream: SafeStreamHandler#test_init_custom_stream().
  TestSuppressOutput.test_suppress_output_normal: SuppressOutput#test_suppress_output_normal().
  TestSuppressOutput.test_suppress_output_in_testing: SuppressOutput#test_suppress_output_in_testing().
  TestSuppressOutput.test_suppress_output_exception_handling: SuppressOutput#test_suppress_output_exception_handling().
  TestSafePrint.test_safe_print_info_level: SafePrint#test_safe_print_info_level().
  TestSafePrint.test_safe_print_warning_level: SafePrint#test_safe_print_warning_level().
  TestSafePrint.test_safe_print_error_level: SafePrint#test_safe_print_error_level().
  TestSafePrint.test_safe_print_debug_level: SafePrint#test_safe_print_debug_level().
  TestSafePrint.test_safe_print_none_message: SafePrint#test_safe_print_none_message().
  TestSafePrint.test_safe_print_quiet: SafePrint#test_safe_print_quiet().
  TestSafePrint.test_safe_print_default_level: SafePrint#test_safe_print_default_level().
  TestCreatePerformanceLogger.test_create_performance_logger: CreatePerformanceLogger#test_create_performance_logger().
  TestCreatePerformanceLogger.test_create_performance_logger_handler: CreatePerformanceLogger#test_create_performance_logger_handler().
  TestCreatePerformanceLogger.test_create_performance_logger_inherits_root_level: CreatePerformanceLogger#test_create_performance_logger_inherits_root_level().
  TestSetupPerformanceLogger.test_setup_performance_logger: SetupPerformanceLogger#test_setup_performance_logger().
  TestSetupPerformanceLogger.test_setup_performance_logger_no_duplicate: SetupPerformanceLogger#test_setup_performance_logger_no_duplicate().
  TestSafeStreamHandler.test_emit_stream_no_write.NoWriteStream: SafeStreamHandler#test_emit_stream_no_write().NoWriteStream#
  TestSetupLogger: SetupLogger#
  TestSafeStreamHandler: SafeStreamHandler#
  TestQuietMode: QuietMode#
  TestLoggingContext: LoggingContext#
  TestLogInfo: LogInfo#
  TestLogWarning: LogWarning#
  TestLogError: LogError#
  TestLogDebug: LogDebug#
  TestSuppressOutput: SuppressOutput#
  TestSafePrint: SafePrint#
  TestLogPerformance: LogPerformance#
  TestCreatePerformanceLogger: CreatePerformanceLogger#
  TestSetupPerformanceLogger: SetupPerformanceLogger#
  TestIntegration: Integration#
---
# Module: [`tests/unit/utils/test_logging.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py)

## Classes
### `NoWriteStream`
- def: [`tests/unit/utils/test_logging.py:232`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L232)
- signature: `class NoWriteStream:`
- used by: (1 test-only callers)

### `TestCreatePerformanceLogger`
- def: [`tests/unit/utils/test_logging.py:664`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L664)
- doc: 测试 create_performance_logger 函数
- signature: `class TestCreatePerformanceLogger:`
- members:
  - `test_create_performance_logger(self)` — [`L667`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L667) — 测试性能日志器创建
  - `test_create_performance_logger_handler(self)` — [`L673`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L673) — 测试性能日志器处理器
  - `test_create_performance_logger_inherits_root_level(self)` — [`L678`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L678) — Perf logger inherits root level (no hard-coded DEBUG).
- uses (calls/refs, reference-scoped): [`create_performance_logger`](../../../tree_sitter_analyzer/utils/logging.md#create_performance_logger)

### `TestIntegration`
- def: [`tests/unit/utils/test_logging.py:723`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L723)
- doc: 测试集成场景
- signature: `class TestIntegration:`
- members:
  - `test_complete_logging_workflow(self)` — [`L726`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L726) — 测试完整日志工作流
  - `test_logging_context_integration(self)` — [`L763`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L763) — 测试日志上下文集成
  - `test_quiet_mode_integration(self)` — [`L751`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L751) — 测试安静模式集成
- uses (calls/refs, reference-scoped): [`log_debug`](../../../tree_sitter_analyzer/utils/logging.md#log_debug), [`log_error`](../../../tree_sitter_analyzer/utils/logging.md#log_error), [`log_warning`](../../../tree_sitter_analyzer/utils/logging.md#log_warning), [`logger`](../../../tree_sitter_analyzer/utils/logging.md#logger), [`log_info`](../../../tree_sitter_analyzer/utils/logging.md#log_info), [`LoggingContext`](../../../tree_sitter_analyzer/utils/logging.md#LoggingContext), [`log_performance`](../../../tree_sitter_analyzer/utils/logging.md#log_performance), [`perf_logger`](../../../tree_sitter_analyzer/utils/logging.md#perf_logger), [`QuietMode`](../../../tree_sitter_analyzer/utils/logging.md#QuietMode)

### `TestLogDebug`
- def: [`tests/unit/utils/test_logging.py:501`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L501)
- doc: 测试 log_debug 函数
- signature: `class TestLogDebug:`
- members:
  - `test_log_debug_exception_handling(self)` — [`L510`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L510) — 测试异常处理
  - `test_log_debug_normal(self)` — [`L504`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L504) — 测试正常debug日志
- uses (calls/refs, reference-scoped): [`log_debug`](../../../tree_sitter_analyzer/utils/logging.md#log_debug), [`logger`](../../../tree_sitter_analyzer/utils/logging.md#logger)

### `TestLogError`
- def: [`tests/unit/utils/test_logging.py:484`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L484)
- doc: 测试 log_error 函数
- signature: `class TestLogError:`
- members:
  - `test_log_error_exception_handling(self)` — [`L494`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L494) — 测试异常处理
  - `test_log_error_normal(self)` — [`L487`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L487) — 测试正常error日志
- uses (calls/refs, reference-scoped): [`log_error`](../../../tree_sitter_analyzer/utils/logging.md#log_error), [`logger`](../../../tree_sitter_analyzer/utils/logging.md#logger)

### `TestLogInfo`
- def: [`tests/unit/utils/test_logging.py:432`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L432)
- doc: 测试 log_info 函数
- signature: `class TestLogInfo:`
- members:
  - `test_log_info_exception_handling(self)` — [`L456`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L456) — 测试异常处理
  - `test_log_info_normal(self)` — [`L435`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L435) — 测试正常info日志
  - `test_log_info_with_args(self)` — [`L442`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L442) — 测试带参数的info日志
  - `test_log_info_with_kwargs(self)` — [`L449`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L449) — 测试带kwargs的info日志
- uses (calls/refs, reference-scoped): [`logger`](../../../tree_sitter_analyzer/utils/logging.md#logger), [`log_info`](../../../tree_sitter_analyzer/utils/logging.md#log_info)

### `TestLogPerformance`
- def: [`tests/unit/utils/test_logging.py:616`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L616)
- doc: 测试 log_performance 函数
- signature: `class TestLogPerformance:`
- members:
  - `test_log_performance_basic(self)` — [`L619`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L619) — 测试基本性能日志
  - `test_log_performance_exception_handling(self)` — [`L657`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L657) — 测试异常处理
  - `test_log_performance_with_all_params(self)` — [`L644`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L644) — 测试带所有参数的性能日志
  - `test_log_performance_with_details(self)` — [`L636`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L636) — 测试带详细信息的性能日志
  - `test_log_performance_with_execution_time(self)` — [`L628`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L628) — 测试带执行时间的性能日志
- uses (calls/refs, reference-scoped): [`log_performance`](../../../tree_sitter_analyzer/utils/logging.md#log_performance), [`perf_logger`](../../../tree_sitter_analyzer/utils/logging.md#perf_logger)

### `TestLogWarning`
- def: [`tests/unit/utils/test_logging.py:464`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L464)
- doc: 测试 log_warning 函数
- signature: `class TestLogWarning:`
- members:
  - `test_log_warning_exception_handling(self)` — [`L474`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L474) — 测试异常处理
  - `test_log_warning_normal(self)` — [`L467`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L467) — 测试正常warning日志
- uses (calls/refs, reference-scoped): [`log_warning`](../../../tree_sitter_analyzer/utils/logging.md#log_warning), [`logger`](../../../tree_sitter_analyzer/utils/logging.md#logger)

### `TestLoggingContext`
- def: [`tests/unit/utils/test_logging.py:382`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L382)
- doc: 测试 LoggingContext 上下文管理器
- signature: `class TestLoggingContext:`
- members:
  - `test_enter_sets_level(self)` — [`L401`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L401) — 测试进入时设置级别
  - `test_exit_restores_level(self)` — [`L411`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L411) — 测试退出时恢复级别
  - `test_init_disabled(self)` — [`L390`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L390) — 测试禁用的日志上下文
  - `test_init_enabled(self)` — [`L385`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L385) — 测试启用的日志上下文
  - `test_init_with_level(self)` — [`L395`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L395) — 测试带级别的初始化
  - `test_notset_level_restores_info(self)` — [`L421`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L421) — 测试NOTSET级别恢复到INFO
- uses (calls/refs, reference-scoped): [`logger`](../../../tree_sitter_analyzer/utils/logging.md#logger), [`LoggingContext`](../../../tree_sitter_analyzer/utils/logging.md#LoggingContext), [`enabled`](../../../tree_sitter_analyzer/utils/logging.md#LoggingContext.enabled), [`old_level`](../../../tree_sitter_analyzer/utils/logging.md#LoggingContext.old_level), [`level`](../../../tree_sitter_analyzer/utils/logging.md#LoggingContext.level)

### `TestQuietMode`
- def: [`tests/unit/utils/test_logging.py:326`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L326)
- doc: 测试 QuietMode 上下文管理器
- signature: `class TestQuietMode:`
- members:
  - `test_enter_sets_level(self)` — [`L339`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L339) — 测试进入时设置级别
  - `test_exit_restores_level(self)` — [`L349`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L349) — 测试退出时恢复级别
  - `test_init_disabled(self)` — [`L334`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L334) — 测试禁用的安静模式
  - `test_init_enabled(self)` — [`L329`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L329) — 测试启用的安静模式
  - `test_multiple_nested_contexts(self)` — [`L369`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L369) — 测试嵌套上下文
  - `test_no_level_change_when_disabled(self)` — [`L359`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L359) — 测试禁用时不改变级别
- uses (calls/refs, reference-scoped): [`logger`](../../../tree_sitter_analyzer/utils/logging.md#logger), [`QuietMode`](../../../tree_sitter_analyzer/utils/logging.md#QuietMode), [`enabled`](../../../tree_sitter_analyzer/utils/logging.md#QuietMode.enabled)

### `TestSafePrint`
- def: [`tests/unit/utils/test_logging.py:561`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L561)
- doc: 测试 safe_print 函数
- signature: `class TestSafePrint:`
- members:
  - `test_safe_print_debug_level(self)` — [`L587`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L587) — 测试debug级别打印
  - `test_safe_print_default_level(self)` — [`L608`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L608) — 测试默认级别
  - `test_safe_print_error_level(self)` — [`L580`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L580) — 测试error级别打印
  - `test_safe_print_info_level(self)` — [`L564`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L564) — 测试info级别打印
  - `test_safe_print_none_message(self)` — [`L594`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L594) — 测试None消息
  - `test_safe_print_quiet(self)` — [`L601`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L601) — 测试安静模式
  - `test_safe_print_warning_level(self)` — [`L571`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L571) — 测试warning级别打印
- uses (calls/refs, reference-scoped): [`safe_print`](../../../tree_sitter_analyzer/utils/logging.md#safe_print)

### `TestSafeStreamHandler`
- def: [`tests/unit/utils/test_logging.py:179`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L179)
- doc: 测试 SafeStreamHandler 类
- signature: `class TestSafeStreamHandler:`
- members:
  - `test_emit_closed_stream(self)` — [`L209`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L209) — 测试关闭的流 - SafeStreamHandler应该安全处理
  - `test_emit_non_writable_stream(self)` — [`L269`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L269) — 测试不可写流
  - `test_emit_normal(self)` — [`L193`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L193) — 测试正常输出
  - `test_emit_os_error(self)` — [`L306`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L306) — 测试OSError异常
  - `test_emit_pytest_stream(self)` — [`L251`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L251) — 测试pytest流
  - `test_emit_stream_no_write(self)` — [`L228`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L228) — 测试无写入方法的流
  - `test_emit_value_error(self)` — [`L287`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L287) — 测试ValueError异常
  - `test_init_custom_stream(self)` — [`L187`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L187) — 测试自定义流
  - `test_init_default_stream(self)` — [`L182`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L182) — 测试默认流
- uses (calls/refs, reference-scoped): [`SafeStreamHandler`](../../../tree_sitter_analyzer/utils/logging.md#SafeStreamHandler), [`emit`](../../../tree_sitter_analyzer/utils/logging.md#SafeStreamHandler.emit)  (1 test-only)

### `TestSetupLogger`
- def: [`tests/unit/utils/test_logging.py:39`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L39)
- doc: 测试 setup_logger 函数
- signature: `class TestSetupLogger:`
- members:
  - `test_setup_logger_debug_level(self)` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L50) — 测试DEBUG级别
  - `test_setup_logger_default(self)` — [`L42`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L42) — 测试默认日志设置
  - `test_setup_logger_env_debug(self)` — [`L79`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L79) — 测试环境变量DEBUG级别
  - `test_setup_logger_env_info(self)` — [`L85`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L85) — 测试环境变量INFO级别
  - `test_setup_logger_error_level(self)` — [`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L68) — 测试ERROR级别
  - `test_setup_logger_file_log_level(self)` — [`L153`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L153) — 测试文件日志级别
  - `test_setup_logger_file_logging_custom_dir(self)` — [`L125`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L125) — 测试自定义日志目录
  - `test_setup_logger_file_logging_enabled(self)` — [`L102`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L102) — 测试启用文件日志
  - `test_setup_logger_info_level(self)` — [`L56`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L56) — 测试INFO级别
  - `test_setup_logger_invalid_level(self)` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L73) — 测试无效级别
  - `test_setup_logger_test_logger(self)` — [`L91`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L91) — 测试测试日志器
  - `test_setup_logger_warning_level(self)` — [`L62`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L62) — 测试WARNING级别
- uses (calls/refs, reference-scoped): [`setup_logger`](../../../tree_sitter_analyzer/utils/logging.md#setup_logger)

### `TestSetupPerformanceLogger`
- def: [`tests/unit/utils/test_logging.py:696`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L696)
- doc: 测试 setup_performance_logger 函数
- signature: `class TestSetupPerformanceLogger:`
- members:
  - `test_setup_performance_logger(self)` — [`L699`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L699) — 测试性能日志器设置
  - `test_setup_performance_logger_no_duplicate(self)` — [`L709`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L709) — 测试不重复添加处理器
- uses (calls/refs, reference-scoped): [`setup_performance_logger`](../../../tree_sitter_analyzer/utils/logging.md#setup_performance_logger)

### `TestSuppressOutput`
- def: [`tests/unit/utils/test_logging.py:517`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L517)
- doc: 测试 suppress_output 装饰器
- signature: `class TestSuppressOutput:`
- members:
  - `test_func()` — [`L524`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L524)
  - `test_suppress_output_exception_handling(self)` — [`L550`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L550) — 测试异常处理
  - `test_suppress_output_in_testing(self)` — [`L531`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L531) — 测试测试模式下的输出抑制
  - `test_suppress_output_normal(self)` — [`L520`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_logging.py#L520) — 测试正常输出抑制
- uses (calls/refs, reference-scoped): [`suppress_output`](../../../tree_sitter_analyzer/utils/logging.md#suppress_output)

