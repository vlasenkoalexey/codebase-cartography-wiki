---
title: 'Module: scripts/format_monitoring_tool.py'
type: catalog
provenance: extracted
module: scripts/format_monitoring_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `scripts.format_monitoring_tool`/
symbols:
  FormatMonitor.monitor_file: FormatMonitor#monitor_file().
  FormatMonitor.generate_monitoring_report: FormatMonitor#generate_monitoring_report().
  project_root: project_root.
  FormatMonitor._monitor_format_type: FormatMonitor#_monitor_format_type().
  FormatMonitor._check_format_regression: FormatMonitor#_check_format_regression().
  FormatMonitor.db: FormatMonitor#db.
  FormatMonitor._validate_format_compliance: FormatMonitor#_validate_format_compliance().
  FormatMonitor._generate_summary_report: FormatMonitor#_generate_summary_report().
  FormatMonitor._generate_performance_report: FormatMonitor#_generate_performance_report().
  main: main().
  FormatMonitoringDatabase.db_path: FormatMonitoringDatabase#db_path.
  FormatMonitor._generate_regression_report: FormatMonitor#_generate_regression_report().
  FormatMonitoringDatabase.get_recent_regressions: FormatMonitoringDatabase#get_recent_regressions().
  FormatMonitoringDatabase.get_performance_trends: FormatMonitoringDatabase#get_performance_trends().
  FormatMonitor.logger: FormatMonitor#logger.
  FormatMonitoringDatabase.init_database: FormatMonitoringDatabase#init_database().
  FormatMonitoringDatabase.record_validation: FormatMonitoringDatabase#record_validation().
  FormatMonitoringDatabase.record_regression: FormatMonitoringDatabase#record_regression().
  FormatMonitoringDatabase.record_performance: FormatMonitoringDatabase#record_performance().
  FormatMonitor.golden_master_manager: FormatMonitor#golden_master_manager.
  FormatMonitoringDatabase.__init__: FormatMonitoringDatabase#__init__().
  FormatMonitoringDatabase.record_quality_metrics: FormatMonitoringDatabase#record_quality_metrics().
  FormatMonitoringDatabase: FormatMonitoringDatabase#
  FormatMonitor: FormatMonitor#
  FormatMonitor._setup_logging: FormatMonitor#_setup_logging().
  FormatMonitor._detect_language: FormatMonitor#_detect_language().
  FormatMonitor._generate_quality_trends_report: FormatMonitor#_generate_quality_trends_report().
  FormatMonitor._generate_performance_recommendations: FormatMonitor#_generate_performance_recommendations().
  FormatMonitor._generate_html_dashboard: FormatMonitor#_generate_html_dashboard().
  FormatMonitor.__init__: FormatMonitor#__init__().
  FormatMonitor.cross_component_validator: FormatMonitor#cross_component_validator.
---
# Module: [`scripts/format_monitoring_tool.py`](../../../../../raw/code/tree-sitter-analyzer/scripts/format_monitoring_tool.py)

## Classes
### `FormatMonitor`
- def: [`scripts/format_monitoring_tool.py:290`](../../../../../raw/code/tree-sitter-analyzer/scripts/format_monitoring_tool.py#L290)
- doc: Format monitoring and analysis tool
- signature: `class FormatMonitor:`
- members:
  - `_check_format_regression(self, output: str, format_type: str, file_path: str, output_hash: str)` — [`L479`](../../../../../raw/code/tree-sitter-analyzer/scripts/format_monitoring_tool.py#L479) — Check for format regressions using golden master comparison
  - `_detect_language(self, file_path: Path)` — [`L409`](../../../../../raw/code/tree-sitter-analyzer/scripts/format_monitoring_tool.py#L409) — Detect programming language from file extension
  - `_generate_html_dashboard(self, reports: dict[str, Any], output_file: Path)` — [`L644`](../../../../../raw/code/tree-sitter-analyzer/scripts/format_monitoring_tool.py#L644) — Generate HTML dashboard for monitoring reports
  - `_generate_performance_recommendations(self, trends: dict[str, list[dict[str, Any]]])` — [`L628`](../../../../../raw/code/tree-sitter-analyzer/scripts/format_monitoring_tool.py#L628) — Generate performance recommendations based on trends
  - `_generate_performance_report(self)` — [`L606`](../../../../../raw/code/tree-sitter-analyzer/scripts/format_monitoring_tool.py#L606) — Generate performance-focused report
  - `_generate_quality_trends_report(self)` — [`L616`](../../../../../raw/code/tree-sitter-analyzer/scripts/format_monitoring_tool.py#L616) — Generate quality trends report
  - `_generate_regression_report(self)` — [`L578`](../../../../../raw/code/tree-sitter-analyzer/scripts/format_monitoring_tool.py#L578) — Generate regression-focused report
  - `_generate_summary_report(self)` — [`L553`](../../../../../raw/code/tree-sitter-analyzer/scripts/format_monitoring_tool.py#L553) — Generate summary monitoring report
  - `_monitor_format_type(self, file_path: str, format_type: str, language: str, temp_dir: str)` — [`L361`](../../../../../raw/code/tree-sitter-analyzer/scripts/format_monitoring_tool.py#L361) — Monitor specific format type for a file
  - `_setup_logging(self)` — [`L299`](../../../../../raw/code/tree-sitter-analyzer/scripts/format_monitoring_tool.py#L299) — Setup logging for monitoring
  - `_validate_format_compliance(self, output: str, format_type: str)` — [`L422`](../../../../../raw/code/tree-sitter-analyzer/scripts/format_monitoring_tool.py#L422) — Validate format compliance and calculate score
  - `generate_monitoring_report(self, output_dir: str = "./monitoring-reports")` — [`L516`](../../../../../raw/code/tree-sitter-analyzer/scripts/format_monitoring_tool.py#L516) — Generate comprehensive monitoring report
  - `monitor_file(self, file_path: str, temp_dir: str)` — [`L313`](../../../../../raw/code/tree-sitter-analyzer/scripts/format_monitoring_tool.py#L313) — Monitor format output for a single file
  - `cross_component_validator` — [`L296`](../../../../../raw/code/tree-sitter-analyzer/scripts/format_monitoring_tool.py#L296)
  - `db` — [`L294`](../../../../../raw/code/tree-sitter-analyzer/scripts/format_monitoring_tool.py#L294)
  - `golden_master_manager` — [`L295`](../../../../../raw/code/tree-sitter-analyzer/scripts/format_monitoring_tool.py#L295)
  - `logger` — [`L297`](../../../../../raw/code/tree-sitter-analyzer/scripts/format_monitoring_tool.py#L297)
- protocol/private: `__init__`[`L293`](../../../../../raw/code/tree-sitter-analyzer/scripts/format_monitoring_tool.py#L293)
- uses (calls/refs, reference-scoped): [`AnalyzeCodeStructureTool`](../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#AnalyzeCodeStructureTool), [`execute`](../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#AnalyzeCodeStructureTool.execute), [`get_performance_trends`](format_monitoring_tool.md#FormatMonitoringDatabase.get_performance_trends), [`get_recent_regressions`](format_monitoring_tool.md#FormatMonitoringDatabase.get_recent_regressions), [`record_performance`](format_monitoring_tool.md#FormatMonitoringDatabase.record_performance), [`record_regression`](format_monitoring_tool.md#FormatMonitoringDatabase.record_regression), [`record_validation`](format_monitoring_tool.md#FormatMonitoringDatabase.record_validation), [`FormatMonitoringDatabase`](format_monitoring_tool.md#FormatMonitoringDatabase)  (7 test-only)
- used by: [`main`](format_monitoring_tool.md#main)

### `FormatMonitoringDatabase`
- def: [`scripts/format_monitoring_tool.py:33`](../../../../../raw/code/tree-sitter-analyzer/scripts/format_monitoring_tool.py#L33)
- doc: Database for storing format monitoring data
- signature: `class FormatMonitoringDatabase:`
- members:
  - `get_performance_trends(self, days: int = 30)` — [`L254`](../../../../../raw/code/tree-sitter-analyzer/scripts/format_monitoring_tool.py#L254) — Get performance trends by format type
  - `get_recent_regressions(self, days: int = 7)` — [`L232`](../../../../../raw/code/tree-sitter-analyzer/scripts/format_monitoring_tool.py#L232) — Get recent format regressions
  - `init_database(self)` — [`L40`](../../../../../raw/code/tree-sitter-analyzer/scripts/format_monitoring_tool.py#L40) — Initialize monitoring database
  - `record_performance(self, file_path: str, format_type: str, metrics: dict[str, Any])` — [`L178`](../../../../../raw/code/tree-sitter-analyzer/scripts/format_monitoring_tool.py#L178) — Record format performance metrics
  - `record_quality_metrics(self, format_type: str, metrics: dict[str, Any])` — [`L206`](../../../../../raw/code/tree-sitter-analyzer/scripts/format_monitoring_tool.py#L206) — Record format quality metrics
  - `record_regression(self, file_path: str, format_type: str, regression_type: str, description: str, severity: str)` — [`L147`](../../../../../raw/code/tree-sitter-analyzer/scripts/format_monitoring_tool.py#L147) — Record format regression
  - `record_validation(self, file_path: str, format_type: str, language: str, result: dict[str, Any])` — [`L116`](../../../../../raw/code/tree-sitter-analyzer/scripts/format_monitoring_tool.py#L116) — Record format validation result
  - `db_path` — [`L37`](../../../../../raw/code/tree-sitter-analyzer/scripts/format_monitoring_tool.py#L37)
- protocol/private: `__init__`[`L36`](../../../../../raw/code/tree-sitter-analyzer/scripts/format_monitoring_tool.py#L36)
- used by: [`monitor_file`](format_monitoring_tool.md#FormatMonitor.monitor_file), [`db`](format_monitoring_tool.md#FormatMonitor.db), [`_generate_performance_report`](format_monitoring_tool.md#FormatMonitor._generate_performance_report), [`_generate_summary_report`](format_monitoring_tool.md#FormatMonitor._generate_summary_report), [`_generate_regression_report`](format_monitoring_tool.md#FormatMonitor._generate_regression_report)

## Functions
- `main()` — [`L698`](../../../../../raw/code/tree-sitter-analyzer/scripts/format_monitoring_tool.py#L698) — Main monitoring function

## Module values
- `project_root` — [`L23`](../../../../../raw/code/tree-sitter-analyzer/scripts/format_monitoring_tool.py#L23)

